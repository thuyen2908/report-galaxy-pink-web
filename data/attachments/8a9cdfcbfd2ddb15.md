# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: create-tickets.feature.spec.js >> Create tickets >> In Service - show Service Count, Price Service Ticket
- Location: dist/bdd/create-tickets.feature.spec.js:889:3

# Error details

```
Test timeout of 90000ms exceeded.
```

```
Error: locator.click: Test timeout of 90000ms exceeded.
Call log:
  - waiting for locator('.xBtn').getByText('Hold')
    - locator resolved to <span>Hold</span>
  - attempting click action
    2 × waiting for element to be visible, enabled and stable
      - element is visible, enabled and stable
      - scrolling into view if needed
      - done scrolling
      - <div tabindex="-1" role="presentation" class="MuiDialog-container MuiDialog-scrollPaper css-16u656j">…</div> from <div role="presentation" class="MuiDialog-root MuiModal-root css-93w38h">…</div> subtree intercepts pointer events
    - retrying click action
    - waiting 20ms
    2 × waiting for element to be visible, enabled and stable
      - element is visible, enabled and stable
      - scrolling into view if needed
      - done scrolling
      - <div tabindex="-1" role="presentation" class="MuiDialog-container MuiDialog-scrollPaper css-16u656j">…</div> from <div role="presentation" class="MuiDialog-root MuiModal-root css-93w38h">…</div> subtree intercepts pointer events
    - retrying click action
      - waiting 100ms
    143 × waiting for element to be visible, enabled and stable
        - element is visible, enabled and stable
        - scrolling into view if needed
        - done scrolling
        - <div tabindex="-1" role="presentation" class="MuiDialog-container MuiDialog-scrollPaper css-16u656j">…</div> from <div role="presentation" class="MuiDialog-root MuiModal-root css-93w38h">…</div> subtree intercepts pointer events
      - retrying click action
        - waiting 500ms

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
          - generic [ref=e15]:
            - generic [ref=e16]: Ticket View
            - generic [ref=e17]: "Daria (Nails) - #102"
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
          - generic [ref=e50]: 06/08/2026
      - paragraph [ref=e51]: © 2026 XSoftware
    - main [ref=e52]:
      - generic [ref=e53]:
        - generic [ref=e55]:
          - generic [ref=e56]:
            - button [ref=e57] [cursor=pointer]:
              - generic [ref=e58]:
                - img [ref=e59]
                - generic [ref=e61]: "3"
            - generic [ref=e62]:
              - generic [ref=e64] [cursor=pointer]:
                - generic [ref=e65]: InService
                - generic [ref=e66]: 590 = $5.90
              - button [ref=e67] [cursor=pointer]:
                - img [ref=e68]
          - list [ref=e76]:
            - listitem [ref=e77] [cursor=pointer]:
              - generic [ref=e78]:
                - generic [ref=e79]:
                  - generic [ref=e80]: "1"
                  - generic [ref=e81]:
                    - generic [ref=e82]:
                      - generic [ref=e83]: Combo 1
                      - generic [ref=e84]:
                        - text: SP x 1
                        - generic [ref=e85]: W
                    - generic [ref=e86]:
                      - generic [ref=e87]: Daria (Nails)
                      - generic [ref=e88]: Waiting Time
                - generic [ref=e90]: $45.00
              - list [ref=e91]:
                - listitem [ref=e92]:
                  - generic [ref=e95]:
                    - generic [ref=e96]:
                      - generic [ref=e97]: Manicure
                      - generic [ref=e98]:
                        - text: S x 1
                        - generic [ref=e99]: W
                    - generic [ref=e100]:
                      - generic [ref=e101]: Daria (Nails)
                      - generic [ref=e102]: Waiting Time
                - listitem [ref=e103]:
                  - generic [ref=e106]:
                    - generic [ref=e107]:
                      - generic [ref=e108]: Pedicure
                      - generic [ref=e109]:
                        - text: S x 1
                        - generic [ref=e110]: W
                    - generic [ref=e111]:
                      - generic [ref=e112]: Daria (Nails)
                      - generic [ref=e113]: Waiting Time
            - listitem [ref=e114] [cursor=pointer]:
              - generic [ref=e115]:
                - generic [ref=e116]:
                  - generic [ref=e117]: "2"
                  - generic [ref=e118]:
                    - generic [ref=e119]:
                      - generic [ref=e120]: Manicure
                      - generic [ref=e121]:
                        - text: S x 1
                        - generic [ref=e122]: W
                    - generic [ref=e123]:
                      - generic [ref=e124]: Daria (Nails)
                      - generic [ref=e125]: Waiting Time
                - generic [ref=e127]: $6.00
            - listitem [ref=e128] [cursor=pointer]:
              - generic [ref=e129]:
                - generic [ref=e130]:
                  - generic [ref=e131]: "3"
                  - generic [ref=e132]:
                    - generic [ref=e133]:
                      - generic [ref=e134]: Pedicure
                      - generic [ref=e135]:
                        - text: S x 1
                        - generic [ref=e136]: W
                    - generic [ref=e137]:
                      - generic [ref=e138]: Daria (Nails)
                      - generic [ref=e139]: Waiting Time
                - generic [ref=e141]: $8.00
          - list [ref=e143]:
            - listitem [ref=e144] [cursor=pointer]:
              - generic [ref=e145]: Tip
              - generic [ref=e146]: $0.00
            - listitem [ref=e147] [cursor=pointer]:
              - generic [ref=e148]: Tax
              - generic [ref=e149]: $0.00
            - listitem [ref=e150] [cursor=pointer]:
              - generic [ref=e151]: Discount
              - generic [ref=e152]: $0.00
            - listitem [ref=e153]:
              - generic [ref=e154]: TOTAL
              - generic [ref=e155]: $59.00
          - generic [ref=e156]:
            - button [ref=e157] [cursor=pointer]: Void Ticket
            - button [ref=e158] [cursor=pointer]: Pay
            - button [ref=e159] [cursor=pointer]: Cancel
        - generic [ref=e160]:
          - button [ref=e162] [cursor=pointer]:
            - img [ref=e163]
          - generic [ref=e165]:
            - tablist [ref=e170]:
              - tab [selected] [ref=e171] [cursor=pointer]:
                - generic [ref=e172]: MANI & PEDI
              - tab [ref=e173] [cursor=pointer]:
                - generic [ref=e174]: FULL SET & FILL IN
              - tab [ref=e175] [cursor=pointer]:
                - generic [ref=e176]: ADDITIONAL SERVICE
              - tab [ref=e177] [cursor=pointer]:
                - generic [ref=e178]: GIFT CARD
            - tabpanel [ref=e181]:
              - list [ref=e183]:
                - listitem [ref=e184] [cursor=pointer]:
                  - generic [ref=e185]:
                    - generic [ref=e187]: M
                    - generic [ref=e188]:
                      - generic [ref=e189]: Manicure
                      - generic [ref=e191]: $6.00
                      - img [ref=e193]
                - listitem [ref=e195] [cursor=pointer]:
                  - generic [ref=e196]:
                    - generic [ref=e198]: P
                    - generic [ref=e199]:
                      - generic [ref=e200]: Pedicure
                      - generic [ref=e202]: $8.00
                      - img [ref=e204]
                - listitem [ref=e206] [cursor=pointer]:
                  - generic [ref=e207]:
                    - generic [ref=e209]: C
                    - generic [ref=e210]:
                      - generic [ref=e211]: Cut cuticle
                      - generic [ref=e213]: $10.00
                      - img [ref=e215]
                - listitem [ref=e217] [cursor=pointer]:
                  - generic [ref=e218]:
                    - generic [ref=e220]: G
                    - generic [ref=e221]:
                      - generic [ref=e222]: Gel removal
                      - generic [ref=e224]: $40.00
                      - img [ref=e226]
                - listitem [ref=e228] [cursor=pointer]:
                  - generic [ref=e229]:
                    - generic [ref=e231]: A
                    - generic [ref=e232]:
                      - generic [ref=e233]: Acrylic removal
                      - generic [ref=e235]: $30.00
                      - img [ref=e237]
                - listitem [ref=e239] [cursor=pointer]:
                  - generic [ref=e240]:
                    - generic [ref=e242]: G
                    - generic [ref=e243]:
                      - generic [ref=e244]: Gel X
                      - generic [ref=e246]: $27.00
                      - img [ref=e248]
                - listitem [ref=e250] [cursor=pointer]:
                  - generic [ref=e251]:
                    - generic [ref=e253]: R
                    - generic [ref=e254]:
                      - generic [ref=e255]: Request price
                      - generic [ref=e257]: $0.00
                      - img [ref=e259]
                - listitem [ref=e261] [cursor=pointer]:
                  - generic [ref=e262]:
                    - generic [ref=e264]: C
                    - generic [ref=e265]:
                      - generic [ref=e266]: Combo 1
                      - generic [ref=e268]: $45.00
                      - img [ref=e270]
                - listitem [ref=e272] [cursor=pointer]:
                  - generic [ref=e273]:
                    - generic [ref=e275]: C
                    - generic [ref=e276]:
                      - generic [ref=e277]: Combo 2
                      - generic [ref=e279]: $60.00
                      - img [ref=e281]
                - listitem [ref=e283] [cursor=pointer]:
                  - generic [ref=e284]:
                    - generic [ref=e286]: S
                    - generic [ref=e287]:
                      - generic [ref=e288]: Supper combo
                      - generic [ref=e290]: $0.00
                      - img [ref=e292]
  - alert [ref=e294]
  - dialog "Reward close" [ref=e297]:
    - heading "Reward close" [level=2] [ref=e298]:
      - text: Reward
      - button "close" [ref=e300] [cursor=pointer]:
        - img [ref=e301]
    - separator [ref=e303]
    - generic [ref=e304]:
      - paragraph [ref=e307]:
        - text: Customer is eligible for a reward.
        - text: Do you want to redeem now?
      - generic [ref=e309]:
        - button "CANCEL" [ref=e310] [cursor=pointer]
        - button "OK" [ref=e311] [cursor=pointer]
```

