# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: check-in.feature.spec.js >> Check In >> Delete a waiting
- Location: dist/bdd/check-in.feature.spec.js:234:3

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: locator('.MuiAlert-message').filter({ hasText: 'Item successfully deleted' })
Expected: visible
Timeout: 30000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 30000ms
  - waiting for locator('.MuiAlert-message').filter({ hasText: 'Item successfully deleted' })

```

```yaml
- banner:
  - button
  - img
  - text: "FUNCTIONS 11 : 00 : 20 PM 06/08/2026"
  - listitem: Balance
  - separator
  - listitem: WAIT
  - separator
  - listitem: APPT BOOK
  - separator
  - listitem: FAST SALE
  - text: "PINK SALON 1032 YONKERS AVE Yonkers Avenel, NJ, 07001 | (090) 123-4567 Pos Pink | Station: 1"
- img
- text: Galaxy Pink 2025.12
- list
- text: PINK SALON
- paragraph: 1032 YONKERS AVE Yonkers Avenel, NJ, 07001
- text: (090) 123-4567 Pos Pink
- paragraph
- text: BUSINESS DATE 06/08/2026
- paragraph: © 2026 XSoftware
- main:
  - tablist:
    - tab "NAILS" [selected]
    - tab "HAIR"
  - tabpanel:
    - list:
      - listitem
      - listitem
    - list:
      - listitem: "A #1 Addison 12:00:00 AM T = 0.00 C = 0.0 L = 0.00 12:00 AM"
      - listitem: "B #2 Bella 12:00:00 AM T = 0.00 C = 0.0 L = 0.00 12:00 AM"
      - listitem: "D #3 David 12:00:00 AM T = 0.00 C = 0.0 L = 0.00 12:00 AM"
      - listitem: "J #4 Jarvis 12:00:00 AM T = 0.00 C = 0.0 L = 0.00 12:00 AM"
      - listitem: "W #5 WorkSlipAdjustTip2 12:00:00 AM T = 0.00 C = 0.0 L = 0.00 12:00 AM"
      - listitem: "Z #6 Zoey 12:00:00 AM T = 0.00 C = 0.0 L = 0.00 12:00 AM"
      - listitem: "A #7 Almira 07:00:00 AM T = 0.00 C = 0.0 L = 0.00 07:00 AM"
      - listitem: "A #8 Amelia 07:00:00 AM T = 0.00 C = 0.0 L = 0.00 07:00 AM"
      - listitem: "A #9 Avery 07:00:00 AM T = 0.00 C = 0.0 L = 0.00 07:00 AM"
      - listitem: "B #10 Brian 07:00:00 AM T = 0.00 C = 0.0 L = 0.00 07:00 AM"
      - listitem: "C #11 Ciara 07:00:00 AM T = 0.00 C = 0.0 L = 0.00 07:00 AM"
      - listitem: "E #12 Eira 07:00:00 AM T = 0.00 C = 0.0 L = 0.00 07:00 AM"
      - listitem:
        - img "item service Emma"
        - text: "#13 Emma 07:00:00 AM T = 0.00 C = 0.0 L = 0.00 07:00 AM"
      - listitem: "E #14 Ethan 07:00:00 AM T = 0.00 C = 0.0 L = 0.00 07:00 AM"
      - listitem: "G #15 Gabriella 07:00:00 AM T = 0.00 C = 0.0 L = 0.00 07:00 AM"
      - listitem: "H #16 Hailey 07:00:00 AM T = 0.00 C = 0.0 L = 0.00 07:00 AM"
      - listitem: "H #17 Hanna 07:00:00 AM T = 0.00 C = 0.0 L = 0.00 07:00 AM"
      - listitem: "H #18 Harry 07:00:00 AM T = 0.00 C = 0.0 L = 0.00 07:00 AM"
      - listitem: "J #19 Jack 07:00:00 AM T = 0.00 C = 0.0 L = 0.00 07:00 AM"
      - listitem: "K #20 Kim 07:00:00 AM T = 0.00 C = 0.0 L = 0.00 07:00 AM"
      - listitem: "L #21 Laura 07:00:00 AM T = 0.00 C = 0.0 L = 0.00 07:00 AM"
      - listitem: "L #22 Leah 07:00:00 AM T = 0.00 C = 0.0 L = 0.00 07:00 AM"
      - listitem: "L #23 Lisa 07:00:00 AM T = 0.00 C = 0.0 L = 0.00 07:00 AM"
      - listitem: "M #24 Maya 07:00:00 AM T = 0.00 C = 0.0 L = 0.00 07:00 AM"
      - listitem: "R #25 Ruby 07:00:00 AM T = 0.00 C = 0.0 L = 0.00 07:00 AM"
      - listitem: "S #26 Sam 07:00:00 AM T = 0.00 C = 0.0 L = 0.00 07:00 AM"
      - listitem: "S #27 Sandy 07:00:00 AM T = 0.00 C = 0.0 L = 0.00 07:00 AM"
      - listitem: "S #28 Sarah 07:00:00 AM T = 0.00 C = 0.0 L = 0.00 07:00 AM"
      - listitem: "S #29 Savannah 07:00:00 AM T = 0.00 C = 0.0 L = 0.00 07:00 AM"
      - listitem: "S #30 Sophia 07:00:00 AM T = 0.00 C = 0.0 L = 0.00 07:00 AM"
      - listitem: "T #31 Tina 07:00:00 AM T = 0.00 C = 0.0 L = 0.00 07:00 AM"
      - listitem: "T #32 Tom 07:00:00 AM T = 0.00 C = 0.0 L = 0.00 07:00 AM"
      - listitem: "V #33 Victoria 07:00:00 AM T = 0.00 C = 0.0 L = 0.00 07:00 AM"
      - listitem: "E #34 Emily 10:58:39 PM T = 6.00 C = 0.0 L = 6.00 07:00 AM"
      - listitem: "K #35 Kelley 10:59:07 PM T = 6.00 C = 0.0 L = 6.00 07:00 AM"
      - listitem: "C #36 Claire 10:58:39 PM T = 8.00 C = 0.0 L = 8.00 07:00 AM"
      - listitem: "A #37 Anna 11:00:04 PM T = 22.00 C = 1.0 L = 22.00 12:00 AM"
      - listitem: "C #38 Christ 10:59:35 PM T = 61.50 C = 3.0 L = 41.50 07:00 AM"
  - button "reload"
  - tablist:
    - tab "SERVICE"
    - tab "WAITING LIST" [selected]
    - tab "CLOSED TICKET"
    - tab "TURN DETAILS"
  - tabpanel:
    - button "Column Settings"
    - searchbox "Search…"
    - grid:
      - row "Status Time Ticket# Customer Service Technician":
        - columnheader "Status"
        - columnheader "Time"
        - columnheader "Ticket#"
        - columnheader "Customer"
        - columnheader "Service"
        - columnheader "Technician"
        - columnheader
      - rowgroup:
        - row "#8 11:00 PM 0 Recreate Full set Anna":
          - gridcell "#8"
          - gridcell "11:00 PM"
          - gridcell "0"
          - gridcell "Recreate"
          - gridcell "Full set"
          - gridcell "Anna"
          - gridcell
