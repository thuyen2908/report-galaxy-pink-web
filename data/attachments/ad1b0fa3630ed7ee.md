# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: ticket-adjustment.feature.spec.js >> Ticket adjustment >> Remove Tax and make new payment
- Location: dist/bdd/ticket-adjustment.feature.spec.js:372:3

# Error details

```
Error: expect(locator).not.toHaveText(expected) failed

Locator:  locator('.xCharge__taxes')
Expected: not "$0.00"
Received: "$0.00"
Timeout:  30000ms

Call log:
  - Expect "not toHaveText" with timeout 30000ms
  - waiting for locator('.xCharge__taxes')
    34 × locator resolved to <span class="xCharge__taxes">$0.00</span>
       - unexpected value "$0.00"

```

# Page snapshot

```yaml
- generic [active] [ref=e1]:
  - generic [ref=e4]:
    - banner [ref=e5]:
      - generic [ref=e6]:
        - button [ref=e7] [cursor=pointer]:
          - img [ref=e8]
        - img [ref=e12] [cursor=pointer]
        - generic [ref=e13]:
          - generic [ref=e15]:
            - generic [ref=e16]: Ticket View
            - generic [ref=e17]: "Iris (Nails) - #271"
          - generic [ref=e18]:
            - generic [ref=e20] [cursor=pointer]: Hold
            - generic [ref=e22] [cursor=pointer]: Combine
          - generic [ref=e24]:
            - generic [ref=e25]: PINK SALON
            - generic [ref=e26]: 1032 YONKERS AVE Yonkers Avenel, NJ, 07001 | (090) 123-4567
            - generic [ref=e27]: "Pos Pink | Station: 1"
    - generic [ref=e29]:
      - generic [ref=e30]:
        - img [ref=e32]
        - generic [ref=e33]:
          - generic [ref=e34]: Galaxy Pink
          - generic [ref=e35]: "2025.12"
      - generic [ref=e36]:
        - list
      - generic [ref=e37]:
        - generic [ref=e39]:
          - generic [ref=e41]: PINK SALON
          - generic [ref=e42]:
            - paragraph [ref=e44]: 1032 YONKERS AVE Yonkers Avenel, NJ, 07001
            - generic [ref=e45]: (090) 123-4567
            - generic [ref=e46]: Pos Pink
        - paragraph [ref=e47]
        - generic [ref=e48]:
          - generic [ref=e49]: BUSINESS DATE
          - generic [ref=e50]: 04/04/2026
      - paragraph [ref=e51]: © 2026 XSoftware
    - main [ref=e52]:
      - generic [ref=e53]:
        - generic [ref=e55]:
          - generic [ref=e56]:
            - button "1" [ref=e57] [cursor=pointer]:
              - generic [ref=e58]:
                - img [ref=e59]
                - generic [ref=e61]: "1"
            - generic [ref=e62]:
              - generic [ref=e64]: Select customer
              - button [ref=e65] [cursor=pointer]:
                - img [ref=e66]
          - list [ref=e73]:
            - listitem [ref=e74] [cursor=pointer]:
              - generic [ref=e75]:
                - generic [ref=e76]:
                  - generic [ref=e77]: "1"
                  - generic [ref=e78]:
                    - generic [ref=e79]:
                      - generic [ref=e80]: Taxable
                      - generic [ref=e81]:
                        - text: S x 1
                        - generic [ref=e82]: W
                    - generic [ref=e83]:
                      - generic [ref=e84]: Iris (Nails)
                      - generic [ref=e85]: Waiting Time
                - generic [ref=e87]: $16.00
          - list [ref=e89]:
            - listitem [ref=e90] [cursor=pointer]:
              - generic [ref=e91]: Tip
              - generic [ref=e92]: $0.00
            - listitem [ref=e93] [cursor=pointer]:
              - generic [ref=e94]: Tax
              - generic [ref=e95]: $0.00
            - listitem [ref=e96] [cursor=pointer]:
              - generic [ref=e97]: Discount
              - generic [ref=e98]: $0.00
            - listitem [ref=e99]:
              - generic [ref=e100]: TOTAL
              - generic [ref=e101]: $16.00
          - generic [ref=e102]:
            - button "Void Ticket" [ref=e103] [cursor=pointer]
            - button "Pay" [ref=e104] [cursor=pointer]
            - button "Cancel" [ref=e105] [cursor=pointer]
        - generic [ref=e106]:
          - button "search" [ref=e108] [cursor=pointer]:
            - img [ref=e109]
          - generic [ref=e111]:
            - tablist [ref=e116]:
              - tab "MANI & PEDI" [ref=e117] [cursor=pointer]:
                - generic [ref=e118]: MANI & PEDI
              - tab "FULL SET & FILL IN" [selected] [ref=e119] [cursor=pointer]:
                - generic [ref=e120]: FULL SET & FILL IN
              - tab "ADDITIONAL SERVICE" [ref=e121] [cursor=pointer]:
                - generic [ref=e122]: ADDITIONAL SERVICE
              - tab "GIFT CARD" [ref=e123] [cursor=pointer]:
                - generic [ref=e124]: GIFT CARD
            - tabpanel [ref=e127]:
              - list [ref=e129]:
                - listitem [ref=e130] [cursor=pointer]:
                  - generic [ref=e131]:
                    - generic [ref=e133]: F
                    - generic [ref=e134]:
                      - generic [ref=e135]: Full set
                      - generic [ref=e137]: $36.00
                      - img [ref=e139]
                - listitem [ref=e141] [cursor=pointer]:
                  - generic [ref=e142]:
                    - generic [ref=e144]: F
                    - generic [ref=e145]:
                      - generic [ref=e146]: Fill gel
                      - generic [ref=e148]: $23.50
                      - img [ref=e150]
                - listitem [ref=e152] [cursor=pointer]:
                  - generic [ref=e153]:
                    - generic [ref=e155]: G
                    - generic [ref=e156]:
                      - generic [ref=e157]: Gel polish
                      - generic [ref=e159]: $29.00
                      - img [ref=e161]
                - listitem [ref=e163] [cursor=pointer]:
                  - generic [ref=e164]:
                    - generic [ref=e166]: F
                    - generic [ref=e167]:
                      - generic [ref=e168]: French full set
                      - generic [ref=e170]: $32.00
                      - img [ref=e172]
                - listitem [ref=e174] [cursor=pointer]:
                  - generic [ref=e175]:
                    - generic [ref=e177]: T
                    - generic [ref=e178]:
                      - generic [ref=e179]: Taxable
                      - generic [ref=e181]: $16.00
                      - img [ref=e183]
  - alert [ref=e185]
```