# Test source

```ts
  1105 | 	await discountElement.click();
  1106 | });
  1107 | 
  1108 | When('I select the type {string} option', async ({ page }, type: string) => {
  1109 | 	const typeElement = page.locator('.xFlex-select');
  1110 | 	await typeElement.click();
  1111 | 	await page.locator('#menu-typeDiscount').getByText(type).click();
  1112 | });
  1113 | 
  1114 | Then(
  1115 | 	'I should see the discount type {string} visible',
  1116 | 	async ({ page }, type: string) => {
  1117 | 		const discountTypeElement = page
  1118 | 			.locator('.MuiListItemText-primary')
  1119 | 			.first()
  1120 | 			.getByText(type);
  1121 | 		await expect(discountTypeElement).toHaveText(type);
  1122 | 	},
  1123 | );
  1124 | 
  1125 | When(
  1126 | 	'I enter the discount amount {string}',
  1127 | 	async ({ page }, amount: string) => {
  1128 | 		await page.locator('input#priceAmount').fill(amount);
  1129 | 	},
  1130 | );
  1131 | 
  1132 | Then(
  1133 | 	'I should see the {string} discount in my cart',
  1134 | 	async ({ page }, discount: string) => {
  1135 | 		const discountElement = page
  1136 | 			.locator('.xTicketItems__discount--title')
  1137 | 			.getByText(discount);
  1138 | 		await expect(discountElement).toContainText(discount);
  1139 | 	},
  1140 | );
  1141 | 
  1142 | Then(
  1143 | 	'I should see the discount ticket detail {string} in my cart',
  1144 | 	async ({ page }, discount: string) => {
  1145 | 		const discountElement = page.locator('.TicketDiscount');
  1146 | 		await expect(discountElement).toContainText(discount);
  1147 | 	},
  1148 | );
  1149 | 
  1150 | Then('I should see {string} in my cart', async ({ page }, charge: string) => {
  1151 | 	const parenIndex = charge.indexOf('(');
  1152 | 	const dollarIndex = charge.indexOf('$');
  1153 | 
  1154 | 	let label = charge;
  1155 | 	let amount: string | undefined;
  1156 | 
  1157 | 	if (parenIndex > 0 && charge.includes(')', parenIndex)) {
  1158 | 		label = charge.slice(0, parenIndex).trim();
  1159 | 		amount = charge.slice(parenIndex).trim();
  1160 | 	} else if (dollarIndex > 0) {
  1161 | 		label = charge.slice(0, dollarIndex).trim();
  1162 | 		amount = charge.slice(dollarIndex).trim();
  1163 | 	}
  1164 | 
  1165 | 	const chargeItem = page
  1166 | 		.locator('ul.xCharge li')
  1167 | 		.filter({ has: page.locator('span', { hasText: label }) });
  1168 | 
  1169 | 	await expect(chargeItem).toBeVisible();
  1170 | 	await expect(chargeItem.locator('span').first()).toHaveText(label);
  1171 | 
  1172 | 	if (amount) {
  1173 | 		await expect(chargeItem.locator('span').nth(1)).toContainText(amount);
  1174 | 	} else {
  1175 | 		await expect(chargeItem).toContainText(charge);
  1176 | 	}
  1177 | });
  1178 | 
  1179 | Then(
  1180 | 	'I should see the {string} absorption type in my cart',
  1181 | 	async ({ page }, type: string) => {
  1182 | 		const typeElement = page
  1183 | 			.locator('.xTicketItems__discount--title')
  1184 | 			.getByText(type);
  1185 | 		await expect(typeElement).toContainText(type);
  1186 | 	},
  1187 | );
  1188 | 
  1189 | When(
  1190 | 	'I select the discount absorb type {string}',
  1191 | 	async ({ page }, type: string) => {
  1192 | 		const typeElement = page
  1193 | 			.locator('ul.listDiscount__commission li')
  1194 | 			.getByText(type);
  1195 | 		await expect(typeElement).toHaveText(type);
  1196 | 		await typeElement.click();
  1197 | 	},
  1198 | );
  1199 | 
  1200 | When(
  1201 | 	'I click on the {string} button on the header',
  1202 | 	async ({ page }, button: string) => {
  1203 | 		const buttonElement = page.locator('.xBtn').getByText(button);
  1204 | 		await expect(buttonElement).toHaveText(button);
> 1205 | 		await buttonElement.click();
       |                       ^ Error: locator.click: Test timeout of 90000ms exceeded.
  1206 | 	},
  1207 | );
  1208 | 
  1209 | Then(
  1210 | 	'I should see discount {string} in my cart',
  1211 | 	async ({ page }, amount: string) => {
  1212 | 		const amountDiscount = page
  1213 | 			.locator('.xTicketItems__discount--price')
  1214 | 			.getByText(amount);
  1215 | 		await expect(amountDiscount).toContainText(amount);
  1216 | 	},
  1217 | );
  1218 | 
  1219 | When(
  1220 | 	'I enter the discount percent {string}',
  1221 | 	async ({ page }, percent: string) => {
  1222 | 		await page.locator('#pricePercent').fill(percent);
  1223 | 	},
  1224 | );
  1225 | 
  1226 | Then('I should see the discount ticket non-zero', async ({ page }) => {
  1227 | 	const discountTicket = page.locator('ul.xCharge li.MuiListItem-root').nth(1);
  1228 | 
  1229 | 	await expect(discountTicket).not.toContainText('0.00');
  1230 | 	await expect(discountTicket).not.toHaveText('$0.00');
  1231 | });
  1232 | 
  1233 | Then(
  1234 | 	'I should see the {string} category',
  1235 | 	async ({ page }, category: string) => {
  1236 | 		const categoryElement = page
  1237 | 			.locator('button.MuiButtonBase-root')
  1238 | 			.getByText(category, { exact: true });
  1239 | 		await expect(categoryElement).toHaveText(category);
  1240 | 	},
  1241 | );
  1242 | 
  1243 | When('I select the {string} category', async ({ page }, category: string) => {
  1244 | 	const categoryElement = page
  1245 | 		.locator('button.MuiButtonBase-root')
  1246 | 		.getByText(category, { exact: true });
  1247 | 	await expect(categoryElement).toHaveText(category);
  1248 | 	await categoryElement.click();
  1249 | });
  1250 | 
  1251 | Then(
  1252 | 	'I should see the number card {string} visible',
  1253 | 	async ({ page }, number: string) => {
  1254 | 		const numberElement = page.locator('.numberCard').getByText(number);
  1255 | 		await expect(numberElement).toHaveText(number);
  1256 | 	},
  1257 | );
  1258 | // tax steps ticket adjustment
  1259 | When('I {string} in ticket', async ({ page }, actionTax: string) => {
  1260 | 	const taxButton = page.locator('.xCharge__taxes');
  1261 | 	await expect(taxButton).toBeVisible();
  1262 | 	await taxButton.click();
  1263 | 	const popup = page.locator('[aria-labelledby="alert-dialog-title"]');
  1264 | 	await expect(popup).toBeVisible();
  1265 | 	const option = popup.locator(`text=${actionTax}`);
  1266 | 	await expect(option).toBeVisible();
  1267 | 	await option.click();
  1268 | });
  1269 | 
  1270 | Then('I should see the tax display {string}', async ({ page }, tax: string) => {
  1271 | 	const taxAmount = page.locator('.xCharge__taxes');
  1272 | 	await expect(taxAmount).toHaveText(tax);
  1273 | });
  1274 | 
  1275 | When('I select the reason {string}', async ({ page }, reason: string) => {
  1276 | 	const reasonElement = page
  1277 | 		.locator('.xVoid')
  1278 | 		.getByText(reason, { exact: true });
  1279 | 	await expect(reasonElement).toHaveText(reason);
  1280 | 	await reasonElement.click();
  1281 | });
  1282 | 
  1283 | Then(
  1284 | 	'I should see a second popup dialog with title {string}',
  1285 | 	async ({ page }, dialogTitle: string) => {
  1286 | 		const dialogTitleElement = page.locator('.MuiDialogTitle-root').last();
  1287 | 
  1288 | 		await expect(dialogTitleElement).toBeVisible();
  1289 | 		await expect(dialogTitleElement).toHaveText(dialogTitle);
  1290 | 	},
  1291 | );
  1292 | 
  1293 | When('I back to HOME page', async ({ page }) => {
  1294 | 	await page.locator('.xHeader__top--left').click();
  1295 | });
  1296 | 
  1297 | Then(
  1298 | 	'I should see the employee {string} in my cart',
  1299 | 	async ({ page }, employee: string) => {
  1300 | 		const employeeElement = page
  1301 | 			.locator('.xTicketItems__wrap')
  1302 | 			.getByText(employee);
  1303 | 		await expect(employeeElement).toContainText(employee);
  1304 | 	},
  1305 | );
```