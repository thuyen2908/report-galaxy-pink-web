# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: create-tickets.feature.spec.js >> Create tickets >> Remove tax in ticket
- Location: dist/bdd/create-tickets.feature.spec.js:443:3

# Error details

```
Error: expect(locator).toContainText(expected) failed

Locator: locator('ul.xCharge li').filter({ has: locator('span').filter({ hasText: 'Tax' }) }).locator('span').nth(1)
Expected substring: "$0.96"
Received string:    "$0.00"
Timeout: 30000ms

Call log:
  - Expect "toContainText" with timeout 30000ms
  - waiting for locator('ul.xCharge li').filter({ has: locator('span').filter({ hasText: 'Tax' }) }).locator('span').nth(1)
    33 × locator resolved to <span class="xCharge__taxes">$0.00</span>
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
            - generic [ref=e17]: "Jack (Nails) - #203"
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
                      - generic [ref=e84]: Jack (Nails)
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
  1045 | 	const discountElement = page
  1046 | 		.locator('ul.xTicketFunctions__type li')
  1047 | 		.getByText(type);
  1048 | 	await expect(discountElement).toHaveText(type);
  1049 | 	await discountElement.click();
  1050 | });
  1051 | 
  1052 | Then('I should see the discount sorted correctly', async ({ page }) => {
  1053 | 	const discountItems = page.locator('.listDiscount__item ul li p');
  1054 | 	const count = await discountItems.count();
  1055 | 
  1056 | 	const texts: string[] = [];
  1057 | 
  1058 | 	for (let i = 0; i < count; i++) {
  1059 | 		texts.push((await discountItems.nth(i).innerText()).trim());
  1060 | 	}
  1061 | 	const expectedOrder = [
  1062 | 		'Open Discount',
  1063 | 		'$5 Off',
  1064 | 		'5% Off',
  1065 | 		'10% Off',
  1066 | 		'20% Off - exclude Product',
  1067 | 	];
  1068 | 
  1069 | 	await expect(texts).toEqual(expectedOrder);
  1070 | });
  1071 | 
  1072 | When('I select the discount {string}', async ({ page }, discount: string) => {
  1073 | 	const discountElement = page
  1074 | 		.locator('.MuiListItem-gutters')
  1075 | 		.getByText(discount, { exact: true });
  1076 | 	await expect(discountElement).toHaveText(discount);
  1077 | 	await discountElement.click();
  1078 | });
  1079 | 
  1080 | When('I select the type {string} option', async ({ page }, type: string) => {
  1081 | 	const typeElement = page.locator('.xFlex-select');
  1082 | 	await typeElement.click();
  1083 | 	await page.locator('#menu-typeDiscount').getByText(type).click();
  1084 | });
  1085 | 
  1086 | Then(
  1087 | 	'I should see the discount type {string} visible',
  1088 | 	async ({ page }, type: string) => {
  1089 | 		const discountTypeElement = page
  1090 | 			.locator('.MuiListItemText-primary')
  1091 | 			.first()
  1092 | 			.getByText(type);
  1093 | 		await expect(discountTypeElement).toHaveText(type);
  1094 | 	},
  1095 | );
  1096 | 
  1097 | When(
  1098 | 	'I enter the discount amount {string}',
  1099 | 	async ({ page }, amount: string) => {
  1100 | 		await page.locator('input#priceAmount').fill(amount);
  1101 | 	},
  1102 | );
  1103 | 
  1104 | Then(
  1105 | 	'I should see the {string} discount in my cart',
  1106 | 	async ({ page }, discount: string) => {
  1107 | 		const discountElement = page
  1108 | 			.locator('.xTicketItems__discount--title')
  1109 | 			.getByText(discount);
  1110 | 		await expect(discountElement).toContainText(discount);
  1111 | 	},
  1112 | );
  1113 | 
  1114 | Then(
  1115 | 	'I should see the discount ticket detail {string} in my cart',
  1116 | 	async ({ page }, discount: string) => {
  1117 | 		const discountElement = page.locator('.TicketDiscount');
  1118 | 		await expect(discountElement).toContainText(discount);
  1119 | 	},
  1120 | );
  1121 | 
  1122 | Then('I should see {string} in my cart', async ({ page }, charge: string) => {
  1123 | 	const parenIndex = charge.indexOf('(');
  1124 | 	const dollarIndex = charge.indexOf('$');
  1125 | 
  1126 | 	let label = charge;
  1127 | 	let amount: string | undefined;
  1128 | 
  1129 | 	if (parenIndex > 0 && charge.includes(')', parenIndex)) {
  1130 | 		label = charge.slice(0, parenIndex).trim();
  1131 | 		amount = charge.slice(parenIndex).trim();
  1132 | 	} else if (dollarIndex > 0) {
  1133 | 		label = charge.slice(0, dollarIndex).trim();
  1134 | 		amount = charge.slice(dollarIndex).trim();
  1135 | 	}
  1136 | 
  1137 | 	const chargeItem = page
  1138 | 		.locator('ul.xCharge li')
  1139 | 		.filter({ has: page.locator('span', { hasText: label }) });
  1140 | 
  1141 | 	await expect(chargeItem).toBeVisible();
  1142 | 	await expect(chargeItem.locator('span').first()).toHaveText(label);
  1143 | 
  1144 | 	if (amount) {
> 1145 | 		await expect(chargeItem.locator('span').nth(1)).toContainText(amount);
       |                                                   ^ Error: expect(locator).toContainText(expected) failed
  1146 | 	} else {
  1147 | 		await expect(chargeItem).toContainText(charge);
  1148 | 	}
  1149 | });
  1150 | 
  1151 | Then(
  1152 | 	'I should see the {string} absorption type in my cart',
  1153 | 	async ({ page }, type: string) => {
  1154 | 		const typeElement = page
  1155 | 			.locator('.xTicketItems__discount--title')
  1156 | 			.getByText(type);
  1157 | 		await expect(typeElement).toContainText(type);
  1158 | 	},
  1159 | );
  1160 | 
  1161 | When(
  1162 | 	'I select the discount absorb type {string}',
  1163 | 	async ({ page }, type: string) => {
  1164 | 		const typeElement = page
  1165 | 			.locator('ul.listDiscount__commission li')
  1166 | 			.getByText(type);
  1167 | 		await expect(typeElement).toHaveText(type);
  1168 | 		await typeElement.click();
  1169 | 	},
  1170 | );
  1171 | 
  1172 | When(
  1173 | 	'I click on the {string} button on the header',
  1174 | 	async ({ page }, button: string) => {
  1175 | 		const buttonElement = page.locator('.xBtn').getByText(button);
  1176 | 		await expect(buttonElement).toHaveText(button);
  1177 | 		await buttonElement.click();
  1178 | 	},
  1179 | );
  1180 | 
  1181 | Then(
  1182 | 	'I should see discount {string} in my cart',
  1183 | 	async ({ page }, amount: string) => {
  1184 | 		const amountDiscount = page
  1185 | 			.locator('.xTicketItems__discount--price')
  1186 | 			.getByText(amount);
  1187 | 		await expect(amountDiscount).toContainText(amount);
  1188 | 	},
  1189 | );
  1190 | 
  1191 | When(
  1192 | 	'I enter the discount percent {string}',
  1193 | 	async ({ page }, percent: string) => {
  1194 | 		await page.locator('#pricePercent').fill(percent);
  1195 | 	},
  1196 | );
  1197 | 
  1198 | Then('I should see the discount ticket non-zero', async ({ page }) => {
  1199 | 	const discountTicket = page.locator('ul.xCharge li.MuiListItem-root').nth(1);
  1200 | 
  1201 | 	await expect(discountTicket).not.toContainText('0.00');
  1202 | 	await expect(discountTicket).not.toHaveText('$0.00');
  1203 | });
  1204 | 
  1205 | Then(
  1206 | 	'I should see the {string} category',
  1207 | 	async ({ page }, category: string) => {
  1208 | 		const categoryElement = page
  1209 | 			.locator('button.MuiButtonBase-root')
  1210 | 			.getByText(category, { exact: true });
  1211 | 		await expect(categoryElement).toHaveText(category);
  1212 | 	},
  1213 | );
  1214 | 
  1215 | When('I select the {string} category', async ({ page }, category: string) => {
  1216 | 	const categoryElement = page
  1217 | 		.locator('button.MuiButtonBase-root')
  1218 | 		.getByText(category, { exact: true });
  1219 | 	await expect(categoryElement).toHaveText(category);
  1220 | 	await categoryElement.click();
  1221 | });
  1222 | 
  1223 | Then(
  1224 | 	'I should see the number card {string} visible',
  1225 | 	async ({ page }, number: string) => {
  1226 | 		const numberElement = page.locator('.numberCard').getByText(number);
  1227 | 		await expect(numberElement).toHaveText(number);
  1228 | 	},
  1229 | );
  1230 | // tax steps ticket adjustment
  1231 | When('I {string} in ticket', async ({ page }, actionTax: string) => {
  1232 | 	const taxButton = page.locator('.xCharge__taxes');
  1233 | 	await expect(taxButton).toBeVisible();
  1234 | 	await taxButton.click();
  1235 | 	const popup = page.locator('[aria-labelledby="alert-dialog-title"]');
  1236 | 	await expect(popup).toBeVisible();
  1237 | 	const option = popup.locator(`text=${actionTax}`);
  1238 | 	await expect(option).toBeVisible();
  1239 | 	await option.click();
  1240 | });
  1241 | 
  1242 | Then('I should see the tax display {string}', async ({ page }, tax: string) => {
  1243 | 	const taxAmount = page.locator('.xCharge__taxes');
  1244 | 	await expect(taxAmount).toHaveText(tax);
  1245 | });
```