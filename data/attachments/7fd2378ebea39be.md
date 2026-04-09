# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: create-tickets.feature.spec.js >> Create tickets >> Apply auto-discount item and change it to another
- Location: dist/bdd/create-tickets.feature.spec.js:369:3

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: locator('div.xQueueList').getByText('Brielle', { exact: true })
Expected: visible
Timeout: 30000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 30000ms
  - waiting for locator('div.xQueueList').getByText('Brielle', { exact: true })

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
          - generic [ref=e14]:
            - generic [ref=e15]:
              - generic [ref=e16]: FUNCTIONS
              - generic [ref=e17]:
                - generic [ref=e18]:
                  - generic [ref=e19]:
                    - generic [ref=e20]: "04"
                    - generic [ref=e21]: ":"
                    - generic [ref=e22]: "28"
                    - generic [ref=e23]: ":"
                    - generic [ref=e24]: "39"
                  - generic [ref=e25]: AM
                - generic [ref=e26]: 04/09/2026
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
          - generic [ref=e70]: 04/09/2026
      - paragraph [ref=e71]: © 2026 XSoftware
    - main [ref=e72]:
      - generic [ref=e73]:
        - generic [ref=e74]:
          - generic [ref=e75]:
            - tablist [ref=e80]:
              - tab "NAILS" [selected] [ref=e81] [cursor=pointer]:
                - generic [ref=e82]: NAILS
              - tab "HAIR" [ref=e83] [cursor=pointer]:
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
                    - generic [ref=e104]: D
                    - generic [ref=e106]:
                      - generic [ref=e107]: "#1"
                      - generic [ref=e108]: David
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
                    - generic [ref=e130]: W
                    - generic [ref=e132]:
                      - generic [ref=e133]: "#2"
                      - generic [ref=e134]: WorkSlipAdjustTip2
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
                    - generic [ref=e156]: Z
                    - generic [ref=e158]:
                      - generic [ref=e159]: "#3"
                      - generic [ref=e160]: Zoey
                  - generic [ref=e162]:
                    - img [ref=e163]
                    - generic [ref=e167]: 12:00:00 AM
                  - generic [ref=e169]:
                    - generic [ref=e171]: T = 0.00
                    - generic [ref=e173]: C = 0.0
                    - generic [ref=e175]: L = 0.00
                    - generic [ref=e177]: 12:00 AM
                - listitem [ref=e178] [cursor=pointer]:
                  - generic [ref=e180]:
                    - generic [ref=e182]: J
                    - generic [ref=e184]:
                      - generic [ref=e185]: "#4"
                      - generic [ref=e186]: Jarvis
                  - generic [ref=e188]:
                    - img [ref=e189]
                    - generic [ref=e193]: 12:00:00 AM
                  - generic [ref=e195]:
                    - generic [ref=e197]: T = 0.00
                    - generic [ref=e199]: C = 0.0
                    - generic [ref=e201]: L = 0.00
                    - generic [ref=e203]: 12:00 AM
                - listitem [ref=e204] [cursor=pointer]:
                  - generic [ref=e206]:
                    - generic [ref=e208]: C
                    - generic [ref=e210]:
                      - generic [ref=e211]: "#5"
                      - generic [ref=e212]: Calantha
                  - generic [ref=e214]:
                    - img [ref=e215]
                    - generic [ref=e219]: 04:21:38 AM
                  - generic [ref=e221]:
                    - generic [ref=e223]: T = 0.00
                    - generic [ref=e225]: C = 0.0
                    - generic [ref=e227]: L = 0.00
                    - generic [ref=e229]: 04:21 AM
                - listitem [ref=e230] [cursor=pointer]:
                  - generic [ref=e232]:
                    - generic [ref=e234]: A
                    - generic [ref=e236]:
                      - generic [ref=e237]: "#6"
                      - generic [ref=e238]: Amelia
                  - generic [ref=e240]:
                    - img [ref=e241]
                    - generic [ref=e245]: 07:00:00 AM
                  - generic [ref=e247]:
                    - generic [ref=e249]: T = 0.00
                    - generic [ref=e251]: C = 0.0
                    - generic [ref=e253]: L = 0.00
                    - generic [ref=e255]: 07:00 AM
                - listitem [ref=e256] [cursor=pointer]:
                  - generic [ref=e258]:
                    - generic [ref=e260]: S
                    - generic [ref=e262]:
                      - generic [ref=e263]: "#7"
                      - generic [ref=e264]: Savannah
                  - generic [ref=e266]:
                    - img [ref=e267]
                    - generic [ref=e271]: 07:00:00 AM
                  - generic [ref=e273]:
                    - generic [ref=e275]: T = 0.00
                    - generic [ref=e277]: C = 0.0
                    - generic [ref=e279]: L = 0.00
                    - generic [ref=e281]: 07:00 AM
                - listitem [ref=e282] [cursor=pointer]:
                  - generic [ref=e284]:
                    - generic [ref=e286]: T
                    - generic [ref=e288]:
                      - generic [ref=e289]: "#8"
                      - generic [ref=e290]: Tom
                  - generic [ref=e292]:
                    - img [ref=e293]
                    - generic [ref=e297]: 07:00:00 AM
                  - generic [ref=e299]:
                    - generic [ref=e301]: T = 0.00
                    - generic [ref=e303]: C = 0.0
                    - generic [ref=e305]: L = 0.00
                    - generic [ref=e307]: 07:00 AM
                - listitem [ref=e308] [cursor=pointer]:
                  - generic [ref=e310]:
                    - generic [ref=e312]: V
                    - generic [ref=e314]:
                      - generic [ref=e315]: "#9"
                      - generic [ref=e316]: Victoria
                  - generic [ref=e318]:
                    - img [ref=e319]
                    - generic [ref=e323]: 07:00:00 AM
                  - generic [ref=e325]:
                    - generic [ref=e327]: T = 0.00
                    - generic [ref=e329]: C = 0.0
                    - generic [ref=e331]: L = 0.00
                    - generic [ref=e333]: 07:00 AM
                - listitem [ref=e334] [cursor=pointer]:
                  - generic [ref=e336]:
                    - generic [ref=e338]: J
                    - generic [ref=e340]:
                      - generic [ref=e341]: "#10"
                      - generic [ref=e342]: Jack
                  - generic [ref=e344]:
                    - img [ref=e345]
                    - generic [ref=e349]: 07:00:00 AM
                  - generic [ref=e351]:
                    - generic [ref=e353]: T = 0.00
                    - generic [ref=e355]: C = 0.0
                    - generic [ref=e357]: L = 0.00
                    - generic [ref=e359]: 07:00 AM
                - listitem [ref=e360] [cursor=pointer]:
                  - generic [ref=e362]:
                    - generic [ref=e364]: A
                    - generic [ref=e366]:
                      - generic [ref=e367]: "#11"
                      - generic [ref=e368]: Almira
                  - generic [ref=e370]:
                    - img [ref=e371]
                    - generic [ref=e375]: 07:00:00 AM
                  - generic [ref=e377]:
                    - generic [ref=e379]: T = 0.00
                    - generic [ref=e381]: C = 0.0
                    - generic [ref=e383]: L = 0.00
                    - generic [ref=e385]: 07:00 AM
                - listitem [ref=e386] [cursor=pointer]:
                  - generic [ref=e388]:
                    - generic [ref=e390]: M
                    - generic [ref=e392]:
                      - generic [ref=e393]: "#12"
                      - generic [ref=e394]: Maya
                  - generic [ref=e396]:
                    - img [ref=e397]
                    - generic [ref=e401]: 07:00:00 AM
                  - generic [ref=e403]:
                    - generic [ref=e405]: T = 0.00
                    - generic [ref=e407]: C = 0.0
                    - generic [ref=e409]: L = 0.00
                    - generic [ref=e411]: 07:00 AM
                - listitem [ref=e412] [cursor=pointer]:
                  - generic [ref=e414]:
                    - generic [ref=e416]: L
                    - generic [ref=e418]:
                      - generic [ref=e419]: "#13"
                      - generic [ref=e420]: Leah
                  - generic [ref=e422]:
                    - img [ref=e423]
                    - generic [ref=e427]: 07:00:00 AM
                  - generic [ref=e429]:
                    - generic [ref=e431]: T = 0.00
                    - generic [ref=e433]: C = 0.0
                    - generic [ref=e435]: L = 0.00
                    - generic [ref=e437]: 07:00 AM
                - listitem [ref=e438] [cursor=pointer]:
                  - generic [ref=e440]:
                    - generic [ref=e442]: S
                    - generic [ref=e444]:
                      - generic [ref=e445]: "#14"
                      - generic [ref=e446]: Sam
                  - generic [ref=e448]:
                    - img [ref=e449]
                    - generic [ref=e453]: 07:00:00 AM
                  - generic [ref=e455]:
                    - generic [ref=e457]: T = 0.00
                    - generic [ref=e459]: C = 0.0
                    - generic [ref=e461]: L = 0.00
                    - generic [ref=e463]: 07:00 AM
                - listitem [ref=e464] [cursor=pointer]:
                  - generic [ref=e466]:
                    - generic [ref=e468]: E
                    - generic [ref=e470]:
                      - generic [ref=e471]: "#15"
                      - generic [ref=e472]: Eira
                  - generic [ref=e474]:
                    - img [ref=e475]
                    - generic [ref=e479]: 07:00:00 AM
                  - generic [ref=e481]:
                    - generic [ref=e483]: T = 0.00
                    - generic [ref=e485]: C = 0.0
                    - generic [ref=e487]: L = 0.00
                    - generic [ref=e489]: 07:00 AM
                - listitem [ref=e490] [cursor=pointer]:
                  - generic [ref=e492]:
                    - generic [ref=e494]: H
                    - generic [ref=e496]:
                      - generic [ref=e497]: "#16"
                      - generic [ref=e498]: Hailey
                  - generic [ref=e500]:
                    - img [ref=e501]
                    - generic [ref=e505]: 07:00:00 AM
                  - generic [ref=e507]:
                    - generic [ref=e509]: T = 0.00
                    - generic [ref=e511]: C = 0.0
                    - generic [ref=e513]: L = 0.00
                    - generic [ref=e515]: 07:00 AM
                - listitem [ref=e516] [cursor=pointer]:
                  - generic [ref=e518]:
                    - generic [ref=e520]: S
                    - generic [ref=e522]:
                      - generic [ref=e523]: "#17"
                      - generic [ref=e524]: Sarah
                  - generic [ref=e526]:
                    - img [ref=e527]
                    - generic [ref=e531]: 07:00:00 AM
                  - generic [ref=e533]:
                    - generic [ref=e535]: T = 0.00
                    - generic [ref=e537]: C = 0.0
                    - generic [ref=e539]: L = 0.00
                    - generic [ref=e541]: 07:00 AM
                - listitem [ref=e542] [cursor=pointer]:
                  - generic [ref=e544]:
                    - generic [ref=e546]: C
                    - generic [ref=e548]:
                      - generic [ref=e549]: "#18"
                      - generic [ref=e550]: Ciara
                  - generic [ref=e552]:
                    - img [ref=e553]
                    - generic [ref=e557]: 07:00:00 AM
                  - generic [ref=e559]:
                    - generic [ref=e561]: T = 0.00
                    - generic [ref=e563]: C = 0.0
                    - generic [ref=e565]: L = 0.00
                    - generic [ref=e567]: 07:00 AM
                - listitem [ref=e568] [cursor=pointer]:
                  - generic [ref=e570]:
                    - generic [ref=e572]: S
                    - generic [ref=e574]:
                      - generic [ref=e575]: "#19"
                      - generic [ref=e576]: Sandy
                  - generic [ref=e578]:
                    - img [ref=e579]
                    - generic [ref=e583]: 07:00:00 AM
                  - generic [ref=e585]:
                    - generic [ref=e587]: T = 0.00
                    - generic [ref=e589]: C = 0.0
                    - generic [ref=e591]: L = 0.00
                    - generic [ref=e593]: 07:00 AM
                - listitem [ref=e594] [cursor=pointer]:
                  - generic [ref=e596]:
                    - generic [ref=e598]: S
                    - generic [ref=e600]:
                      - generic [ref=e601]: "#20"
                      - generic [ref=e602]: Sophia
                  - generic [ref=e604]:
                    - img [ref=e605]
                    - generic [ref=e609]: 07:00:00 AM
                  - generic [ref=e611]:
                    - generic [ref=e613]: T = 0.00
                    - generic [ref=e615]: C = 0.0
                    - generic [ref=e617]: L = 0.00
                    - generic [ref=e619]: 07:00 AM
                - listitem [ref=e620] [cursor=pointer]:
                  - generic [ref=e622]:
                    - img "item service Owner" [ref=e625]
                    - generic [ref=e627]:
                      - generic [ref=e628]: "#21"
                      - generic [ref=e629]: Owner
                  - generic [ref=e631]:
                    - img [ref=e632]
                    - generic [ref=e636]: 04:21:28 AM
                  - generic [ref=e638]:
                    - generic [ref=e640]: T = 6.00
                    - generic [ref=e642]: C = 0.0
                    - generic [ref=e644]: L = 6.00
                    - generic [ref=e646]: 04:21 AM
                - listitem [ref=e647] [cursor=pointer]:
                  - generic [ref=e649]:
                    - generic [ref=e651]: D
                    - generic [ref=e653]:
                      - generic [ref=e654]: "#22"
                      - generic [ref=e655]: Dylan
                  - generic [ref=e657]:
                    - img [ref=e658]
                    - generic [ref=e662]: 04:24:05 AM
                  - generic [ref=e664]:
                    - generic [ref=e666]: T = 6.00
                    - generic [ref=e668]: C = 0.0
                    - generic [ref=e670]: L = 6.00
                    - generic [ref=e672]: 04:22 AM
                - listitem [ref=e673] [cursor=pointer]:
                  - generic [ref=e675]:
                    - generic [ref=e677]: E
                    - generic [ref=e679]:
                      - generic [ref=e680]: "#23"
                      - generic [ref=e681]: Emily
                  - generic [ref=e683]:
                    - img [ref=e684]
                    - generic [ref=e688]: 04:09:09 AM
                  - generic [ref=e690]:
                    - generic [ref=e692]: T = 6.00
                    - generic [ref=e694]: C = 0.0
                    - generic [ref=e696]: L = 6.00
                    - generic [ref=e698]: 07:00 AM
                - listitem [ref=e699] [cursor=pointer]:
                  - generic [ref=e701]:
                    - generic [ref=e703]: M
                    - generic [ref=e705]:
                      - generic [ref=e706]: "#24"
                      - generic [ref=e707]: Mia
                  - generic [ref=e709]:
                    - img [ref=e710]
                    - generic [ref=e714]: 04:12:40 AM
                  - generic [ref=e716]:
                    - generic [ref=e718]: T = 8.00
                    - generic [ref=e720]: C = 0.0
                    - generic [ref=e722]: L = 8.00
                    - generic [ref=e724]: 04:12 AM
                - listitem [ref=e725] [cursor=pointer]:
                  - generic [ref=e727]:
                    - generic [ref=e729]: C
                    - generic [ref=e731]:
                      - generic [ref=e732]: "#25"
                      - generic [ref=e733]: Claire
                  - generic [ref=e735]:
                    - img [ref=e736]
                    - generic [ref=e740]: 04:09:09 AM
                  - generic [ref=e742]:
                    - generic [ref=e744]: T = 8.00
                    - generic [ref=e746]: C = 0.0
                    - generic [ref=e748]: L = 8.00
                    - generic [ref=e750]: 07:00 AM
                - listitem [ref=e751] [cursor=pointer]:
                  - generic [ref=e753]:
                    - generic [ref=e755]: A
                    - generic [ref=e757]:
                      - generic [ref=e758]: "#26"
                      - generic [ref=e759]: Addison
                  - generic [ref=e761]:
                    - img [ref=e762]
                    - generic [ref=e766]: 04:17:12 AM
                  - generic [ref=e768]:
                    - generic [ref=e770]: T = 20.00
                    - generic [ref=e772]: C = 1.0
                    - generic [ref=e774]: L = 37.00
                    - generic [ref=e776]: 12:00 AM
                - listitem [ref=e777] [cursor=pointer]:
                  - generic [ref=e779]:
                    - generic [ref=e781]: C
                    - generic [ref=e783]:
                      - generic [ref=e784]: "#27"
                      - generic [ref=e785]: Christ
                  - generic [ref=e787]:
                    - img [ref=e788]
                    - generic [ref=e792]: 04:10:34 AM
                  - generic [ref=e794]:
                    - generic [ref=e796]: T = 53.50
                    - generic [ref=e798]: C = 2.0
                    - generic [ref=e800]: L = 33.50
                    - generic [ref=e802]: 07:00 AM
                - listitem [ref=e803] [cursor=pointer]:
                  - generic [ref=e805]:
                    - generic [ref=e807]: K
                    - generic [ref=e809]:
                      - generic [ref=e810]: "#28"
                      - generic [ref=e811]: Kelley
                  - generic [ref=e813]:
                    - img [ref=e814]
                    - generic [ref=e818]: 04:25:46 AM
                  - generic [ref=e820]:
                    - generic [ref=e822]: T = 59.00
                    - generic [ref=e824]: C = 2.0
                    - generic [ref=e826]: L = 6.00
                    - generic [ref=e828]: 07:00 AM
                - listitem [ref=e829] [cursor=pointer]:
                  - generic [ref=e831]:
                    - generic [ref=e833]: A
                    - generic [ref=e835]:
                      - generic [ref=e836]: "#29"
                      - generic [ref=e837]: Alexis
                  - generic [ref=e839]:
                    - img [ref=e840]
                    - generic [ref=e844]: 04:18:59 AM
                  - generic [ref=e846]:
                    - generic [ref=e848]: T = 77.10
                    - generic [ref=e850]: C = 3.0
                    - generic [ref=e852]: L = 37.10
                    - generic [ref=e854]: 04:15 AM
                - listitem [ref=e855] [cursor=pointer]:
                  - generic [ref=e857]:
                    - generic [ref=e859]: A
                    - generic [ref=e861]:
                      - generic [ref=e862]: "#30"
                      - generic [ref=e863]: Anna
                  - generic [ref=e865]:
                    - img [ref=e866]
                    - generic [ref=e870]: 04:24:20 AM
                  - generic [ref=e872]:
                    - generic [ref=e874]: T = 160.00
                    - generic [ref=e876]: C = 8.0
                    - generic [ref=e878]: L = 20.00
                    - generic [ref=e880]: 12:00 AM
          - button "reload" [ref=e882] [cursor=pointer]:
            - img [ref=e883]
        - generic [ref=e886]:
          - tablist [ref=e891]:
            - tab "SERVICE" [selected] [ref=e892] [cursor=pointer]:
              - generic [ref=e893]: SERVICE
            - tab "WAITING LIST" [ref=e894] [cursor=pointer]:
              - generic [ref=e895]: WAITING LIST
            - tab "CLOSED TICKET" [ref=e896] [cursor=pointer]:
              - generic [ref=e897]: CLOSED TICKET
            - tab "TURN DETAILS" [ref=e898] [cursor=pointer]:
              - generic [ref=e899]: TURN DETAILS
          - tabpanel [ref=e902]:
            - list [ref=e903]:
              - listitem [ref=e904] [cursor=pointer]:
                - img [ref=e905]
              - listitem [ref=e908] [cursor=pointer]:
                - img [ref=e909]
            - list [ref=e913]:
              - listitem [ref=e914] [cursor=pointer]:
                - generic [ref=e917]:
                  - generic [ref=e918]: "#156"
                  - list [ref=e919]:
                    - listitem [ref=e920]:
                      - generic [ref=e921]: W
                      - generic [ref=e922]: WorkSlipAdjustTip
                - generic [ref=e924]:
                  - generic [ref=e925]: W
                  - generic [ref=e926]:
                    - generic [ref=e927]:
                      - generic [ref=e929]:
                        - img [ref=e930]
                        - generic [ref=e934]: 04:21 AM - Now
                      - generic [ref=e936]:
                        - img [ref=e937]
                        - generic [ref=e940]: Waiting for Service
                    - generic [ref=e941]:
                      - generic [ref=e942]: $0.00
                      - generic [ref=e944]: 0 min
              - listitem [ref=e945] [cursor=pointer]:
                - generic [ref=e948]:
                  - generic [ref=e949]: "#159"
                  - list [ref=e950]:
                    - listitem [ref=e951]:
                      - generic [ref=e952]: W
                      - generic [ref=e953]: Calantha
                - generic [ref=e955]:
                  - generic [ref=e956]: C
                  - generic [ref=e957]:
                    - generic [ref=e958]:
                      - generic [ref=e960]:
                        - img [ref=e961]
                        - generic [ref=e965]: 04:21 AM - Now
                      - generic [ref=e967]:
                        - img [ref=e968]
                        - generic [ref=e971]: Waiting for Service
                    - generic [ref=e972]:
                      - generic [ref=e973]: $0.00
                      - generic [ref=e975]: 0 min
              - listitem [ref=e976] [cursor=pointer]:
                - generic [ref=e979]:
                  - generic [ref=e980]: "#165"
                  - list [ref=e981]:
                    - listitem [ref=e982]:
                      - generic [ref=e983]: W
                      - generic [ref=e984]: Calantha
                - generic [ref=e986]:
                  - generic [ref=e987]: C
                  - generic [ref=e988]:
                    - generic [ref=e989]:
                      - generic [ref=e991]:
                        - img [ref=e992]
                        - generic [ref=e996]: 04:23 AM - Now
                      - generic [ref=e998]:
                        - img [ref=e999]
                        - generic [ref=e1002]: Waiting for Service
                    - generic [ref=e1003]:
                      - generic [ref=e1004]: $0.00
                      - generic [ref=e1006]: 0 min
              - listitem [ref=e1007] [cursor=pointer]:
                - generic [ref=e1010]:
                  - generic [ref=e1011]: "#170"
                  - list [ref=e1012]:
                    - listitem [ref=e1013]:
                      - generic [ref=e1014]: W
                      - generic [ref=e1015]: Calantha
                - generic [ref=e1017]:
                  - generic [ref=e1018]: C
                  - generic [ref=e1019]:
                    - generic [ref=e1020]:
                      - generic [ref=e1022]:
                        - img [ref=e1023]
                        - generic [ref=e1027]: 04:24 AM - Now
                      - generic [ref=e1029]:
                        - img [ref=e1030]
                        - generic [ref=e1033]: Waiting for Service
                    - generic [ref=e1034]:
                      - generic [ref=e1035]: $0.00
                      - generic [ref=e1037]: 0 min
              - listitem [ref=e1038] [cursor=pointer]:
                - generic [ref=e1041]:
                  - generic [ref=e1042]: "#180"
                  - list [ref=e1043]:
                    - listitem [ref=e1044]:
                      - generic [ref=e1045]: W
                      - generic [ref=e1046]: Brielle
                  - generic [ref=e1048]: "1"
                - generic [ref=e1049]:
                  - generic [ref=e1050]: B
                  - generic [ref=e1051]:
                    - generic [ref=e1052]:
                      - generic [ref=e1054]:
                        - img [ref=e1055]
                        - generic [ref=e1059]: 04:27 AM - Now
                      - generic [ref=e1061]:
                        - img [ref=e1062]
                        - generic [ref=e1065]: Ombre - $0.00
                    - generic [ref=e1066]:
                      - generic [ref=e1067]: $0.00
                      - generic [ref=e1069]: 0 min
  - alert [ref=e1070]