- alert: Create Waiting
```

# Test source

```ts
  2508 | 			await expect(headerElement).toBeVisible();
  2509 | 			await expect(headerElement).toContainText(header);
  2510 | 		}
  2511 | 	},
  2512 | );
  2513 | 
  2514 | Then(
  2515 | 	'I should see the Batch history table displayed correctly',
  2516 | 	async ({ page }) => {
  2517 | 		const headers = [
  2518 | 			'Batch Date',
  2519 | 			'Application',
  2520 | 			'Transactions Count',
  2521 | 			'Return Amount',
  2522 | 			'Sale Amount',
  2523 | 			'Total Amount',
  2524 | 			'Void Amount',
  2525 | 			'Transactions',
  2526 | 		];
  2527 | 
  2528 | 		for (const header of headers) {
  2529 | 			const headerElement = page
  2530 | 				.locator('.MuiDataGrid-columnHeaderTitleContainerContent')
  2531 | 				.getByText(header, { exact: true });
  2532 | 			await expect(headerElement).toBeVisible();
  2533 | 			await expect(headerElement).toContainText(header);
  2534 | 		}
  2535 | 	},
  2536 | );
  2537 | 
  2538 | Then('I should see the icon zoom out', async ({ page }) => {
  2539 | 	const zoomOutIcon = page.locator('[data-testid="ZoomOutIcon"]');
  2540 | 	await expect(zoomOutIcon).toBeVisible();
  2541 | });
  2542 | 
  2543 | When('I click on the icon zoom out', async ({ page }) => {
  2544 | 	await page.locator('[data-testid="ZoomOutIcon"]').click();
  2545 | });
  2546 | 
  2547 | When(
  2548 | 	'I click button clock in for employee {string}',
  2549 | 	async ({ page }, employeeNickname: string) => {
  2550 | 		const targetRow = page.locator('.MuiDataGrid-row').filter({
  2551 | 			has: page.locator('.MuiDataGrid-cell[data-field="nickName"]', {
  2552 | 				hasText: employeeNickname,
  2553 | 			}),
  2554 | 		});
  2555 | 
  2556 | 		const clockInButton = targetRow.locator('button', {
  2557 | 			hasText: 'CLOCK IN',
  2558 | 		});
  2559 | 
  2560 | 		await expect(targetRow.first()).toBeVisible();
  2561 | 		await clockInButton.first().scrollIntoViewIfNeeded();
  2562 | 		await expect(clockInButton.first()).toBeVisible();
  2563 | 		await clockInButton.first().click();
  2564 | 	},
  2565 | );
  2566 | 
  2567 | Then(
  2568 | 	'I should see the first ticket with total {string}',
  2569 | 	async ({ page }, amount: string) => {
  2570 | 		const totalElement = page
  2571 | 			.locator('.MuiDataGrid-row')
  2572 | 			.locator('[data-field="ticketTotals"]', { hasText: amount })
  2573 | 			.first();
  2574 | 		await expect(totalElement).not.toHaveText('Ticket Totals');
  2575 | 		await expect(totalElement).toContainText(amount);
  2576 | 		await expect(totalElement).toBeVisible();
  2577 | 	},
  2578 | );
  2579 | 
  2580 | Then(
  2581 | 	'I should see the Auto Turn 1.00 for {string}',
  2582 | 	async ({ page }, name: string) => {
  2583 | 		const row = page.locator('tr').filter({
  2584 | 			has: page.locator(`[title="${name}"]`),
  2585 | 		});
  2586 | 		const autoTurn = row.locator('td[turntype="AutoTicket"]', {
  2587 | 			hasText: '1.00',
  2588 | 		});
  2589 | 		await expect(autoTurn).toBeVisible();
  2590 | 	},
  2591 | );
  2592 | 
  2593 | When(
  2594 | 	'I click on the queue {string} button',
  2595 | 	async ({ page }, queue: string) => {
  2596 | 		const queueButton = page.locator('.MuiButtonBase-root', { hasText: queue });
  2597 | 		await expect(queueButton).toBeVisible();
  2598 | 		await queueButton.click();
  2599 | 	},
  2600 | );
  2601 | 
  2602 | Then(
  2603 | 	'I should see the toast message {string} visible',
  2604 | 	async ({ page }, message: string) => {
  2605 | 		const toastMessage = page.locator('.MuiAlert-message', {
  2606 | 			hasText: message,
  2607 | 		});
> 2608 | 		await expect(toastMessage).toBeVisible();
       |                              ^ Error: expect(locator).toBeVisible() failed
  2609 | 	},
  2610 | );
  2611 | 
  2612 | When(
  2613 | 	'I select the {string} service in my cart',
  2614 | 	async ({ page }, service: string) => {
  2615 | 		const serviceButton = page.locator('.xTicketItems__name', {
  2616 | 			hasText: service,
  2617 | 		});
  2618 | 		await expect(serviceButton).toBeVisible();
  2619 | 		await serviceButton.click();
  2620 | 	},
  2621 | );
  2622 | 
  2623 | When(
  2624 | 	'I double click on the first turn detail for {string}',
  2625 | 	async ({ page }, name: string) => {
  2626 | 		const row = page.locator('tr').filter({
  2627 | 			has: page.locator(`[title="${name}"]`),
  2628 | 		});
  2629 | 		const firstTurnDetail = row.locator('td').nth(1);
  2630 | 		await expect(firstTurnDetail).toBeVisible();
  2631 | 		await firstTurnDetail.dblclick();
  2632 | 	},
  2633 | );
  2634 | 
  2635 | When('I click on refresh', async ({ page }) => {
  2636 | 	await page.locator('[data-testid="RefreshOutlinedIconIcon"]').click();
  2637 | });
  2638 | 
  2639 | Then(
  2640 | 	'I should see the print button {string} visible',
  2641 | 	async ({ page }, button: string) => {
  2642 | 		const printButton = page.getByRole('button', { name: button });
  2643 | 		await expect(printButton).toBeVisible();
  2644 | 	},
  2645 | );
  2646 | 
  2647 | Then(
  2648 | 	'I should see the Auto Turn -1.00 for {string}',
  2649 | 	async ({ page }, name: string) => {
  2650 | 		const row = page.locator('tr').filter({
  2651 | 			has: page.locator(`[title="${name}"]`),
  2652 | 		});
  2653 | 		await expect(row).toBeVisible();
  2654 | 
  2655 | 		const turnCell = row.locator('td', {
  2656 | 			has: page.locator('.MuiChip-label', { hasText: '-1.00' }),
  2657 | 		});
  2658 | 		await expect(turnCell.first()).toBeVisible();
  2659 | 	},
  2660 | );
  2661 | 
  2662 | Then(
  2663 | 	'I should see the Auto Turn 50.00 for {string}',
  2664 | 	async ({ page }, name: string) => {
  2665 | 		const row = page.locator('tr').filter({
  2666 | 			has: page.locator(`[title="${name}"]`),
  2667 | 		});
  2668 | 		await expect(row).toBeVisible();
  2669 | 
  2670 | 		const turnCell = row.locator('td', {
  2671 | 			has: page.locator('.MuiChip-label', { hasText: '50.00' }),
  2672 | 		});
  2673 | 		await expect(turnCell.first()).toBeVisible();
  2674 | 	},
  2675 | );
  2676 | 
  2677 | Then(
  2678 | 	'I should see the employee {string} listed first in the employee list',
  2679 | 	async ({ page }, employeeName: string) => {
  2680 | 		const firstEmployee = page
  2681 | 			.locator('div.xQueueList li.xEmployeeItem')
  2682 | 			.first();
  2683 | 
  2684 | 		await expect(firstEmployee).toContainText(employeeName);
  2685 | 	},
  2686 | );
  2687 | 
  2688 | Then(
  2689 | 	'I should see the employee {string} listed last in the employee list',
  2690 | 	async ({ page }, employeeName: string) => {
  2691 | 		const lastEmployee = page.locator('div.xQueueList li.xEmployeeItem').last();
  2692 | 
  2693 | 		await expect(lastEmployee).toContainText(employeeName);
  2694 | 	},
  2695 | );
  2696 | 
  2697 | Then(
  2698 | 	'I should see the Turn -1.00 for {string}',
  2699 | 	async ({ page }, name: string) => {
  2700 | 		const row = page.locator('td').filter({
  2701 | 			has: page.getByTitle(name),
  2702 | 		});
  2703 | 		const turnLabel = row
  2704 | 			.locator('.MuiChip-root', { hasText: 'Turn' })
  2705 | 			.locator('.MuiChip-label', { hasText: '-1.00' });
  2706 | 		await expect(turnLabel).toBeVisible();
  2707 | 	},
  2708 | );
```