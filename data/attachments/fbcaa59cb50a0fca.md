# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: payroll.feature.spec.js >> Payroll >> Commission payroll details in the Owner View are calculated correctly
- Location: dist/bdd/payroll.feature.spec.js:129:3

# Error details

```
Error: expect(locator).toContainText(expected) failed

Locator: locator('table tbody tr').filter({ hasText: 'Credit Card Fee:' }).first().locator('td').nth(1)
Expected substring: "($0.25)"
Received string:    "$0.00"
Timeout: 30000ms

Call log:
  - Expect "toContainText" with timeout 30000ms
  - waiting for locator('table tbody tr').filter({ hasText: 'Credit Card Fee:' }).first().locator('td').nth(1)
    63 × locator resolved to <td>…</td>
       - unexpected value "$0.00"

```

```yaml
- cell "$0.00"
```

# Test source

```ts
  4158 | 		await expect(divider).toBeVisible();
  4159 | 		await expect(divider.locator('span.item-divider')).toHaveText(text);
  4160 | 	},
  4161 | );
  4162 | 
  4163 | Then(
  4164 | 	'I should see the Total Sales, Net Comm, NC Tip, Total Payout as {string} in employee view',
  4165 | 	async ({ page }, expectedValues: string) => {
  4166 | 		const values = expectedValues.split(' ');
  4167 | 		expect(values).toHaveLength(4);
  4168 | 
  4169 | 		const [totalSales, netComm, ncTip, totalPayout] = values;
  4170 | 
  4171 | 		const detailsTable = page.locator('table.details-payroll');
  4172 | 		const dataRow = detailsTable.locator('tbody tr').nth(1);
  4173 | 
  4174 | 		await expect(dataRow).toBeVisible();
  4175 | 
  4176 | 		const totalSalesCell = dataRow.locator('td').nth(2);
  4177 | 		const netCommCell = dataRow.locator('td').nth(3);
  4178 | 		const ncTipCell = dataRow.locator('td').nth(4);
  4179 | 		const totalPayoutCell = dataRow.locator('td').nth(5);
  4180 | 
  4181 | 		await expect(totalSalesCell).toHaveText(totalSales);
  4182 | 		await expect(netCommCell).toHaveText(netComm);
  4183 | 		await expect(ncTipCell).toHaveText(ncTip);
  4184 | 		await expect(totalPayoutCell).toHaveText(totalPayout);
  4185 | 	},
  4186 | );
  4187 | 
  4188 | Then(
  4189 | 	'I should see the technician name {string} in the employee view',
  4190 | 	async ({ page }, technicianName: string) => {
  4191 | 		const technicianRow = page
  4192 | 			.locator('table tbody tr')
  4193 | 			.filter({ hasText: 'Technician' });
  4194 | 		const nameCell = technicianRow.locator('td').nth(1);
  4195 | 
  4196 | 		await expect(nameCell).toBeVisible();
  4197 | 		await expect(nameCell).toHaveText(technicianName);
  4198 | 	},
  4199 | );
  4200 | 
  4201 | Then(
  4202 | 	'I should see the payroll type {string} in the employee view',
  4203 | 	async ({ page }, payrollType: string) => {
  4204 | 		const typeRow = page
  4205 | 			.locator('table tbody tr')
  4206 | 			.filter({ hasText: 'Payroll Type' });
  4207 | 		const typeCell = typeRow.locator('td').nth(1);
  4208 | 
  4209 | 		await expect(typeCell).toBeVisible();
  4210 | 		await expect(typeCell).toHaveText(payrollType);
  4211 | 	},
  4212 | );
  4213 | 
  4214 | Then(
  4215 | 	'I should see the # of Work Days {string} in the employee view',
  4216 | 	async ({ page }, workDays: string) => {
  4217 | 		const workDaysRow = page
  4218 | 			.locator('table tbody tr')
  4219 | 			.filter({ hasText: '# of Work Days' });
  4220 | 		const workDaysCell = workDaysRow.locator('td').nth(1);
  4221 | 
  4222 | 		await expect(workDaysCell).toBeVisible();
  4223 | 		await expect(workDaysCell).toHaveText(workDays);
  4224 | 	},
  4225 | );
  4226 | 
  4227 | Then(
  4228 | 	'I should see the text {string} in the single payroll view',
  4229 | 	async ({ page }, text: string) => {
  4230 | 		const saleSummaryRow = page
  4231 | 			.locator('table tbody tr')
  4232 | 			.filter({ hasText: text });
  4233 | 		await expect(saleSummaryRow).toBeVisible();
  4234 | 	},
  4235 | );
  4236 | 
  4237 | Then(
  4238 | 	'I should see the detail {string} in the single payroll view',
  4239 | 	async ({ page }, detail: string) => {
  4240 | 		const colonIndex = detail.indexOf(':');
  4241 | 		if (colonIndex === -1) {
  4242 | 			throw new Error(
  4243 | 				`Invalid detail format: "${detail}". Expected format: "Label: Value"`,
  4244 | 			);
  4245 | 		}
  4246 | 
  4247 | 		const label = detail.substring(0, colonIndex + 1).trim();
  4248 | 		const expectedValue = detail.substring(colonIndex + 1).trim();
  4249 | 
  4250 | 		const detailRow = page
  4251 | 			.locator('table tbody tr')
  4252 | 			.filter({ hasText: label })
  4253 | 			.first();
  4254 | 
  4255 | 		const valueCell = detailRow.locator('td').nth(1);
  4256 | 
  4257 | 		await expect(valueCell).toBeVisible();
> 4258 | 		await expect(valueCell).toContainText(expectedValue);
       |                           ^ Error: expect(locator).toContainText(expected) failed
  4259 | 	},
  4260 | );
  4261 | 
  4262 | Then(
  4263 | 	'I should see the second Total {string} in the single payroll view',
  4264 | 	async ({ page }, amount: string) => {
  4265 | 		const totalRow = page
  4266 | 			.locator('table tbody tr')
  4267 | 			.filter({ hasText: 'Total' })
  4268 | 			.nth(1);
  4269 | 		const amountCell = totalRow.locator('td').nth(1);
  4270 | 
  4271 | 		await expect(amountCell).toBeVisible();
  4272 | 		await expect(amountCell).toHaveText(amount);
  4273 | 	},
  4274 | );
  4275 | 
  4276 | Then(
  4277 | 	'I should see the Reg Pay, NC Tip, Commission as {string} in employee view',
  4278 | 	async ({ page }, expectedValues: string) => {
  4279 | 		const values = expectedValues.split(' ');
  4280 | 		expect(values).toHaveLength(3);
  4281 | 
  4282 | 		const [regPay, ncTip, commission] = values;
  4283 | 
  4284 | 		const detailsTable = page.locator('table.details-payroll');
  4285 | 		const dataRow = detailsTable.locator('tbody tr').nth(1);
  4286 | 
  4287 | 		await expect(dataRow).toBeVisible();
  4288 | 
  4289 | 		// const totalSalesCell = dataRow.locator('td').nth(2);
  4290 | 		const regPayCell = dataRow.locator('td').nth(3);
  4291 | 		const ncTipCell = dataRow.locator('td').nth(4);
  4292 | 		const commissionCell = dataRow.locator('td').nth(5);
  4293 | 
  4294 | 		// await expect(totalSalesCell).toHaveText(regHrs);
  4295 | 		await expect(regPayCell).toHaveText(regPay);
  4296 | 		await expect(ncTipCell).toHaveText(ncTip);
  4297 | 		await expect(commissionCell).toHaveText(commission);
  4298 | 	},
  4299 | );
  4300 | 
  4301 | Then(
  4302 | 	'I should see the first Total {string} in the single payroll view',
  4303 | 	async ({ page }, amount: string) => {
  4304 | 		const totalRow = page
  4305 | 			.locator('table tbody tr')
  4306 | 			.filter({ hasText: 'Total' })
  4307 | 			.first();
  4308 | 		const amountCell = totalRow.locator('td').nth(1);
  4309 | 
  4310 | 		await expect(amountCell).toBeVisible();
  4311 | 		await expect(amountCell).toHaveText(amount);
  4312 | 	},
  4313 | );
  4314 | When('I waiting 1s', async ({ page }) => {
  4315 | 	await page.waitForTimeout(1000);
  4316 | });
  4317 | 
  4318 | When('I click on the reset key', async ({ page }) => {
  4319 | 	const resetButton = page.locator('svg[data-testid="XResetIcon"]');
  4320 | 	await expect(resetButton).toBeVisible();
  4321 | 	await resetButton.click();
  4322 | });
  4323 | Then('I should see no results found', async ({ page }) => {
  4324 | 	const noResults = page.locator('text=No results found');
  4325 | 	await expect(noResults).toBeVisible();
  4326 | });
  4327 | Then(
  4328 | 	'I should see the new void reason name {string} {string}, created at today, in the list',
  4329 | 	async ({ page }, field: string, value: string) => {
  4330 | 		const newRow = page.locator('.MuiDataGrid-row', {
  4331 | 			has: page.locator(`[data-field="${field}"]`, { hasText: value }),
  4332 | 		});
  4333 | 
  4334 | 		const valueCell = newRow.locator(`[data-field="${field}"]`);
  4335 | 		const dateCell = newRow.locator('[data-field="createdAt"]');
  4336 | 
  4337 | 		const formattedToday = await page.evaluate(() => {
  4338 | 			const today = new Date();
  4339 | 			return today.toLocaleDateString('en-US', {
  4340 | 				year: 'numeric',
  4341 | 				month: '2-digit',
  4342 | 				day: '2-digit',
  4343 | 			});
  4344 | 		});
  4345 | 
  4346 | 		await expect(valueCell).toBeVisible();
  4347 | 		await expect(valueCell).toHaveText(value);
  4348 | 		await expect(dateCell).toBeVisible();
  4349 | 		await expect(dateCell).toContainText(formattedToday);
  4350 | 	},
  4351 | );
  4352 | Then(
  4353 | 	'I should see the {string} Adjustment',
  4354 | 	async ({ page }, Title: string) => {
  4355 | 		const titleAdjustTurn = page.locator('.dailyTask__title');
  4356 | 
  4357 | 		await expect(titleAdjustTurn).toBeVisible();
  4358 | 		await expect(titleAdjustTurn).toHaveText(Title);
```