# Test source

```ts
  107 | );
  108 | 
  109 | When('I click on the {string} button', async ({ page }, buttonText: string) => {
  110 | 	const button = page.getByRole('button', { name: buttonText, exact: true });
  111 | 	await expect(button).toBeVisible();
  112 | 
  113 | 	await button.click();
  114 | });
  115 | 
  116 | Then(
  117 | 	'I should see the text {string} visible',
  118 | 	async ({ page }, text: string) => {
  119 | 		await expect(page.getByText(text, { exact: true })).toBeVisible();
  120 | 	},
  121 | );
  122 | 
  123 | Then(
  124 | 	'I should see the button with id {string} visible',
  125 | 	async ({ page }, buttonId: string) => {
  126 | 		await expect(page.locator(`button#${buttonId}`)).toBeVisible();
  127 | 	},
  128 | );
  129 | 
  130 | When(
  131 | 	'I click on the element with id {string}',
  132 | 	async ({ page }, elementId: string) => {
  133 | 		const element = page.locator(`#${elementId}`);
  134 | 
  135 | 		await expect(element).toBeVisible();
  136 | 
  137 | 		await element.click();
  138 | 	},
  139 | );
  140 | 
  141 | Then(
  142 | 	'I should see a popup dialog with title {string}',
  143 | 	async ({ page }, dialogTitle: string) => {
  144 | 		const dialogTitleElement = page.locator('.MuiDialogTitle-root');
  145 | 
  146 | 		await expect(dialogTitleElement).toBeVisible();
  147 | 		await expect(dialogTitleElement).toHaveText(dialogTitle);
  148 | 	},
  149 | );
  150 | 
  151 | When(
  152 | 	'I select the change charge action {string}',
  153 | 	async ({ page }, action: string) => {
  154 | 		const actionElement = page
  155 | 			.locator('ul.xCharge__tax--action li')
  156 | 			.getByText(action);
  157 | 		await expect(actionElement).toHaveText(action);
  158 | 		await actionElement.click();
  159 | 	},
  160 | );
  161 | 
  162 | Then(
  163 | 	'I should see a popup dialog with content {string}',
  164 | 	async ({ page }, content: string) => {
  165 | 		const dialogContentElement = page.locator('.MuiDialogContent-root');
  166 | 
  167 | 		await expect(dialogContentElement).toBeVisible();
  168 | 		await expect(dialogContentElement).toContainText(content);
  169 | 	},
  170 | );
  171 | 
  172 | When(
  173 | 	'I click on the {string} button in the popup dialog',
  174 | 	async ({ page }, buttonText: string) => {
  175 | 		const dialog = page.locator('div[role="dialog"]');
  176 | 
  177 | 		const button = dialog.getByRole('button', {
  178 | 			name: buttonText,
  179 | 			exact: true,
  180 | 		});
  181 | 		await expect(button).toBeVisible();
  182 | 
  183 | 		await button.click();
  184 | 	},
  185 | );
  186 | 
  187 | When(
  188 | 	'I click on the {string} button in the Customer popup dialog',
  189 | 	async ({ page }, buttonText: string) => {
  190 | 		const buttonDialog = page
  191 | 			.locator('.customDialogAction')
  192 | 			.getByText(buttonText);
  193 | 
  194 | 		await expect(buttonDialog).toBeVisible();
  195 | 		await buttonDialog.click();
  196 | 	},
  197 | );
  198 | 
  199 | When('I close the popup dialog', async ({ page }) => {
  200 | 	await page.locator('button[title="Close"]').click();
  201 | });
  202 | 
  203 | Then('I should see the tax amount non-zero', async ({ page }) => {
  204 | 	const chargeTax = page.locator('.xCharge__taxes');
  205 | 
  206 | 	//await expect(chargeTax).not.toContainText('0.00');
> 207 | 	await expect(chargeTax).not.toHaveText('$0.00');
      |                              ^ Error: expect(locator).not.toHaveText(expected) failed
  208 | });
  209 | 
  210 | When(
  211 | 	'I select the {string} payment type',
  212 | 	async ({ page }, paymentType: string) => {
  213 | 		const paymentTypeButton = page
  214 | 			.locator('.paymentType')
  215 | 			.getByText(paymentType, { exact: true });
  216 | 		await expect(paymentTypeButton).toBeVisible();
  217 | 
  218 | 		await paymentTypeButton.click();
  219 | 	},
  220 | );
  221 | 
  222 | When(
  223 | 	'I select the {string} payment type on the payment ticket dialog',
  224 | 	async ({ page }, paymentType: string) => {
  225 | 		const paymentTypeButton = page
  226 | 			.locator('ul.xPayment__type li')
  227 | 			.getByText(paymentType, { exact: true });
  228 | 		await expect(paymentTypeButton).toBeVisible();
  229 | 
  230 | 		await paymentTypeButton.click();
  231 | 	},
  232 | );
  233 | 
  234 | When('I click on the item {string} button', async ({ page }, item: string) => {
  235 | 	const itemButton = page.locator('.xMultiple').getByText(item);
  236 | 	await expect(itemButton).toBeVisible();
  237 | 
  238 | 	await itemButton.click();
  239 | });
  240 | 
  241 | When(
  242 | 	'I select the {string} service in the dialog',
  243 | 	async ({ page }, service: string) => {
  244 | 		const serviceButton = page
  245 | 			.locator('div.xMultiple__wrap')
  246 | 			.locator('li.xTicketItems')
  247 | 			.getByText(service, { exact: true });
  248 | 		await expect(serviceButton).toBeVisible();
  249 | 
  250 | 		await serviceButton.click();
  251 | 	},
  252 | );
  253 | 
  254 | When(
  255 | 	'I select the {string} employee in the dialog',
  256 | 	async ({ page }, employee: string) => {
  257 | 		const employeeButton = page
  258 | 			.locator('.xEmployeeItem')
  259 | 			.getByText(employee, { exact: true });
  260 | 		await expect(employeeButton).toBeVisible();
  261 | 
  262 | 		await employeeButton.click();
  263 | 	},
  264 | );
  265 | 
  266 | When(
  267 | 	'I click on the {string} button in the dialog',
  268 | 	async ({ page }, button: string) => {
  269 | 		const buttonElement = page
  270 | 			.locator('.xMultiple__wrap')
  271 | 			.getByRole('button', { name: button });
  272 | 
  273 | 		await expect(buttonElement).toBeVisible();
  274 | 
  275 | 		await buttonElement.click();
  276 | 	},
  277 | );
  278 | 
  279 | Then(
  280 | 	'I should see the {string} employee in my cart',
  281 | 	async ({ page }, employee: string) => {
  282 | 		const employeeElement = page
  283 | 			.locator('.xTicketItems__wrap')
  284 | 			.getByText(employee);
  285 | 		await expect(employeeElement).toContainText(employee);
  286 | 	},
  287 | );
  288 | 
  289 | Then(
  290 | 	'I should see multiple {string} employees in my cart',
  291 | 	async ({ page }, employee: string) => {
  292 | 		const employeeElements = await page
  293 | 			.locator('li.xTicketItems')
  294 | 			.getByText(employee)
  295 | 			.all();
  296 | 
  297 | 		expect(employeeElements.length).toBeGreaterThan(1);
  298 | 	},
  299 | );
  300 | 
  301 | Then(
  302 | 	'I should see multiple {string} technicians in the waiting list',
  303 | 	async ({ page }, technician: string) => {
  304 | 		const technicianElements = await page
  305 | 			.locator('div[data-field="technicianNickNames"]')
  306 | 			.getByText(technician, { exact: true })
  307 | 			.all();
```