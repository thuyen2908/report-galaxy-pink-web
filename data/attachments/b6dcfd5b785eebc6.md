# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: departments.feature.spec.js >> Departments management >> Create a new department
- Location: dist/bdd/departments.feature.spec.js:15:3

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: locator('.MuiAlert-message').filter({ hasText: 'The data item has been created successfully' })
Expected: visible
Timeout: 30000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 30000ms
  - waiting for locator('.MuiAlert-message').filter({ hasText: 'The data item has been created successfully' })

```

# Page snapshot

```yaml
- generic [ref=e1]:
  - generic [ref=e4]:
    - banner [ref=e5]:
      - generic [ref=e6]:
        - button [ref=e7] [cursor=pointer]:
          - img [ref=e8]
        - img [ref=e12] [cursor=pointer]
        - generic [ref=e13]:
          - generic [ref=e16]: Departments
          - generic [ref=e18]:
            - generic [ref=e19]: PINK SALON
            - generic [ref=e20]: 1032 YONKERS AVE Yonkers Avenel, NJ, 07001 | (090) 123-4567
            - generic [ref=e21]: "Pos Pink | Station: 1"
    - generic [ref=e23]:
      - generic [ref=e24]:
        - img [ref=e26]
        - generic [ref=e27]:
          - generic [ref=e28]: Galaxy Pink
          - generic [ref=e29]: "2025.12"
      - generic [ref=e31]:
        - generic [ref=e33]:
          - generic [ref=e35]: PINK SALON
          - generic [ref=e36]:
            - paragraph [ref=e38]: 1032 YONKERS AVE Yonkers Avenel, NJ, 07001
            - generic [ref=e39]: (090) 123-4567
            - generic [ref=e40]: Pos Pink
        - paragraph [ref=e41]
        - generic [ref=e42]:
          - generic [ref=e43]: BUSINESS DATE
          - generic [ref=e44]: 04/06/2026
      - paragraph [ref=e45]: © 2026 XSoftware
    - main [ref=e46]:
      - generic [ref=e47]:
        - generic [ref=e49]:
          - generic [ref=e52]:
            - img [ref=e53]
            - searchbox [ref=e55]
          - grid [ref=e56]:
            - generic [ref=e57]:
              - row [ref=e58]:
                - columnheader [ref=e59] [cursor=pointer]:
                  - generic [ref=e61]: Department Name
                - columnheader [ref=e62] [cursor=pointer]:
                  - generic [ref=e64]: Department Type
                - columnheader [ref=e65] [cursor=pointer]:
                  - generic [ref=e67]: Non-Inventory
                - columnheader [ref=e68] [cursor=pointer]:
                  - generic [ref=e70]: Created At
                - columnheader [ref=e71] [cursor=pointer]:
                  - generic [ref=e73]: Created By
                - columnheader [ref=e74]:
                  - generic [ref=e76]: Actions
              - rowgroup [ref=e77]:
                - row [ref=e78]:
                  - gridcell [ref=e79]: Facial
                  - gridcell [ref=e80]: Service
                  - gridcell [ref=e81]:
                    - img [ref=e83]
                  - gridcell [ref=e85]: 01/07/2026 09:48 PM
                  - gridcell [ref=e86]: pos.xsofts@galaxyaccess.us
                  - gridcell [ref=e87]:
                    - menu [ref=e88]:
                      - menuitem [ref=e89] [cursor=pointer]:
                        - img [ref=e90]
                      - menuitem [ref=e92] [cursor=pointer]:
                        - img [ref=e93]
                      - menuitem [ref=e95] [cursor=pointer]:
                        - img [ref=e96]
                - row [ref=e98]:
                  - gridcell [ref=e99]: Nails
                  - gridcell [ref=e100]: Service
                  - gridcell [ref=e101]:
                    - img [ref=e103]
                  - gridcell [ref=e105]: 01/07/2026 09:48 PM
                  - gridcell [ref=e106]: pos.xsofts@galaxyaccess.us
                  - gridcell [ref=e107]:
                    - menu [ref=e108]:
                      - menuitem [ref=e109] [cursor=pointer]:
                        - img [ref=e110]
                      - menuitem [ref=e112] [cursor=pointer]:
                        - img [ref=e113]
                      - menuitem [ref=e115] [cursor=pointer]:
                        - img [ref=e116]
                - row [ref=e118]:
                  - gridcell [ref=e119]: Nails (4)
                  - gridcell [ref=e120]: Service
                  - gridcell [ref=e121]:
                    - img [ref=e123]
                  - gridcell [ref=e125]: 03/04/2026 09:09 PM
                  - gridcell [ref=e126]: pos.pink@galaxyaccess.us
                  - gridcell [ref=e127]:
                    - menu [ref=e128]:
                      - menuitem [ref=e129] [cursor=pointer]:
                        - img [ref=e130]
                      - menuitem [ref=e132] [cursor=pointer]:
                        - img [ref=e133]
                      - menuitem [ref=e135] [cursor=pointer]:
                        - img [ref=e136]
                - row [ref=e138]:
                  - gridcell [ref=e139]: Hair
                  - gridcell [ref=e140]: Service
                  - gridcell [ref=e141]:
                    - img [ref=e143]
                  - gridcell [ref=e145]: 01/07/2026 09:48 PM
                  - gridcell [ref=e146]: pos.xsofts@galaxyaccess.us
                  - gridcell [ref=e147]:
                    - menu [ref=e148]:
                      - menuitem [ref=e149] [cursor=pointer]:
                        - img [ref=e150]
                      - menuitem [ref=e152] [cursor=pointer]:
                        - img [ref=e153]
                      - menuitem [ref=e155] [cursor=pointer]:
                        - img [ref=e156]
                - row [ref=e158]:
                  - gridcell [ref=e159]: Waxing
                  - gridcell [ref=e160]: Service
                  - gridcell [ref=e161]:
                    - img [ref=e163]
                  - gridcell [ref=e165]: 01/07/2026 09:48 PM
                  - gridcell [ref=e166]: pos.xsofts@galaxyaccess.us
                  - gridcell [ref=e167]:
                    - menu [ref=e168]:
                      - menuitem [ref=e169] [cursor=pointer]:
                        - img [ref=e170]
                      - menuitem [ref=e172] [cursor=pointer]:
                        - img [ref=e173]
                      - menuitem [ref=e175] [cursor=pointer]:
                        - img [ref=e176]
                - row [ref=e178]:
                  - gridcell [ref=e179]: Nails (0)
                  - gridcell [ref=e180]: Service
                  - gridcell [ref=e181]:
                    - img [ref=e183]
                  - gridcell [ref=e185]: 03/04/2026 05:08 AM
                  - gridcell [ref=e186]: pos.pink@galaxyaccess.us
                  - gridcell [ref=e187]:
                    - menu [ref=e188]:
                      - menuitem [ref=e189] [cursor=pointer]:
                        - img [ref=e190]
                      - menuitem [ref=e192] [cursor=pointer]:
                        - img [ref=e193]
                      - menuitem [ref=e195] [cursor=pointer]:
                        - img [ref=e196]
                - row [ref=e198]:
                  - gridcell [ref=e199]: Massage
                  - gridcell [ref=e200]: Service
                  - gridcell [ref=e201]:
                    - img [ref=e203]
                  - gridcell [ref=e205]: 01/07/2026 09:48 PM
                  - gridcell [ref=e206]: pos.xsofts@galaxyaccess.us
                  - gridcell [ref=e207]:
                    - menu [ref=e208]:
                      - menuitem [ref=e209] [cursor=pointer]:
                        - img [ref=e210]
                      - menuitem [ref=e212] [cursor=pointer]:
                        - img [ref=e213]
                      - menuitem [ref=e215] [cursor=pointer]:
                        - img [ref=e216]
                - row [ref=e218]:
                  - gridcell [ref=e219]: Eyelash
                  - gridcell [ref=e220]: Service
                  - gridcell [ref=e221]:
                    - img [ref=e223]
                  - gridcell [ref=e225]: 01/07/2026 09:48 PM
                  - gridcell [ref=e226]: pos.xsofts@galaxyaccess.us
                  - gridcell [ref=e227]:
                    - menu [ref=e228]:
                      - menuitem [ref=e229] [cursor=pointer]:
                        - img [ref=e230]
                      - menuitem [ref=e232] [cursor=pointer]:
                        - img [ref=e233]
                      - menuitem [ref=e235] [cursor=pointer]:
                        - img [ref=e236]
                - row [ref=e238]:
                  - gridcell [ref=e239]: Fancy Nails
                  - gridcell [ref=e240]: Service
                  - gridcell [ref=e241]:
                    - img [ref=e243]
                  - gridcell [ref=e245]: 03/04/2026 05:07 AM
                  - gridcell [ref=e246]: pos.pink@galaxyaccess.us
                  - gridcell [ref=e247]:
                    - menu [ref=e248]:
                      - menuitem [ref=e249] [cursor=pointer]:
                        - img [ref=e250]
                      - menuitem [ref=e252] [cursor=pointer]:
                        - img [ref=e253]
                      - menuitem [ref=e255] [cursor=pointer]:
                        - img [ref=e256]
                - row [ref=e258]:
                  - gridcell [ref=e259]: Product
                  - gridcell [ref=e260]: Product
                  - gridcell [ref=e261]:
                    - img [ref=e263]
                  - gridcell [ref=e265]: 01/07/2026 09:48 PM
                  - gridcell [ref=e266]: pos.xsofts@galaxyaccess.us
                  - gridcell [ref=e267]:
                    - menu [ref=e268]:
                      - menuitem [ref=e269] [cursor=pointer]:
                        - img [ref=e270]
                      - menuitem [ref=e272] [cursor=pointer]:
                        - img [ref=e273]
                      - menuitem [ref=e275] [cursor=pointer]:
                        - img [ref=e276]
                - row [ref=e278]:
                  - gridcell [ref=e279]: Pedicure & Manicure
                  - gridcell [ref=e280]: Service
                  - gridcell [ref=e281]:
                    - img [ref=e283]
                  - gridcell [ref=e285]: 03/18/2026 05:07 AM
                  - gridcell [ref=e286]: pos.pink@galaxyaccess.us
                  - gridcell [ref=e287]:
                    - menu [ref=e288]:
                      - menuitem [ref=e289] [cursor=pointer]:
                        - img [ref=e290]
                      - menuitem [ref=e292] [cursor=pointer]:
                        - img [ref=e293]
                      - menuitem [ref=e295] [cursor=pointer]:
                        - img [ref=e296]
                - row [ref=e298]:
                  - gridcell [ref=e299]: Nails (2)
                  - gridcell [ref=e300]: Service
                  - gridcell [ref=e301]:
                    - img [ref=e303]
                  - gridcell [ref=e305]: 03/04/2026 09:08 PM
                  - gridcell [ref=e306]: pos.pink@galaxyaccess.us
                  - gridcell [ref=e307]:
                    - menu [ref=e308]:
                      - menuitem [ref=e309] [cursor=pointer]:
                        - img [ref=e310]
                      - menuitem [ref=e312] [cursor=pointer]:
                        - img [ref=e313]
                      - menuitem [ref=e315] [cursor=pointer]:
                        - img [ref=e316]
                - row [ref=e318]:
                  - gridcell [ref=e319]: Nails (3)
                  - gridcell [ref=e320]: Service
                  - gridcell [ref=e321]:
                    - img [ref=e323]
                  - gridcell [ref=e325]: 03/04/2026 09:09 PM
                  - gridcell [ref=e326]: pos.pink@galaxyaccess.us
                  - gridcell [ref=e327]:
                    - menu [ref=e328]:
                      - menuitem [ref=e329] [cursor=pointer]:
                        - img [ref=e330]
                      - menuitem [ref=e332] [cursor=pointer]:
                        - img [ref=e333]
                      - menuitem [ref=e335] [cursor=pointer]:
                        - img [ref=e336]
                - row [ref=e338]:
                  - gridcell [ref=e339]: Nails (1)
                  - gridcell [ref=e340]: Service
                  - gridcell [ref=e341]:
                    - img [ref=e343]
                  - gridcell [ref=e345]: 03/04/2026 05:09 AM
                  - gridcell [ref=e346]: pos.pink@galaxyaccess.us
                  - gridcell [ref=e347]:
                    - menu [ref=e348]:
                      - menuitem [ref=e349] [cursor=pointer]:
                        - img [ref=e350]
                      - menuitem [ref=e352] [cursor=pointer]:
                        - img [ref=e353]
                      - menuitem [ref=e355] [cursor=pointer]:
                        - img [ref=e356]
          - generic [ref=e362]:
            - paragraph [ref=e363]: "Rows per page:"
            - generic [ref=e364]:
              - combobox [ref=e365] [cursor=pointer]: "50"
              - textbox: "50"
              - img
            - paragraph [ref=e366]: 1–14 of 14
            - generic [ref=e367]:
              - button [disabled]:
                - img
              - button [disabled]:
                - img
        - generic [ref=e368]:
          - button [ref=e369] [cursor=pointer]:
            - img [ref=e371]
            - text: Refresh
          - button [ref=e374] [cursor=pointer]:
            - img [ref=e376]
            - text: Add New
  - alert [ref=e378]: Home
  - dialog "Create New Department" [ref=e381]:
    - heading "Create New Department" [level=2] [ref=e382]
    - button "close" [ref=e383] [cursor=pointer]:
      - img [ref=e384]
    - generic [ref=e386]:
      - generic [ref=e387]:
        - generic [ref=e389]:
          - generic [ref=e390]:
            - text: Department Name
            - generic [ref=e391]: "*"
          - generic [ref=e392]:
            - textbox "Department Name" [ref=e393]: Pedicure & Manicure
            - group:
              - generic: Department Name *
        - generic [ref=e395]:
          - generic [ref=e396]:
            - text: Department Type
            - generic [ref=e397]: "*"
          - generic [ref=e398]:
            - combobox "Department Type Service" [ref=e399] [cursor=pointer]:
              - generic [ref=e401]: Service
            - textbox: Service
            - img
            - group:
              - generic: Department Type *
        - group [ref=e404]:
          - generic [ref=e405] [cursor=pointer]:
            - checkbox "Non-Inventory" [ref=e408]
            - generic [ref=e411]: Non-Inventory
      - generic [ref=e412]:
        - button "Save" [ref=e413] [cursor=pointer]:
          - img [ref=e415]
          - text: Save
        - button "Cancel" [ref=e417] [cursor=pointer]:
          - img [ref=e419]
          - text: Cancel
