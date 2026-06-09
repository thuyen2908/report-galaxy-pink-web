# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: close-out.feature.spec.js >> Close Out report >> Technician report display correctly
- Location: dist/bdd/close-out.feature.spec.js:14:3

# Error details

```
Error: expect(locator).toHaveText(expected) failed

Locator:  locator('.bill-render').locator('.sales-details .sales-row').filter({ hasNot: locator('.bill-render').locator('.total-row') }).first().locator('.tip')
Expected: "$10.00"
Received: "$0.00"
Timeout:  30000ms

Call log:
  - Expect "toHaveText" with timeout 30000ms
  - waiting for locator('.bill-render').locator('.sales-details .sales-row').filter({ hasNot: locator('.bill-render').locator('.total-row') }).first().locator('.tip')
    63 × locator resolved to <div class="tip">$0.00</div>
       - unexpected value "$0.00"

```

```yaml
- text: $0.00
```

# Test source

```ts
  4385 | 
  4386 | 		await expect(targetChip).toBeVisible();
  4387 | 		await expect(targetChip).toContainText(expectedValue);
  4388 | 	},
  4389 | );
  4390 | Then(
  4391 | 	'I should see the position employee {string} is {string}',
  4392 | 	async ({ page }, employeeName: string, position: string) => {
  4393 | 		const listEmployee = page.locator('ul.ListItemEmployee__wrap ').first();
  4394 | 		await expect(listEmployee).toBeVisible();
  4395 | 
  4396 | 		const employeeRow = listEmployee
  4397 | 			.locator('li.xEmployeeItem')
  4398 | 			.filter({ hasText: employeeName });
  4399 | 		await expect(employeeRow).toBeVisible();
  4400 | 
  4401 | 		const numberPosition = employeeRow.locator('.number');
  4402 | 		await expect(numberPosition).toBeVisible();
  4403 | 		await expect(numberPosition).toHaveText(position);
  4404 | 	},
  4405 | );
  4406 | 
  4407 | Then(
  4408 | 	'I should see the header {string} in the bill render',
  4409 | 	async ({ page }, header: string) => {
  4410 | 		const billRender = page.locator('.bill-render');
  4411 | 		await expect(billRender).toBeVisible();
  4412 | 
  4413 | 		const headerElement = billRender
  4414 | 			.locator('p.header')
  4415 | 			.getByText(header, { exact: true });
  4416 | 		await expect(headerElement).toBeVisible();
  4417 | 	},
  4418 | );
  4419 | 
  4420 | Then(
  4421 | 	'I should see the detail {string} in the bill render',
  4422 | 	async ({ page }, detail: string) => {
  4423 | 		const colonIndex = detail.indexOf(':');
  4424 | 		if (colonIndex === -1) {
  4425 | 			throw new Error(
  4426 | 				`Invalid detail format: "${detail}". Expected format: "Label: Value"`,
  4427 | 			);
  4428 | 		}
  4429 | 
  4430 | 		const labelPart = detail.substring(0, colonIndex).trim(); // E.g.: "Technician Name"
  4431 | 		const expectedValue = detail.substring(colonIndex + 1).trim(); // E.g.: "Elena"
  4432 | 
  4433 | 		const infoRow = page.locator('.info-row').filter({
  4434 | 			has: page.locator('.info-label', {
  4435 | 				hasText: new RegExp(`^\\s*${labelPart}\\s*:?\\s*$`),
  4436 | 			}),
  4437 | 		});
  4438 | 
  4439 | 		await expect(infoRow).toBeVisible();
  4440 | 
  4441 | 		const valueElement = infoRow.locator('.info-value');
  4442 | 		await expect(valueElement).toBeVisible();
  4443 | 		await expect(valueElement).toContainText(expectedValue);
  4444 | 	},
  4445 | );
  4446 | 
  4447 | Then(
  4448 | 	'I should see the {string} with value {string} in the sale row detail',
  4449 | 	async ({ page }, field: string, value: string) => {
  4450 | 		const billRender = page.locator('.bill-render');
  4451 | 		await expect(billRender).toBeVisible();
  4452 | 
  4453 | 		const salesRow = billRender
  4454 | 			.locator('.sales-details .sales-row')
  4455 | 			.filter({ hasNot: billRender.locator('.total-row') })
  4456 | 			.first();
  4457 | 		await expect(salesRow).toBeVisible();
  4458 | 
  4459 | 		const fieldToSelector: Record<string, string> = {
  4460 | 			'Item Name': '.item-name',
  4461 | 			QTY: '.quantity',
  4462 | 			Tip: '.tip',
  4463 | 			Amount: '.amount',
  4464 | 		};
  4465 | 
  4466 | 		const selector = fieldToSelector[field];
  4467 | 		if (!selector) {
  4468 | 			throw new Error(
  4469 | 				`Unsupported sale row field: "${field}". Supported fields: ${Object.keys(
  4470 | 					fieldToSelector,
  4471 | 				).join(', ')}`,
  4472 | 			);
  4473 | 		}
  4474 | 
  4475 | 		const cell = salesRow.locator(selector);
  4476 | 		await expect(cell).toBeVisible();
  4477 | 
  4478 | 		if (field === 'Item Name') {
  4479 | 			const cellText = (await cell.innerText()).replace(/\s+/g, ' ').trim();
  4480 | 			const expected = value.replace(/\s+/g, ' ').trim();
  4481 | 			expect(cellText).toContain(expected);
  4482 | 			return;
  4483 | 		}
  4484 | 
> 4485 | 		await expect(cell).toHaveText(value, { useInnerText: true });
       |                      ^ Error: expect(locator).toHaveText(expected) failed
  4486 | 	},
  4487 | );
  4488 | 
  4489 | Then(
  4490 | 	'I should see the summary detail {string} in the bill render',
  4491 | 	async ({ page }, detail: string) => {
  4492 | 		const match = detail.match(/^(.*?)\s+(\$?-?[\d,.]+(?:\/\d+)?)$/);
  4493 | 
  4494 | 		let label: string;
  4495 | 		let expectedValue: string;
  4496 | 
  4497 | 		if (match) {
  4498 | 			label = match[1].trim();
  4499 | 			expectedValue = match[2].trim();
  4500 | 		} else {
  4501 | 			const lastSpaceIndex = detail.trim().lastIndexOf(' ');
  4502 | 			label = detail.trim().slice(0, lastSpaceIndex).trim();
  4503 | 			expectedValue = detail
  4504 | 				.trim()
  4505 | 				.slice(lastSpaceIndex + 1)
  4506 | 				.trim();
  4507 | 		}
  4508 | 
  4509 | 		const summaryRow = page.locator('.summary-row').filter({
  4510 | 			has: page.locator('.summary-label', {
  4511 | 				hasText: new RegExp(`^${label}$`, 'i'),
  4512 | 			}),
  4513 | 		});
  4514 | 
  4515 | 		await expect(summaryRow).toBeVisible();
  4516 | 
  4517 | 		const valueElement = summaryRow.locator('.summary-value');
  4518 | 		await expect(valueElement).toHaveText(expectedValue);
  4519 | 	},
  4520 | );
  4521 | 
  4522 | Then(
  4523 | 	'I should see the employee {string} is not at position 1',
  4524 | 	async ({ page }, employeeName: string) => {
  4525 | 		const listEmployee = page.locator('ul.ListItemEmployee__wrap ').first();
  4526 | 		await expect(listEmployee).toBeVisible();
  4527 | 		const employeeRow = listEmployee
  4528 | 			.locator('li.xEmployeeItem')
  4529 | 			.filter({ hasText: employeeName });
  4530 | 		await expect(employeeRow).toBeVisible();
  4531 | 		const numberPosition = employeeRow.locator('.number');
  4532 | 		await expect(numberPosition).toBeVisible();
  4533 | 		await expect(numberPosition).not.toHaveText('#1');
  4534 | 	},
  4535 | );
  4536 | When('I click the Delete ticket button', async ({ page }) => {
  4537 | 	const buttonDelete = page.locator('svg[data-testid="DeleteIcon"]');
  4538 | 	await buttonDelete.click();
  4539 | });
  4540 | 
  4541 | Then(
  4542 | 	'I should see the Tech, Deductions, Tip, Amount as {string} in the bill render',
  4543 | 	async ({ page }, expectedRow: string) => {
  4544 | 		const [tech, deductions, tip, amount] = expectedRow.split(' ');
  4545 | 
  4546 | 		const row = page.locator('.sales-row').filter({
  4547 | 			has: page.locator('.tech-name', { hasText: tech }),
  4548 | 		});
  4549 | 
  4550 | 		await expect(row).toBeVisible();
  4551 | 
  4552 | 		await expect(row.locator('.deductions')).toHaveText(deductions);
  4553 | 		await expect(row.locator('.tip')).toHaveText(tip);
  4554 | 		await expect(row.locator('.amount')).toHaveText(amount);
  4555 | 	},
  4556 | );
  4557 | 
  4558 | Then(
  4559 | 	'The department name should be {string}',
  4560 | 	async ({ page }, name: string) => {
  4561 | 		await expect(
  4562 | 			page.getByRole('dialog').locator('input[name="name"]'),
  4563 | 		).toHaveValue(name);
  4564 | 	},
  4565 | );
  4566 | 
  4567 | Then(
  4568 | 	'The department type should be {string}',
  4569 | 	async ({ page }, type: string) => {
  4570 | 		await expect(
  4571 | 			page
  4572 | 				.getByRole('dialog')
  4573 | 				.getByRole('combobox', { name: /department type/i }),
  4574 | 		).toHaveText(new RegExp(type, 'i'));
  4575 | 	},
  4576 | );
  4577 | 
  4578 | Then('department type should be {string}', async ({ page }, type: string) => {
  4579 | 	const deptTypeCell = page
  4580 | 		.locator('.MuiDataGrid-row')
  4581 | 		.first()
  4582 | 		.locator('[data-field="deptType"]');
  4583 | 
  4584 | 	await expect(deptTypeCell).toContainText(type);
  4585 | });
```