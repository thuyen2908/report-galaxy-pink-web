# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: turn-details.feature.spec.js >> Turn details >> Turn update when voiding a ticket
- Location: dist/bdd/turn-details.feature.spec.js:17:3

# Error details

```
Error: expect(locator).toHaveText(expected) failed

Locator:  locator('ul.ListItemEmployee__wrap').first().locator('li.xEmployeeItem').filter({ hasText: 'Jessica' }).locator('div.xEmployeeItem__time').locator('span.MuiChip-label').first()
Expected: "C = 0.0"
Received: "T = 0.00"
Timeout:  30000ms

Call log:
  - Expect "toHaveText" with timeout 30000ms
  - waiting for locator('ul.ListItemEmployee__wrap').first().locator('li.xEmployeeItem').filter({ hasText: 'Jessica' }).locator('div.xEmployeeItem__time').locator('span.MuiChip-label').first()
    33 × locator resolved to <span class="MuiChip-label MuiChip-labelSmall css-tavflp">T = 0.00</span>
       - unexpected value "T = 0.00"

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
          - generic [ref=e14]:
            - generic [ref=e15]:
              - generic [ref=e16]: FUNCTIONS
              - generic [ref=e17]:
                - generic [ref=e18]:
                  - generic [ref=e19]:
                    - generic [ref=e20]: "07"
                    - generic [ref=e21]: ":"
                    - generic [ref=e22]: "20"
                    - generic [ref=e23]: ":"
                    - generic [ref=e24]: "07"
                  - generic [ref=e25]: AM
                - generic [ref=e26]: 04/04/2026
            - generic [ref=e27]:
              - listitem [ref=e28] [cursor=pointer]:
                - generic [ref=e29]: Balance
              - separator [ref=e30]
              - listitem [ref=e31] [cursor=pointer]:
                - generic [ref=e32]: WAIT
              - separator [ref=e33]
              - listitem [ref=e34] [cursor=pointer]:
                - generic [ref=e35]: APPT BOOK
              - separator [ref=e36]
              - listitem [ref=e37] [cursor=pointer]:
                - generic [ref=e38]: FAST SALE
          - img [ref=e41]
          - generic [ref=e44]:
            - generic [ref=e45]: PINK SALON
            - generic [ref=e46]: 1032 YONKERS AVE Yonkers Avenel, NJ, 07001 | (090) 123-4567
            - generic [ref=e47]: "Pos Pink | Station: 1"
    - generic [ref=e49]:
      - generic [ref=e50]:
        - img [ref=e52]
        - generic [ref=e53]:
          - generic [ref=e54]: Galaxy Pink
          - generic [ref=e55]: "2025.12"
      - generic [ref=e56]:
        - list
      - generic [ref=e57]:
        - generic [ref=e59]:
          - generic [ref=e61]: PINK SALON
          - generic [ref=e62]:
            - paragraph [ref=e64]: 1032 YONKERS AVE Yonkers Avenel, NJ, 07001
            - generic [ref=e65]: (090) 123-4567
            - generic [ref=e66]: Pos Pink
        - paragraph [ref=e67]
        - generic [ref=e68]:
          - generic [ref=e69]: BUSINESS DATE
          - generic [ref=e70]: 04/04/2026
      - paragraph [ref=e71]: © 2026 XSoftware
    - main [ref=e72]:
      - generic [ref=e73]:
        - generic [ref=e74]:
          - generic [ref=e75]:
            - tablist [ref=e80]:
              - tab "NAILS" [ref=e81] [cursor=pointer]:
                - generic [ref=e82]: NAILS
              - tab "HAIR" [active] [selected] [ref=e83] [cursor=pointer]:
                - generic [ref=e84]: HAIR
            - tabpanel [ref=e87]:
              - list [ref=e88]:
                - listitem [ref=e89] [cursor=pointer]:
                  - img [ref=e90]
                - listitem [ref=e93] [cursor=pointer]:
                  - img [ref=e94]
              - list [ref=e99]:
                - listitem [ref=e100] [cursor=pointer]:
                  - generic [ref=e102]:
                    - generic [ref=e104]: A
                    - generic [ref=e106]:
                      - generic [ref=e107]: "#1"
                      - generic [ref=e108]: Anna
                  - generic [ref=e110]:
                    - img [ref=e111]
                    - generic [ref=e115]: 12:00:00 AM
                  - generic [ref=e117]:
                    - generic [ref=e119]: T = 0.00
                    - generic [ref=e121]: C = 0.0
                    - generic [ref=e123]: L = 0.00
                    - generic [ref=e125]: 12:00 AM
                - listitem [ref=e126] [cursor=pointer]:
                  - generic [ref=e128]:
                    - generic [ref=e130]: J
                    - generic [ref=e132]:
                      - generic [ref=e133]: "#2"
                      - generic [ref=e134]: Jessica
                  - generic [ref=e136]:
                    - img [ref=e137]
                    - generic [ref=e141]: 12:00:00 AM
                  - generic [ref=e143]:
                    - generic [ref=e145]: T = 0.00
                    - generic [ref=e147]: C = 0.0
                    - generic [ref=e149]: L = 0.00
                    - generic [ref=e151]: 12:00 AM
                - listitem [ref=e152] [cursor=pointer]:
                  - generic [ref=e154]:
                    - generic [ref=e156]: T
                    - generic [ref=e158]:
                      - generic [ref=e159]: "#3"
                      - generic [ref=e160]: TurnDetail
                  - generic [ref=e162]:
                    - img [ref=e163]
                    - generic [ref=e167]: 05:54:57 AM
                  - generic [ref=e169]:
                    - generic [ref=e171]: T = 0.00
                    - generic [ref=e173]: C = 0.0
                    - generic [ref=e175]: L = 0.00
                    - generic [ref=e177]: 05:54 AM
                - listitem [ref=e178] [cursor=pointer]:
                  - generic [ref=e180]:
                    - generic [ref=e182]: A
                    - generic [ref=e184]:
                      - generic [ref=e185]: "#4"
                      - generic [ref=e186]: Avery
                  - generic [ref=e188]:
                    - img [ref=e189]
                    - generic [ref=e193]: 07:00:00 AM
                  - generic [ref=e195]:
                    - generic [ref=e197]: T = 0.00
                    - generic [ref=e199]: C = 0.0
                    - generic [ref=e201]: L = 0.00
                    - generic [ref=e203]: 07:00 AM
                - listitem [ref=e204] [cursor=pointer]:
                  - generic [ref=e206]:
                    - generic [ref=e208]: E
                    - generic [ref=e210]:
                      - generic [ref=e211]: "#5"
                      - generic [ref=e212]: Emily
                  - generic [ref=e214]:
                    - img [ref=e215]
                    - generic [ref=e219]: 07:00:00 AM
                  - generic [ref=e221]:
                    - generic [ref=e223]: T = 0.00
                    - generic [ref=e225]: C = 0.0
                    - generic [ref=e227]: L = 0.00
                    - generic [ref=e229]: 07:00 AM
                - listitem [ref=e230] [cursor=pointer]:
                  - generic [ref=e232]:
                    - generic [ref=e234]: A
                    - generic [ref=e236]:
                      - generic [ref=e237]: "#6"
                      - generic [ref=e238]: Addison
                  - generic [ref=e240]:
                    - img [ref=e241]
                    - generic [ref=e245]: 07:02:41 AM
                  - generic [ref=e247]:
                    - generic [ref=e249]: T = 74.00
                    - generic [ref=e251]: C = 3.0
                    - generic [ref=e253]: L = 54.00
                    - generic [ref=e255]: 12:00 AM
          - button "reload" [ref=e257] [cursor=pointer]:
            - img [ref=e258]
        - generic [ref=e261]:
          - tablist [ref=e266]:
            - tab "SERVICE" [selected] [ref=e267] [cursor=pointer]:
              - generic [ref=e268]: SERVICE
            - tab "WAITING LIST" [ref=e269] [cursor=pointer]:
              - generic [ref=e270]: WAITING LIST
            - tab "CLOSED TICKET" [ref=e271] [cursor=pointer]:
              - generic [ref=e272]: CLOSED TICKET
            - tab "TURN DETAILS" [ref=e273] [cursor=pointer]:
              - generic [ref=e274]: TURN DETAILS
          - tabpanel [ref=e277]:
            - list [ref=e278]:
              - listitem [ref=e279] [cursor=pointer]:
                - img [ref=e280]
              - listitem [ref=e283] [cursor=pointer]:
                - img [ref=e284]
            - list [ref=e288]:
              - listitem [ref=e289] [cursor=pointer]:
                - generic [ref=e292]:
                  - generic [ref=e293]: "#111"
                  - list [ref=e294]:
                    - listitem [ref=e295]:
                      - generic [ref=e296]: W
                      - generic [ref=e297]: Claire
                - generic [ref=e299]:
                  - generic [ref=e300]: C
                  - generic [ref=e301]:
                    - generic [ref=e302]:
                      - generic [ref=e304]: Check-in
                      - generic [ref=e306]:
                        - img [ref=e307]
                        - generic [ref=e311]: 05:03 AM - Now
                      - generic [ref=e313]:
                        - img [ref=e314]
                        - generic [ref=e317]: Waiting for Service
                    - generic [ref=e318]:
                      - generic [ref=e319]: $0.00
                      - generic [ref=e321]: 0 min
              - listitem [ref=e322] [cursor=pointer]:
                - generic [ref=e325]:
                  - generic [ref=e326]: "#124"
                  - list [ref=e327]:
                    - listitem [ref=e328]:
                      - generic [ref=e329]: W
                      - generic [ref=e330]: Kayla
                - generic [ref=e332]:
                  - generic [ref=e333]: K
                  - generic [ref=e334]:
                    - generic [ref=e335]:
                      - generic [ref=e337]:
                        - img [ref=e338]
                        - generic [ref=e342]: 05:35 AM - Now
                      - generic [ref=e344]:
                        - img [ref=e345]
                        - generic [ref=e348]: Waiting for Service
                    - generic [ref=e349]:
                      - generic [ref=e350]: $0.00
                      - generic [ref=e352]: 0 min
              - listitem [ref=e353] [cursor=pointer]:
                - generic [ref=e356]:
                  - generic [ref=e357]: "#130"
                  - list [ref=e358]:
                    - listitem [ref=e359]:
                      - generic [ref=e360]: W
                      - generic [ref=e361]: Keelin
                - generic [ref=e363]:
                  - generic [ref=e364]: K
                  - generic [ref=e365]:
                    - generic [ref=e366]:
                      - generic [ref=e368]:
                        - img [ref=e369]
                        - generic [ref=e373]: 05:36 AM - Now
                      - generic [ref=e375]:
                        - img [ref=e376]
                        - generic [ref=e379]: Waiting for Service
                    - generic [ref=e380]:
                      - generic [ref=e381]: $0.00
                      - generic [ref=e383]: 0 min
              - listitem [ref=e384] [cursor=pointer]:
                - generic [ref=e387]:
                  - generic [ref=e388]: "#138"
                  - list [ref=e389]:
                    - listitem [ref=e390]:
                      - generic [ref=e391]: W
                      - generic [ref=e392]: Keelin
                - generic [ref=e394]:
                  - generic [ref=e395]: K
                  - generic [ref=e396]:
                    - generic [ref=e397]:
                      - generic [ref=e399]:
                        - img [ref=e400]
                        - generic [ref=e404]: 05:37 AM - Now
                      - generic [ref=e406]:
                        - img [ref=e407]
                        - generic [ref=e410]: Waiting for Service
                    - generic [ref=e411]:
                      - generic [ref=e412]: $0.00
                      - generic [ref=e414]: 0 min
              - listitem [ref=e415] [cursor=pointer]:
                - generic [ref=e418]:
                  - generic [ref=e419]: "#143"
                  - list [ref=e420]:
                    - listitem [ref=e421]:
                      - generic [ref=e422]: W
                      - generic [ref=e423]: Keelin
                - generic [ref=e425]:
                  - generic [ref=e426]: K
                  - generic [ref=e427]:
                    - generic [ref=e428]:
                      - generic [ref=e430]:
                        - img [ref=e431]
                        - generic [ref=e435]: 05:38 AM - Now
                      - generic [ref=e437]:
                        - img [ref=e438]
                        - generic [ref=e441]: Waiting for Service
                    - generic [ref=e442]:
                      - generic [ref=e443]: $0.00
                      - generic [ref=e445]: 0 min
              - listitem [ref=e446] [cursor=pointer]:
                - generic [ref=e449]:
                  - generic [ref=e450]: "#166"
                  - list [ref=e451]:
                    - listitem [ref=e452]:
                      - generic [ref=e453]: W
                      - generic [ref=e454]: Calantha
                - generic [ref=e456]:
                  - generic [ref=e457]: C
                  - generic [ref=e458]:
                    - generic [ref=e459]:
                      - generic [ref=e461]:
                        - img [ref=e462]
                        - generic [ref=e466]: 05:44 AM - Now
                      - generic [ref=e468]:
                        - img [ref=e469]
                        - generic [ref=e472]: Waiting for Service
                    - generic [ref=e473]:
                      - generic [ref=e474]: $0.00
                      - generic [ref=e476]: 0 min
              - listitem [ref=e477] [cursor=pointer]:
                - generic [ref=e480]:
                  - generic [ref=e481]: "#191"
                  - list [ref=e482]:
                    - listitem [ref=e483]:
                      - generic [ref=e484]: W
                      - generic [ref=e485]: Iris
                - generic [ref=e487]:
                  - generic [ref=e488]: I
                  - generic [ref=e489]:
                    - generic [ref=e490]:
                      - generic [ref=e492]:
                        - img [ref=e493]
                        - generic [ref=e497]: 05:47 AM - Now
                      - generic [ref=e499]:
                        - img [ref=e500]
                        - generic [ref=e503]: Waiting for Service
                    - generic [ref=e504]:
                      - generic [ref=e505]: $0.00
                      - generic [ref=e507]: 0 min
              - listitem [ref=e508] [cursor=pointer]:
                - generic [ref=e511]:
                  - generic [ref=e512]: "#192"
                  - list [ref=e513]:
                    - listitem [ref=e514]:
                      - generic [ref=e515]: W
                      - generic [ref=e516]: Brielle
                - generic [ref=e518]:
                  - generic [ref=e519]: B
                  - generic [ref=e520]:
                    - generic [ref=e521]:
                      - generic [ref=e523]:
                        - img [ref=e524]
                        - generic [ref=e528]: 05:47 AM - Now
                      - generic [ref=e530]:
                        - img [ref=e531]
                        - generic [ref=e534]: Waiting for Service
                    - generic [ref=e535]:
                      - generic [ref=e536]: $0.00
                      - generic [ref=e538]: 0 min
              - listitem [ref=e539] [cursor=pointer]:
                - generic [ref=e542]:
                  - generic [ref=e543]: "#195"
                  - list [ref=e544]:
                    - listitem [ref=e545]:
                      - generic [ref=e546]: W
                      - generic [ref=e547]: Sandy
                - generic [ref=e549]:
                  - generic [ref=e550]: S
                  - generic [ref=e551]:
                    - generic [ref=e552]:
                      - generic [ref=e554]:
                        - img [ref=e555]
                        - generic [ref=e559]: 05:48 AM - Now
                      - generic [ref=e561]:
                        - img [ref=e562]
                        - generic [ref=e565]: Waiting for Service
                    - generic [ref=e566]:
                      - generic [ref=e567]: $0.00
                      - generic [ref=e569]: 0 min
              - listitem [ref=e570] [cursor=pointer]:
                - generic [ref=e573]:
                  - generic [ref=e574]: "#200"
                  - list [ref=e575]:
                    - listitem [ref=e576]:
                      - generic [ref=e577]: W
                      - generic [ref=e578]: Jack
                - generic [ref=e580]:
                  - generic [ref=e581]: J
                  - generic [ref=e582]:
                    - generic [ref=e583]:
                      - generic [ref=e585]:
                        - img [ref=e586]
                        - generic [ref=e590]: 05:49 AM - Now
                      - generic [ref=e592]:
                        - img [ref=e593]
                        - generic [ref=e596]: Waiting for Service
                    - generic [ref=e597]:
                      - generic [ref=e598]: $0.00
                      - generic [ref=e600]: 0 min
              - listitem [ref=e601] [cursor=pointer]:
                - generic [ref=e604]:
                  - generic [ref=e605]: "#201"
                  - list [ref=e606]:
                    - listitem [ref=e607]:
                      - generic [ref=e608]: W
                      - generic [ref=e609]: Sandy
                - generic [ref=e611]:
                  - generic [ref=e612]: S
                  - generic [ref=e613]:
                    - generic [ref=e614]:
                      - generic [ref=e616]:
                        - img [ref=e617]
                        - generic [ref=e621]: 05:49 AM - Now
                      - generic [ref=e623]:
                        - img [ref=e624]
                        - generic [ref=e627]: Waiting for Service
                    - generic [ref=e628]:
                      - generic [ref=e629]: $0.00
                      - generic [ref=e631]: 0 min
              - listitem [ref=e632] [cursor=pointer]:
                - generic [ref=e635]:
                  - generic [ref=e636]: "#203"
                  - list [ref=e637]:
                    - listitem [ref=e638]:
                      - generic [ref=e639]: W
                      - generic [ref=e640]: Jack
                - generic [ref=e642]:
                  - generic [ref=e643]: J
                  - generic [ref=e644]:
                    - generic [ref=e645]:
                      - generic [ref=e647]:
                        - img [ref=e648]
                        - generic [ref=e652]: 05:49 AM - Now
                      - generic [ref=e654]:
                        - img [ref=e655]
                        - generic [ref=e658]: Waiting for Service
                    - generic [ref=e659]:
                      - generic [ref=e660]: $0.00
                      - generic [ref=e662]: 0 min
              - listitem [ref=e663] [cursor=pointer]:
                - generic [ref=e666]:
                  - generic [ref=e667]: "#204"
                  - list [ref=e668]:
                    - listitem [ref=e669]:
                      - generic [ref=e670]: W
                      - generic [ref=e671]: Sandy
                - generic [ref=e673]:
                  - generic [ref=e674]: S
                  - generic [ref=e675]:
                    - generic [ref=e676]:
                      - generic [ref=e678]:
                        - img [ref=e679]
                        - generic [ref=e683]: 05:49 AM - Now
                      - generic [ref=e685]:
                        - img [ref=e686]
                        - generic [ref=e689]: Waiting for Service
                    - generic [ref=e690]:
                      - generic [ref=e691]: $0.00
                      - generic [ref=e693]: 0 min
              - listitem [ref=e694] [cursor=pointer]:
                - generic [ref=e697]:
                  - generic [ref=e698]: "#220"
                  - list [ref=e699]:
                    - listitem [ref=e700]:
                      - generic [ref=e701]: W
                      - generic [ref=e702]: Keelin
                - generic [ref=e704]:
                  - generic [ref=e705]: K
                  - generic [ref=e706]:
                    - generic [ref=e707]:
                      - generic [ref=e709]:
                        - img [ref=e710]
                        - generic [ref=e714]: 07:02 AM - Now
                      - generic [ref=e716]:
                        - img [ref=e717]
                        - generic [ref=e720]: Waiting for Service
                    - generic [ref=e721]:
                      - generic [ref=e722]: $0.00
                      - generic [ref=e724]: 0 min
              - listitem [ref=e725] [cursor=pointer]:
                - generic [ref=e728]:
                  - generic [ref=e729]: "#226"
                  - list [ref=e730]:
                    - listitem [ref=e731]:
                      - generic [ref=e732]: W
                      - generic [ref=e733]: Keelin
                - generic [ref=e735]:
                  - generic [ref=e736]: K
                  - generic [ref=e737]:
                    - generic [ref=e738]:
                      - generic [ref=e740]:
                        - img [ref=e741]
                        - generic [ref=e745]: 07:03 AM - Now
                      - generic [ref=e747]:
                        - img [ref=e748]
                        - generic [ref=e751]: Waiting for Service
                    - generic [ref=e752]:
                      - generic [ref=e753]: $0.00
                      - generic [ref=e755]: 0 min
              - listitem [ref=e756] [cursor=pointer]:
                - generic [ref=e759]:
                  - generic [ref=e760]: "#231"
                  - list [ref=e761]:
                    - listitem [ref=e762]:
                      - generic [ref=e763]: W
                      - generic [ref=e764]: Keelin
                - generic [ref=e766]:
                  - generic [ref=e767]: K
                  - generic [ref=e768]:
                    - generic [ref=e769]:
                      - generic [ref=e771]:
                        - img [ref=e772]
                        - generic [ref=e776]: 07:04 AM - Now
                      - generic [ref=e778]:
                        - img [ref=e779]
                        - generic [ref=e782]: Waiting for Service
                    - generic [ref=e783]:
                      - generic [ref=e784]: $0.00
                      - generic [ref=e786]: 0 min
              - listitem [ref=e787] [cursor=pointer]:
                - generic [ref=e790]:
                  - generic [ref=e791]: "#233"
                  - list [ref=e792]:
                    - listitem [ref=e793]:
                      - generic [ref=e794]: D
                      - generic [ref=e795]: Ethan
                  - generic [ref=e797]: "1"
                - generic [ref=e798]:
                  - generic [ref=e799]: E
                  - generic [ref=e800]:
                    - generic [ref=e801]:
                      - generic [ref=e803]:
                        - img [ref=e804]
                        - generic [ref=e808]: 07:03 PM - Now
                      - generic [ref=e810]:
                        - img [ref=e811]
                        - generic [ref=e814]: Ready to Close
                    - generic [ref=e815]:
                      - generic [ref=e816]: $47.00
                      - generic [ref=e818]: 0 min
              - listitem [ref=e819] [cursor=pointer]:
                - generic [ref=e822]:
                  - generic [ref=e823]: "#236"
                  - list [ref=e824]:
                    - listitem [ref=e825]:
                      - generic [ref=e826]: D
                      - generic [ref=e827]: Ethan
                  - generic [ref=e829]: "1"
                - generic [ref=e830]:
                  - generic [ref=e831]: E
                  - generic [ref=e832]:
                    - generic [ref=e833]:
                      - generic [ref=e835]:
                        - img [ref=e836]
                        - generic [ref=e840]: 07:03 PM - Now
                      - generic [ref=e842]:
                        - img [ref=e843]
                        - generic [ref=e846]: Ready to Close
                    - generic [ref=e847]:
                      - generic [ref=e848]: $47.00
                      - generic [ref=e850]: 0 min
              - listitem [ref=e851] [cursor=pointer]:
                - generic [ref=e854]:
                  - generic [ref=e855]: "#268"
                  - list [ref=e856]:
                    - listitem [ref=e857]:
                      - generic [ref=e858]: W
                      - generic [ref=e859]: Iris
                - generic [ref=e861]:
                  - generic [ref=e862]: I
                  - generic [ref=e863]:
                    - generic [ref=e864]:
                      - generic [ref=e866]:
                        - img [ref=e867]
                        - generic [ref=e871]: 07:15 AM - Now
                      - generic [ref=e873]:
                        - img [ref=e874]
                        - generic [ref=e877]: Waiting for Service
                    - generic [ref=e878]:
                      - generic [ref=e879]: $0.00
                      - generic [ref=e881]: 0 min
              - listitem [ref=e882] [cursor=pointer]:
                - generic [ref=e885]:
                  - generic [ref=e886]: "#269"
                  - list [ref=e887]:
                    - listitem [ref=e888]:
                      - generic [ref=e889]: W
                      - generic [ref=e890]: Luna
                - generic [ref=e892]:
                  - generic [ref=e893]: L
                  - generic [ref=e894]:
                    - generic [ref=e895]:
                      - generic [ref=e897]:
                        - img [ref=e898]
                        - generic [ref=e902]: 07:15 AM - Now
                      - generic [ref=e904]:
                        - img [ref=e905]
                        - generic [ref=e908]: Waiting for Service
                    - generic [ref=e909]:
                      - generic [ref=e910]: $0.00
                      - generic [ref=e912]: 0 min
              - listitem [ref=e913] [cursor=pointer]:
                - generic [ref=e916]:
                  - generic [ref=e917]: "#271"
                  - list [ref=e918]:
                    - listitem [ref=e919]:
                      - generic [ref=e920]: W
                      - generic [ref=e921]: Iris
                - generic [ref=e923]:
                  - generic [ref=e924]: I
                  - generic [ref=e925]:
                    - generic [ref=e926]:
                      - generic [ref=e928]:
                        - img [ref=e929]
                        - generic [ref=e933]: 07:15 AM - Now
                      - generic [ref=e935]:
                        - img [ref=e936]
                        - generic [ref=e939]: Waiting for Service
                    - generic [ref=e940]:
                      - generic [ref=e941]: $0.00
                      - generic [ref=e943]: 0 min
              - listitem [ref=e944] [cursor=pointer]:
                - generic [ref=e947]:
                  - generic [ref=e948]: "#272"
                  - list [ref=e949]:
                    - listitem [ref=e950]:
                      - generic [ref=e951]: W
                      - generic [ref=e952]: WorkSlipAdjustTip
                - generic [ref=e954]:
                  - generic [ref=e955]: W
                  - generic [ref=e956]:
                    - generic [ref=e957]:
                      - generic [ref=e959]:
                        - img [ref=e960]
                        - generic [ref=e964]: 07:15 AM - Now
                      - generic [ref=e966]:
                        - img [ref=e967]
                        - generic [ref=e970]: Waiting for Service
                    - generic [ref=e971]:
                      - generic [ref=e972]: $0.00
                      - generic [ref=e974]: 0 min
              - listitem [ref=e975] [cursor=pointer]:
                - generic [ref=e978]:
                  - generic [ref=e979]: "#273"
                  - list [ref=e980]:
                    - listitem [ref=e981]:
                      - generic [ref=e982]: W
                      - generic [ref=e983]: Luna
                - generic [ref=e985]:
                  - generic [ref=e986]: L
                  - generic [ref=e987]:
                    - generic [ref=e988]:
                      - generic [ref=e990]:
                        - img [ref=e991]
                        - generic [ref=e995]: 07:16 AM - Now
                      - generic [ref=e997]:
                        - img [ref=e998]
                        - generic [ref=e1001]: Waiting for Service
                    - generic [ref=e1002]:
                      - generic [ref=e1003]: $0.00
                      - generic [ref=e1005]: 0 min
              - listitem [ref=e1006] [cursor=pointer]:
                - generic [ref=e1009]:
                  - generic [ref=e1010]: "#275"
                  - list [ref=e1011]:
                    - listitem [ref=e1012]:
                      - generic [ref=e1013]: W
                      - generic [ref=e1014]: WorkSlipAdjustTip
                - generic [ref=e1016]:
                  - generic [ref=e1017]: W
                  - generic [ref=e1018]:
                    - generic [ref=e1019]:
                      - generic [ref=e1021]:
                        - img [ref=e1022]
                        - generic [ref=e1026]: 07:16 AM - Now
                      - generic [ref=e1028]:
                        - img [ref=e1029]
                        - generic [ref=e1032]: Waiting for Service
                    - generic [ref=e1033]:
                      - generic [ref=e1034]: $0.00
                      - generic [ref=e1036]: 0 min
              - listitem [ref=e1037] [cursor=pointer]:
                - generic [ref=e1040]:
                  - generic [ref=e1041]: "#277"
                  - list [ref=e1042]:
                    - listitem [ref=e1043]:
                      - generic [ref=e1044]: W
                      - generic [ref=e1045]: Hazel
                - generic [ref=e1047]:
                  - generic [ref=e1048]: H
                  - generic [ref=e1049]:
                    - generic [ref=e1050]:
                      - generic [ref=e1052]:
                        - img [ref=e1053]
                        - generic [ref=e1057]: 07:17 AM - Now
                      - generic [ref=e1059]:
                        - img [ref=e1060]
                        - generic [ref=e1063]: Waiting for Service
                    - generic [ref=e1064]:
                      - generic [ref=e1065]: $0.00
                      - generic [ref=e1067]: 0 min
              - listitem [ref=e1068] [cursor=pointer]:
                - generic [ref=e1071]:
                  - generic [ref=e1072]: "#280"
                  - list [ref=e1073]:
                    - listitem [ref=e1074]:
                      - generic [ref=e1075]: W
                      - generic [ref=e1076]: WorkSlipAdjustTip
                - generic [ref=e1078]:
                  - generic [ref=e1079]: W
                  - generic [ref=e1080]:
                    - generic [ref=e1081]:
                      - generic [ref=e1083]:
                        - img [ref=e1084]
                        - generic [ref=e1088]: 07:17 AM - Now
                      - generic [ref=e1090]:
                        - img [ref=e1091]
                        - generic [ref=e1094]: Waiting for Service
                    - generic [ref=e1095]:
                      - generic [ref=e1096]: $0.00
                      - generic [ref=e1098]: 0 min
              - listitem [ref=e1099] [cursor=pointer]:
                - generic [ref=e1102]:
                  - generic [ref=e1103]: "#281"
                  - list [ref=e1104]:
                    - listitem [ref=e1105]:
                      - generic [ref=e1106]: W
                      - generic [ref=e1107]: Calantha
                - generic [ref=e1109]:
                  - generic [ref=e1110]: C
                  - generic [ref=e1111]:
                    - generic [ref=e1112]:
                      - generic [ref=e1114]:
                        - img [ref=e1115]
                        - generic [ref=e1119]: 07:17 AM - Now
                      - generic [ref=e1121]:
                        - img [ref=e1122]
                        - generic [ref=e1125]: Waiting for Service
                    - generic [ref=e1126]:
                      - generic [ref=e1127]: $0.00
                      - generic [ref=e1129]: 0 min
              - listitem [ref=e1130] [cursor=pointer]:
                - generic [ref=e1133]:
                  - generic [ref=e1134]: "#287"
                  - list [ref=e1135]:
                    - listitem [ref=e1136]:
                      - generic [ref=e1137]: W
                      - generic [ref=e1138]: Hazel
                - generic [ref=e1140]:
                  - generic [ref=e1141]: H
                  - generic [ref=e1142]:
                    - generic [ref=e1143]:
                      - generic [ref=e1145]:
                        - img [ref=e1146]
                        - generic [ref=e1150]: 07:18 AM - Now
                      - generic [ref=e1152]:
                        - img [ref=e1153]
                        - generic [ref=e1156]: Waiting for Service
                    - generic [ref=e1157]:
                      - generic [ref=e1158]: $0.00
                      - generic [ref=e1160]: 0 min
  - alert [ref=e1161]
```