```

# Test source

```ts
  2462 | 			await expect(headerElement).toBeVisible();
  2463 | 			await expect(headerElement).toContainText(header);
  2464 | 		}
  2465 | 	},
  2466 | );
  2467 | 
  2468 | Then(
  2469 | 	'I should see the Batch history table displayed correctly',
  2470 | 	async ({ page }) => {
  2471 | 		const headers = [
  2472 | 			'Batch Date',
  2473 | 			'Application',
  2474 | 			'Transactions Count',
  2475 | 			'Return Amount',
  2476 | 			'Sale Amount',
  2477 | 			'Total Amount',
  2478 | 			'Void Amount',
  2479 | 			'Transactions',
  2480 | 		];
  2481 | 
  2482 | 		for (const header of headers) {
  2483 | 			const headerElement = page
  2484 | 				.locator('.MuiDataGrid-columnHeaderTitleContainerContent')
  2485 | 				.getByText(header, { exact: true });
  2486 | 			await expect(headerElement).toBeVisible();
  2487 | 			await expect(headerElement).toContainText(header);
  2488 | 		}
  2489 | 	},
  2490 | );
  2491 | 
  2492 | Then('I should see the icon zoom out', async ({ page }) => {
  2493 | 	const zoomOutIcon = page.locator('[data-testid="ZoomOutIcon"]');
  2494 | 	await expect(zoomOutIcon).toBeVisible();
  2495 | });
  2496 | 
  2497 | When('I click on the icon zoom out', async ({ page }) => {
  2498 | 	await page.locator('[data-testid="ZoomOutIcon"]').click();
  2499 | });
  2500 | 
  2501 | When(
  2502 | 	'I click button clock in for employee {string}',
  2503 | 	async ({ page }, employeeNickname: string) => {
  2504 | 		const targetRow = page.locator('.MuiDataGrid-row').filter({
  2505 | 			has: page.locator('.MuiDataGrid-cell[data-field="nickName"]', {
  2506 | 				hasText: employeeNickname,
  2507 | 			}),
  2508 | 		});
  2509 | 
  2510 | 		const clockInButton = targetRow.locator('button', {
  2511 | 			hasText: 'CLOCK IN',
  2512 | 		});
  2513 | 
  2514 | 		await expect(targetRow.first()).toBeVisible();
  2515 | 		await clockInButton.first().scrollIntoViewIfNeeded();
  2516 | 		await expect(clockInButton.first()).toBeVisible();
  2517 | 		await clockInButton.first().click();
  2518 | 	},
  2519 | );
  2520 | 
  2521 | Then(
  2522 | 	'I should see the first ticket with total {string}',
  2523 | 	async ({ page }, amount: string) => {
  2524 | 		const totalElement = page
  2525 | 			.locator('.MuiDataGrid-row')
  2526 | 			.locator('[data-field="ticketTotals"]', { hasText: amount })
  2527 | 			.first();
  2528 | 		await expect(totalElement).not.toHaveText('Ticket Totals');
  2529 | 		await expect(totalElement).toContainText(amount);
  2530 | 		await expect(totalElement).toBeVisible();
  2531 | 	},
  2532 | );
  2533 | 
  2534 | Then(
  2535 | 	'I should see the Auto Turn 1.00 for {string}',
  2536 | 	async ({ page }, name: string) => {
  2537 | 		const row = page.locator('tr').filter({
  2538 | 			has: page.locator(`[title="${name}"]`),
  2539 | 		});
  2540 | 		const autoTurn = row.locator('td[turntype="AutoTicket"]', {
  2541 | 			hasText: '1.00',
  2542 | 		});
  2543 | 		await expect(autoTurn).toBeVisible();
  2544 | 	},
  2545 | );
  2546 | 
  2547 | When(
  2548 | 	'I click on the queue {string} button',
  2549 | 	async ({ page }, queue: string) => {
  2550 | 		const queueButton = page.locator('.MuiButtonBase-root', { hasText: queue });
  2551 | 		await expect(queueButton).toBeVisible();
  2552 | 		await queueButton.click();
  2553 | 	},
  2554 | );
  2555 | 
  2556 | Then(
  2557 | 	'I should see the toast message {string} visible',
  2558 | 	async ({ page }, message: string) => {
  2559 | 		const toastMessage = page.locator('.MuiAlert-message', {
  2560 | 			hasText: message,
  2561 | 		});
> 2562 | 		await expect(toastMessage).toBeVisible();
       |                              ^ Error: expect(locator).toBeVisible() failed
  2563 | 	},
  2564 | );
  2565 | 
  2566 | When(
  2567 | 	'I select the {string} service in my cart',
  2568 | 	async ({ page }, service: string) => {
  2569 | 		const serviceButton = page.locator('.xTicketItems__name', {
  2570 | 			hasText: service,
  2571 | 		});
  2572 | 		await expect(serviceButton).toBeVisible();
  2573 | 		await serviceButton.click();
  2574 | 	},
  2575 | );
  2576 | 
  2577 | When(
  2578 | 	'I double click on the first turn detail for {string}',
  2579 | 	async ({ page }, name: string) => {
  2580 | 		const row = page.locator('tr').filter({
  2581 | 			has: page.locator(`[title="${name}"]`),
  2582 | 		});
  2583 | 		const firstTurnDetail = row.locator('td').nth(1);
  2584 | 		await expect(firstTurnDetail).toBeVisible();
  2585 | 		await firstTurnDetail.dblclick();
  2586 | 	},
  2587 | );
  2588 | 
  2589 | When('I click on refresh', async ({ page }) => {
  2590 | 	await page.locator('[data-testid="RefreshOutlinedIconIcon"]').click();
  2591 | });
  2592 | 
  2593 | Then(
  2594 | 	'I should see the print button {string} visible',
  2595 | 	async ({ page }, button: string) => {
  2596 | 		const printButton = page.getByRole('button', { name: button });
  2597 | 		await expect(printButton).toBeVisible();
  2598 | 	},
  2599 | );
  2600 | 
  2601 | Then(
  2602 | 	'I should see the Auto Turn -1.00 for {string}',
  2603 | 	async ({ page }, name: string) => {
  2604 | 		const row = page.locator('tr').filter({
  2605 | 			has: page.locator(`[title="${name}"]`),
  2606 | 		});
  2607 | 		await expect(row).toBeVisible();
  2608 | 
  2609 | 		const turnCell = row.locator('td', {
  2610 | 			has: page.locator('.MuiChip-label', { hasText: '-1.00' }),
  2611 | 		});
  2612 | 		await expect(turnCell.first()).toBeVisible();
  2613 | 	},
  2614 | );
  2615 | 
  2616 | Then(
  2617 | 	'I should see the Auto Turn 50.00 for {string}',
  2618 | 	async ({ page }, name: string) => {
  2619 | 		const row = page.locator('tr').filter({
  2620 | 			has: page.locator(`[title="${name}"]`),
  2621 | 		});
  2622 | 		await expect(row).toBeVisible();
  2623 | 
  2624 | 		const turnCell = row.locator('td', {
  2625 | 			has: page.locator('.MuiChip-label', { hasText: '50.00' }),
  2626 | 		});
  2627 | 		await expect(turnCell.first()).toBeVisible();
  2628 | 	},
  2629 | );
  2630 | 
  2631 | Then(
  2632 | 	'I should see the employee {string} listed first in the employee list',
  2633 | 	async ({ page }, employeeName: string) => {
  2634 | 		const firstEmployee = page
  2635 | 			.locator('div.xQueueList li.xEmployeeItem')
  2636 | 			.first();
  2637 | 
  2638 | 		await expect(firstEmployee).toContainText(employeeName);
  2639 | 	},
  2640 | );
  2641 | 
  2642 | Then(
  2643 | 	'I should see the employee {string} listed last in the employee list',
  2644 | 	async ({ page }, employeeName: string) => {
  2645 | 		const lastEmployee = page.locator('div.xQueueList li.xEmployeeItem').last();
  2646 | 
  2647 | 		await expect(lastEmployee).toContainText(employeeName);
  2648 | 	},
  2649 | );
  2650 | 
  2651 | Then(
  2652 | 	'I should see the Turn -1.00 for {string}',
  2653 | 	async ({ page }, name: string) => {
  2654 | 		const row = page.locator('td').filter({
  2655 | 			has: page.getByTitle(name),
  2656 | 		});
  2657 | 		const turnLabel = row
  2658 | 			.locator('.MuiChip-root', { hasText: 'Turn' })
  2659 | 			.locator('.MuiChip-label', { hasText: '-1.00' });
  2660 | 		await expect(turnLabel).toBeVisible();
  2661 | 	},
  2662 | );
```