```

# Test source

```ts
  1   | import { expect } from '@playwright/test';
  2   | import { createBdd, type DataTable } from 'playwright-bdd';
  3   | 
  4   | import { constants } from '#const';
  5   | import { type PageId } from '#types';
  6   | 
  7   | const { When, Then } = createBdd();
  8   | 
  9   | Then(
  10  | 	'I should be redirected to {pageId} page',
  11  | 	async ({ page }, pageId: PageId) => {
  12  | 		const pageUrl = constants.PageUrl[pageId];
  13  | 
  14  | 		await page.waitForURL(pageUrl);
  15  | 		await expect(page).toHaveURL(pageUrl);
  16  | 	},
  17  | );
  18  | 
  19  | When('I click on the functions', async ({ page }) => {
  20  | 	await page.locator('.pageName').getByText('FUNCTIONS').click();
  21  | });
  22  | 
  23  | When(
  24  | 	'I select the {string} on the Daily Task',
  25  | 	async ({ page }, task: string) => {
  26  | 		await page.locator('.dailyTask').getByText(task, { exact: true }).click();
  27  | 	},
  28  | );
  29  | 
  30  | Then(
  31  | 	'I should see the employee {string} in the employee list',
  32  | 	async ({ page }, employeeName: string) => {
  33  | 		const employeeList = page.locator('div.xQueueList');
  34  | 
  35  | 		await expect(
  36  | 			employeeList.getByText(employeeName, { exact: true }),
> 37  | 		).toBeVisible();
      |     ^ Error: expect(locator).toBeVisible() failed
  38  | 	},
  39  | );
  40  | 
  41  | Then(
  42  | 	'I should see the employee {string} in the payroll list',
  43  | 	async ({ page }, employeeName: string) => {
  44  | 		const employeeList = page.locator('div.MuiDataGrid-virtualScrollerContent');
  45  | 
  46  | 		await expect(
  47  | 			employeeList.getByText(employeeName, { exact: true }),
  48  | 		).toBeVisible();
  49  | 	},
  50  | );
  51  | 
  52  | Then(
  53  | 	'I should not see the employee {string} in the employee list',
  54  | 	async ({ page }, employeeName: string) => {
  55  | 		const employeeList = page.locator('div.xQueueList');
  56  | 
  57  | 		await expect(
  58  | 			employeeList.getByText(employeeName, { exact: true }),
  59  | 		).not.toBeVisible();
  60  | 	},
  61  | );
  62  | 
  63  | Then(
  64  | 	'I should see the {string} screen',
  65  | 	async ({ page }, screenName: string) => {
  66  | 		const screenTitle = page
  67  | 			.locator('span.pageName')
  68  | 			.getByText(screenName)
  69  | 			.last();
  70  | 
  71  | 		await expect(screenTitle).toBeVisible();
  72  | 	},
  73  | );
  74  | 
  75  | Then(
  76  | 	'I should see the {string} service',
  77  | 	async ({ page }, serviceName: string) => {
  78  | 		const service = page
  79  | 			.locator('li.ItemService')
  80  | 			.getByText(serviceName, { exact: true });
  81  | 		await expect(service).toBeVisible();
  82  | 	},
  83  | );
  84  | 
  85  | When(
  86  | 	'I add the {string} service to my cart',
  87  | 	async ({ page }, serviceName: string) => {
  88  | 		const service = page
  89  | 			.locator('li.ItemService')
  90  | 			.getByText(serviceName, { exact: true });
  91  | 
  92  | 		await service.click();
  93  | 	},
  94  | );
  95  | 
  96  | Then(
  97  | 	'I should see my cart showing {int} item added',
  98  | 	async ({ page }, itemCount: number) => {
  99  | 		const itemCountElement = page.locator(
  100 | 			'svg[data-testid="LocalPrintshopIcon"] + span',
  101 | 		);
  102 | 
  103 | 		await expect(itemCountElement).toBeVisible();
  104 | 
  105 | 		expect(itemCountElement).toHaveText(itemCount.toString());
  106 | 	},
  107 | );
  108 | 
  109 | When('I click on the {string} button', async ({ page }, buttonText: string) => {
  110 | 	const button = page.getByRole('button', { name: buttonText, exact: true });
  111 | 	await expect(button).toBeVisible();
  112 | 	await button.click();
  113 | });
  114 | When('I click on the {string} span', async ({ page }, spanText: string) => {
  115 | 	const span = page.locator('span', { hasText: spanText });
  116 | 	await expect(span).toBeVisible();
  117 | 	await span.click();
  118 | });
  119 | 
  120 | Then(
  121 | 	'I should see the text {string} visible',
  122 | 	async ({ page }, text: string) => {
  123 | 		await expect(page.getByText(text, { exact: true })).toBeVisible();
  124 | 	},
  125 | );
  126 | 
  127 | Then(
  128 | 	'I should see the button with id {string} visible',
  129 | 	async ({ page }, buttonId: string) => {
  130 | 		await expect(page.locator(`button#${buttonId}`)).toBeVisible();
  131 | 	},
  132 | );
  133 | 
  134 | When(
  135 | 	'I click on the element with id {string}',
  136 | 	async ({ page }, elementId: string) => {
  137 | 		const element = page.locator(`#${elementId}`);
```