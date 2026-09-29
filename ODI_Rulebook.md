# ODI Rulebook v2 (data-backed)
Banaya: 28 Sep 2026 | Data: 2,576 ODI (Cricsheet, 15 Sep 2026 tak), 2,156 clean 50-over matches | Saath ki files: `ODI_Data_Book.xlsx` (har match ki poori detail), `ODI_Ball_By_Ball_CSV.zip` (har ball)

**Ek line mein:** yeh rulebook ab sirf yaad-dasht ki 4-5 matches par nahi, 2,156 matches ke asli numbers par hai. Kuch purane rules data ne sahi kiye, kuch galat nikle, neeche dono likhe hain.

---
## 0. Live match ka 60-second checklist
1. **Target dekho** (section 1 table): total kis band mein hai? Base chance kya hai?
2. **Chasing team ka record** (section 3): kya wo chase mein achhi hai ya kamzor?
3. **Ground** (Data Book, Grounds sheet): is ground par chase kaisa chalta hai?
4. **Ab ki state** (section 4 grids): overs, required rate, wickets down. Grid ka % lo.
5. **Market ka price** (1/odds) us % se compare karo. Agar market chase karne wali team ko data se bohot zyada de raha hai, wahan chase side par sambhal ke.
6. **Wicket cluster ka signal** (section 5): 20-40 overs mein 4+ wickets gire? Chase ka chance tezi se girta hai.
7. **Kabhi 100% mat maano:** 95% wali position bhi ~3-4% baar palat jaati hai (section 6).

---
## 1. Base rate: total ke hisaab se chase kitni baar jeeta
Sirf major teams (AUS, BAN, ENG, IND, NZ, PAK, SA, SL, WI) ek doosre ke against. "Chase %" = doosri batting karne wali team jeeti.

| 1st innings total | Chase % (all-time) | n | Chase % (2019 se) | n |
|---|---|---|---|---|
| 200 tak | 92% | 246 | 98% | 54 |
| 200-225 | 78% | 154 | 82% | 22 |
| 225-250 | 62% | 220 | 64% | 45 |
| 250-275 | 49% | 237 | 57% | 56 |
| 275-290 | 39% | 135 | 53% | 32 |
| 290-300 | 33% | 81 | 35% | 23 |
| 300-325 | 25% | 159 | 36% | 39 |
| 325-350 | 22% | 93 | 26% | 35 |
| 350-375 | 14% | 59 | 25% | 24 |
| 375+ | 2% | 43 | 0% | 19 |

**Sabak:** modern game (2019 se) mein chase pehle se zyada jeet-ta hai, khaaskar 275-375 band mein. Lekin 350+ target ab bhi 86% defend hota hai (2019 se, 43 matches). 375+ ko chase karna lagbhag na-mumkin raha (43 mein se sirf 1, wo bhi SA ka 438 wala match).

Yaad rakhne wale numbers: 300-325 par chase ka chance 25% (2019 se 36%). 250-275 par lagbhag 50-50.

---
## 2. Purane rules jo data ne sahi/galat kiye (honest report)
| Purana rule | Data ne kya dikhaya | Naya rule |
|---|---|---|
| "Chase team ka fast start = trap" | **Galat (average par).** Pehle 10 overs mein rate se 1.5+ upar to jeet 90% (n=118). 0.5-1.5 upar 78% (n=91). Rate se peeche 16%-34%. | Fast start **achhi cheez** hai. Lekin **300+ target** par 10 overs ke baad rate se upar hone par bhi jeet sirf ~41%-54% (n chhota: 17 aur 13). |
| "290-325 total defend hota hai" | **Sahi.** 290-300: 67% defend, 300-325: 75% defend (all-time). 2019 se thoda kam (65%, 64%). | Rakho, par modern ke liye ~65% samjho. |
| "Flat pitch par 350+ bhi chase ho jaata hai" | **Mostly galat.** 350-375: sirf 14% (2019 se 25%). 375+: 2%. | 350+ ko "defend" maano jab tak chase team ke 2-3 set batsman na hon. |
| "Low RRR + wickets haath mein = safe" | **Kaafi had tak sahi.** Model: 95%+ states mein 3.5% flip, 98%+ mein 0.8%. | Safe, par 100% nahi. Section 6 dekho. |
| "Middle overs mein spin squeeze se collapse" | **Data mein bowler type nahi**, isliye test nahi ho sakta. Lekin wicket cluster ka asar **confirm**: chase team rate se aage ho aur 20-40 overs mein 4 wickets gaye to jeet 67%, 6 gaye to 12%. | Spin ko watch-signal rakho, par asli trigger **wickets ka cluster** hai. |
| "Same series ka pattern follow karo" | Yeh data se test nahi hota (bahut chhota sample). | Tie-breaker ki tarah use karo, akele decider nahi. |