# Test source

```ts
  4230 | 
  4231 | 		await expect(dataRow).toBeVisible();
  4232 | 
  4233 | 		// const totalSalesCell = dataRow.locator('td').nth(2);
  4234 | 		const regPayCell = dataRow.locator('td').nth(3);
  4235 | 		const ncTipCell = dataRow.locator('td').nth(4);
  4236 | 		const commissionCell = dataRow.locator('td').nth(5);
  4237 | 
  4238 | 		// await expect(totalSalesCell).toHaveText(regHrs);
  4239 | 		await expect(regPayCell).toHaveText(regPay);
  4240 | 		await expect(ncTipCell).toHaveText(ncTip);
  4241 | 		await expect(commissionCell).toHaveText(commission);
  4242 | 	},
  4243 | );
  4244 | 
  4245 | Then(
  4246 | 	'I should see the first Total {string} in the single payroll view',
  4247 | 	async ({ page }, amount: string) => {
  4248 | 		const totalRow = page
  4249 | 			.locator('table tbody tr')
  4250 | 			.filter({ hasText: 'Total' })
  4251 | 			.first();
  4252 | 		const amountCell = totalRow.locator('td').nth(1);
  4253 | 
  4254 | 		await expect(amountCell).toBeVisible();
  4255 | 		await expect(amountCell).toHaveText(amount);
  4256 | 	},
  4257 | );
  4258 | When('I waiting 1s', async ({ page }) => {
  4259 | 	await page.waitForTimeout(1000);
  4260 | });
  4261 | 
  4262 | When('I click on the reset key', async ({ page }) => {
  4263 | 	const resetButton = page.locator('svg[data-testid="XResetIcon"]');
  4264 | 	await expect(resetButton).toBeVisible();
  4265 | 	await resetButton.click();
  4266 | });
  4267 | Then('I should see no results found', async ({ page }) => {
  4268 | 	const noResults = page.locator('text=No results found');
  4269 | 	await expect(noResults).toBeVisible();
  4270 | });
  4271 | Then(
  4272 | 	'I should see the new void reason name {string} {string}, created at today, in the list',
  4273 | 	async ({ page }, field: string, value: string) => {
  4274 | 		const newRow = page.locator('.MuiDataGrid-row', {
  4275 | 			has: page.locator(`[data-field="${field}"]`, { hasText: value }),
  4276 | 		});
  4277 | 
  4278 | 		const valueCell = newRow.locator(`[data-field="${field}"]`);
  4279 | 		const dateCell = newRow.locator('[data-field="createdAt"]');
  4280 | 
  4281 | 		const formattedToday = await page.evaluate(() => {
  4282 | 			const today = new Date();
  4283 | 			return today.toLocaleDateString('en-US', {
  4284 | 				year: 'numeric',
  4285 | 				month: '2-digit',
  4286 | 				day: '2-digit',
  4287 | 			});
  4288 | 		});
  4289 | 
  4290 | 		await expect(valueCell).toBeVisible();
  4291 | 		await expect(valueCell).toHaveText(value);
  4292 | 		await expect(dateCell).toBeVisible();
  4293 | 		await expect(dateCell).toContainText(formattedToday);
  4294 | 	},
  4295 | );
  4296 | Then(
  4297 | 	'I should see the {string} Adjustment',
  4298 | 	async ({ page }, Title: string) => {
  4299 | 		const titleAdjustTurn = page.locator('.dailyTask__title');
  4300 | 
  4301 | 		await expect(titleAdjustTurn).toBeVisible();
  4302 | 		await expect(titleAdjustTurn).toHaveText(Title);
  4303 | 	},
  4304 | );
  4305 | When(
  4306 | 	'I click on the {string} in turn adjustment',
  4307 | 	async ({ page }, addJustTurn: string) => {
  4308 | 		const lateTurn = page
  4309 | 			.locator('.dailyTask')
  4310 | 			.locator('.MuiListItem-root')
  4311 | 			.filter({ hasText: new RegExp(`^${addJustTurn}$`) });
  4312 | 		await expect(lateTurn).toBeVisible();
  4313 | 		await expect(lateTurn).toHaveText(addJustTurn);
  4314 | 		await lateTurn.click();
  4315 | 	},
  4316 | );
  4317 | Then(
  4318 | 	'I should see Employee {string} with {string} in the employee list',
  4319 | 	async ({ page }, employeeName: string, turn: string) => {
  4320 | 		const listEmployee = page.locator('ul.ListItemEmployee__wrap ').first();
  4321 | 		await expect(listEmployee).toBeVisible();
  4322 | 		const employeeRow = listEmployee
  4323 | 			.locator('li.xEmployeeItem')
  4324 | 			.filter({ hasText: employeeName });
  4325 | 		await expect(employeeRow).toBeVisible();
  4326 | 		const turnCell = employeeRow
  4327 | 			.locator('div.xEmployeeItem__time')
  4328 | 			.locator('span.MuiChip-label')
  4329 | 			.first();
> 4330 | 		await expect(turnCell).toHaveText(turn);
       |                          ^ Error: expect(locator).toHaveText(expected) failed
  4331 | 	},
  4332 | );
  4333 | Then(
  4334 | 	'I should see the position employee {string} is {string}',
  4335 | 	async ({ page }, employeeName: string, position: string) => {
  4336 | 		const listEmployee = page.locator('ul.ListItemEmployee__wrap ').first();
  4337 | 		await expect(listEmployee).toBeVisible();
  4338 | 
  4339 | 		const employeeRow = listEmployee
  4340 | 			.locator('li.xEmployeeItem')
  4341 | 			.filter({ hasText: employeeName });
  4342 | 		await expect(employeeRow).toBeVisible();
  4343 | 
  4344 | 		const numberPosition = employeeRow.locator('.number');
  4345 | 		await expect(numberPosition).toBeVisible();
  4346 | 		await expect(numberPosition).toHaveText(position);
  4347 | 	},
  4348 | );
  4349 | 
  4350 | Then(
  4351 | 	'I should see the header {string} in the bill render',
  4352 | 	async ({ page }, header: string) => {
  4353 | 		const billRender = page.locator('.bill-render');
  4354 | 		await expect(billRender).toBeVisible();
  4355 | 
  4356 | 		const headerElement = billRender
  4357 | 			.locator('p.header')
  4358 | 			.getByText(header, { exact: true });
  4359 | 		await expect(headerElement).toBeVisible();
  4360 | 	},
  4361 | );
  4362 | 
  4363 | Then(
  4364 | 	'I should see the detail {string} in the bill render',
  4365 | 	async ({ page }, detail: string) => {
  4366 | 		const colonIndex = detail.indexOf(':');
  4367 | 		if (colonIndex === -1) {
  4368 | 			throw new Error(
  4369 | 				`Invalid detail format: "${detail}". Expected format: "Label: Value"`,
  4370 | 			);
  4371 | 		}
  4372 | 
  4373 | 		const labelPart = detail.substring(0, colonIndex).trim(); // E.g.: "Technician Name"
  4374 | 		const expectedValue = detail.substring(colonIndex + 1).trim(); // E.g.: "Elena"
  4375 | 
  4376 | 		const infoRow = page.locator('.info-row').filter({
  4377 | 			has: page.locator('.info-label', {
  4378 | 				hasText: new RegExp(`^\\s*${labelPart}\\s*:?\\s*$`),
  4379 | 			}),
  4380 | 		});
  4381 | 
  4382 | 		await expect(infoRow).toBeVisible();
  4383 | 
  4384 | 		const valueElement = infoRow.locator('.info-value');
  4385 | 		await expect(valueElement).toBeVisible();
  4386 | 		await expect(valueElement).toContainText(expectedValue);
  4387 | 	},
  4388 | );
  4389 | 
  4390 | Then(
  4391 | 	'I should see the {string} with value {string} in the sale row detail',
  4392 | 	async ({ page }, field: string, value: string) => {
  4393 | 		const billRender = page.locator('.bill-render');
  4394 | 		await expect(billRender).toBeVisible();
  4395 | 
  4396 | 		const salesRow = billRender
  4397 | 			.locator('.sales-details .sales-row')
  4398 | 			.filter({ hasNot: billRender.locator('.total-row') })
  4399 | 			.first();
  4400 | 		await expect(salesRow).toBeVisible();
  4401 | 
  4402 | 		const fieldToSelector: Record<string, string> = {
  4403 | 			'Item Name': '.item-name',
  4404 | 			QTY: '.quantity',
  4405 | 			Tip: '.tip',
  4406 | 			Amount: '.amount',
  4407 | 		};
  4408 | 
  4409 | 		const selector = fieldToSelector[field];
  4410 | 		if (!selector) {
  4411 | 			throw new Error(
  4412 | 				`Unsupported sale row field: "${field}". Supported fields: ${Object.keys(
  4413 | 					fieldToSelector,
  4414 | 				).join(', ')}`,
  4415 | 			);
  4416 | 		}
  4417 | 
  4418 | 		const cell = salesRow.locator(selector);
  4419 | 		await expect(cell).toBeVisible();
  4420 | 
  4421 | 		if (field === 'Item Name') {
  4422 | 			const cellText = (await cell.innerText()).replace(/\s+/g, ' ').trim();
  4423 | 			const expected = value.replace(/\s+/g, ' ').trim();
  4424 | 			expect(cellText).toContain(expected);
  4425 | 			return;
  4426 | 		}
  4427 | 
  4428 | 		await expect(cell).toHaveText(value, { useInnerText: true });
  4429 | 	},
  4430 | );
```