---
## 3. Team cards (major v major, 2019 se; Data Book > Teams)
| Team | Chase jeet % | n | Defend jeet % | n | Avg 1st score |
|---|---|---|---|---|---|
| India | 66% | 56 | 62% | 48 | 297 |
| New Zealand | 61% | 49 | 57% | 35 | 275 |
| Australia | 58% | 38 | 61% | 49 | 280 |
| Pakistan | 55% | 44 | 37% | 27 | 267 |
| South Africa | 51% | 35 | 53% | 36 | 281 |
| England | 49% | 35 | 46% | 41 | 292 |
| Bangladesh | 45% | 33 | 34% | 35 | 249 |
| West Indies | 44% | 36 | **10%** | 31 | 234 |
| Sri Lanka | **30%** | 23 | 43% | 47 | 246 |

- **Sri Lanka chase mein sabse kamzor** (30%). Isi wajah se ENG 1st ODI (265) aur 3rd ODI (356) mein haare.
- **West Indies defend karna nahi jaante** (10%, 31 mein 3 jeet). Is liye WI ke 295 par India ka chase favourite tha.
- **India sabse achha chaser**, Pakistan chase theek par defend kamzor.

Head to head (Data Book > Head to Head): AUS v SA 53 matches, chase 40% (2019 se 14 matches: chase 29%, avg 1st score 311). ENG v SL 39 matches, chase 46%. IND v WI 50 matches, chase 54%.

Grounds (clean matches): Wanderers 30 matches, avg 264, chase 50%. Kingsmead 19, avg 264, chase 47%. Headingley 16, chase 56%. Kennington Oval 39, avg 260, chase 62%. Riverside (Chester-le-Street) 13, chase 54%. Chhote samples, sirf hint ke liye.

---
## 4. Live grids: chase jeetne ka % (sabhi teams, asli history)
Rows = required rate (RRR), columns = wickets gire. "-" matlab 20 se kam examples.

**20 overs ke baad (30 baaki):**
| Required rate | 2 down | 3 down | 4 down | 5 down |
|---|---|---|---|---|
| 5 to 6 | 68% | 38% | 19% | 12% |
| 6 to 7 | 38% | 22% | 15% | 6% |
| 7 to 8 | 18% | 10% | 6% | 0% |
| 8 to 9 | 4% | 0% | 0% | - |
| 9 to 10 | - | - | - | - |

**30 overs ke baad (20 baaki):**
| Required rate | 2 down | 3 down | 4 down | 5 down | 6 down |
|---|---|---|---|---|---|
| 5 to 6 | 93% | 83% | 56% | 29% | - |
| 6 to 7 | 75% | 53% | 34% | 21% | 0% |
| 7 to 8 | 58% | 24% | 10% | 12% | 7% |
| 8 to 9 | - | 29% | 6% | 5% | 0% |
| 9 to 10 | - | - | 0% | 0% | - |

**40 overs ke baad (10 baaki):**
| Required rate | 2 down | 3 down | 4 down | 5 down | 6 down |
|---|---|---|---|---|---|
| 4 to 5 | - | 100% | 100% | 88% | - |
| 5 to 6 | - | 92% | 94% | 75% | - |
| 6 to 7 | - | 96% | 84% | 73% | 44% |
| 7 to 8 | - | 82% | 59% | 50% | 28% |
| 8 to 9 | - | - | - | 31% | 12% |

Poori grids (10, 35, 45 overs bhi) Data Book > Chase Odds mein.

Misaal: SA v AUS Wanderers, 237/4 (34.2 overs, 129 off 94, RRR 8.2): 35-overs wali grid (RRR 8-9, 4 down) ke hisaab se ~17%; model ne ~17% diya. Market ne AUS ko ~25% diya tha, AUS haara.

---
## 5. Wicket cluster aur fast start (Data Book > Collapse Patterns)
- 20 overs par rate se aage aur 2 ya kam wicket gire: chase 90% jeeta (n=157). Par target 325+ ho to sirf 50% (n=10).
- Aise chasers jo 20 overs par aage the, unka jeet %: 20-40 overs mein 0-1 wicket gaye → 100%, 2 → 92%, 3 → 83%, 4 → 67%, 6 → 12%.
- Matlab: **fast start se zyada, agle 20 overs mein wickets bachana** important hai. Set batsman ka jaana (Buttler retired hurt, Maharaj/Jacks jaise spell) is cluster ka trigger banta hai.

---
## 6. "Sure thing" bhi palat-ti hai? (Data Book > Reversals)
Model ne har over ke baad ki chase state ko score kiya, phir dekha kitni baar result ulta hua.

| Chase team ka win chance kabhi tak pahunchi | Odds (approx) | Matches | Chase HAARI | Flip rate |
|---|---|---|---|---|
| 90%+ | 1.11 | 1,154 | 77 | 6.7% |
| 95%+ | 1.05 | 1,079 | 38 | 3.5% |
| 98%+ | 1.02 | 973 | 8 | 0.8% |

Ulta: chase team 10% se neeche gir kar bhi **6.0%** baar jeeti (64/1,063), 5% se neeche **3.0%**, 2% se neeche **1.2%**.

**Jawab "2-3-4-5 paisa se bhi match palat-te hain?":** Haan, lekin rare. 1.05 par 100 mein ~3-4, 1.02 par 100 mein ~1. Isliye "pakka" nahi, par bohot kam risk.

Dataset ke bade flips (Data Book > Upsets): SA ne 2006 mein 435 chase kiya (5/1 se, model 0.1%). Australia ne 2014 Brisbane mein ENG ke 301 ko 244/9 (57 chahiye the, 36 balls baaki) se chase kiya. Sri Lanka 2010 MCG par 129 chahiye the 144 balls mein, 8 wicket gire hue, phir bhi jeeta. Chokes mein: SA 2011 Wanderers (145/4 se 189 all out, 1 run se haara vs India), Pakistan 2013 Sharjah (25 chahiye the 60 balls mein, 1 run se haara).

Dataset mein **nahi** (Afghanistan matches withheld): Maxwell ka 201* (AUS 91/7 se jeeta, 2023 WC). Wo aur 1996 WC SF (WI vs AUS) hamare notes se hain, dataset se nahi.

---
## 7. Hamare case files (27-28 Sep aur pichli series)
| Match | Kya hua | Data ne kya kaha | Lesson |
|---|---|---|---|
| SA v AUS 1st ODI, Durban | SA 297/8 ne AUS ko 230 par roka | 290-300 par chase 33% | Chasing team ne fast start liya, phir 9 wicket 101 par gire (cluster). |
| ENG v SL 2nd ODI, Leeds | SL 321/6 ne ENG ko 305/9 par roka | 300-325 par chase 25%-36% | ENG 143/0 tha, phir Wellalage aur Buttler ki injury. Bada target + cluster. |
| ENG v SL 1st ODI, Durham | ENG 265, SL 176 all out | 250-275 par chase 49%-57%, par SL ka chase record 30% | Team ka chase record + slow pitch + dot balls + middle order gir gaya. |
| ENG v SL 3rd ODI, Oval | ENG 355/7, SL haara | 350-375 par chase 14%-25%, SL 12/1 par | Bada target + early wicket. Model ne SL ko ~7% diya. |
| SA v AUS 2nd ODI, Wanderers | SA 365, AUS haara (237/4 se) | 350-375 band 14%-25%. 237/4 par ~17% | AUS ne ek hafte ke andar (24 aur 27 Sep) 2 baar same pattern dikhaya. Market ne AUS ko zyada diya. |
| IND v WI 1st ODI | WI 295/7, India ne aasaani se jeeta | 290-300 band 33%-35%, par India chase 66%, WI defend 10% | Team record band ke base rate se zyada important tha. |

---
## 8. Live decision flow
1. Target band se base rate lo (section 1).
2. Chase team ke record se adjust karo: India/NZ up, SL/WI/BAN down (section 3).
3. State grid se current chance lo (section 4).
4. Market ke 1/odds se compare karo. Agar market chase team ko data se 8-10 points zyada de raha hai, chase side par shak karo.
5. Agle 5-10 overs ke signals: set batsman, 4 wickets cluster, dot balls, injury.
6. Jis team ka koi khaas kamzori record (jaise SL chase) is series mein ek baar dikha chuka ho, use tie-breaker maano.

---
## 9. Limits (seedhi baat)
- Yeh sab **base rate** hain, guarantee nahi. n chhota ho (40 se kam) to number hilta hai.
- Data mein **pitch, weather, bowler type, toss ke baad ki conditions nahi** hain. Spin/seam wali baatein qualitative hain.
- Afghanistan ke 159 matches withheld hain. 22-27 Sep 2026 ke matches is dataset mein nahi.
- Market ke live odds main nahi dekh sakta. Aap apne screenshot se 1/odds nikaal kar section 8 step 4 karo.
- Jo paisa lagao wo wahi jo haarne par bhi theek ho. Koi bhi model 100% nahi.
