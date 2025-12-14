# Insurance Calculator (Auto Currency)

**Autorius / Author:** Donatas Vitenas  
**Statusas / Status:** Veikiantis prototipas (ribotos apimties) / Working prototype (limited scope)  
**Veikimo principas / Execution model:** vietinis (naršyklėje) / client-side (browser-based), su realiu valiutų kursų šaltiniu / using real currency rates

---

# 🇱🇹 LIETUVIŲ KALBA

## Apie projektą

Šis projektas yra **asmeninis, pilnai veikiantis draudimo kainų skaičiavimo sprendimas**, skirtas situacijoms, kai invoice pateikiamas užsienio valiuta, o galutinė kaina turi būti apskaičiuota ir pateikta **EUR**.

Tai **ne teorinis pavyzdys ir ne „mock“ aplikacija**.  
Skaičiavimai atliekami **realiu laiku**, naudojant **oficialius valiutų kursus**, todėl sprendimas gali būti naudojamas **praktiniame darbe**.

Projektas sukurtas kaip **nedidelės apimties, savarankiškai veikiantis įrankis**, tinkamas realiam naudojimui be papildomos infrastruktūros.

---

## Kam šis sprendimas reikalingas

Praktikoje dažnai pasitaiko situacijos, kai:
- invoice pateikiamas USD, GBP ar kita valiuta,
- draudimo pasiūlymas turi būti pateiktas EUR,
- valiutų kursai nuolat kinta,
- rankinis perskaičiavimas didina klaidų ir neatitikimų riziką.

Šis įrankis leidžia:
- **automatiškai konvertuoti invoice sumą į EUR**,
- naudoti **vieną patikimą ir oficialų valiutų kursų šaltinį**,
- sumažinti rankinį darbą ir žmogiškų klaidų tikimybę,
- turėti aiškų, pakartojamą ir skaidrų skaičiavimo procesą.

---

## Kaip veikia valiutų konvertavimas

Valiutų kursai gaunami iš **Frankfurter API**, kuris naudoja  
**Europos Centrinio Banko (ECB)** oficialius duomenis.

Tai reiškia, kad:
- naudojami **realūs, bankinėje praktikoje taikomi kursai**,
- duomenys nėra imituojami ar generuojami dirbtinai,
- nereikia API rakto ar autentifikacijos,
- sprendimas veikia **tiesiog naršyklėje (client-side)**.

Naudojamas šaltinis:

---

## Ką daro ši skaičiuoklė

- Automatiškai konvertuoja invoice sumą į EUR,
- Apskaičiuoja brokerio savikainą, kainą klientui ir pelną,
- Leidžia pasirinkti skirtingus procentinius scenarijus,
- Palygina skirtingus skaičiavimo variantus,
- Sugeneruoja **paruoštą tekstą klientui** (LT / EN / RU),
- Visi skaičiavimai atliekami **realiu laiku naršyklėje**.

---

## Kodėl projektas turi „ribotos apimties“ statusą

Nors sprendimas yra **funkcionalus ir praktiškai naudojamas**, jis turi sąmoningai nustatytas ribas:
- nėra serverio ar duomenų bazės,
- nėra naudotojų valdymo,
- nėra SLA ar ilgalaikio palaikymo,
- nėra integracijos su vidinėmis įmonių sistemomis.

Tai **nėra funkcionalumo trūkumas**, o sąmoningas sprendimas išlaikyti paprastumą ir patikimumą.

---

## Pastaba

Šis projektas yra **nekomercinis**, tačiau **funkcionaliai veikiantis**.  
Jis naudoja viešai prieinamus, oficialius valiutų kursų duomenis ir gali būti naudojamas praktinėse situacijose be papildomos infrastruktūros.

---

# 🇬🇧 ENGLISH VERSION

## About the project

This project is a **personal, fully functional insurance price calculation solution**, designed for cases where an invoice is issued in a foreign currency and the final price must be calculated and presented in **EUR**.

This is **not a theoretical example or a mock application**.  
All calculations are performed **in real time**, using **official currency exchange rates**, making the tool suitable for **practical use**.

The project is implemented as a **small, self-contained solution** that works without additional infrastructure.

---

## Why this solution is needed

In real business scenarios, it is common that:
- invoices are issued in USD, GBP, or other currencies,
- insurance offers must be presented in EUR,
- exchange rates constantly change,
- manual recalculation increases the risk of errors.

This tool allows users to:
- **automatically convert invoice amounts to EUR**,
- rely on **a single, official currency rate source**,
- reduce manual work and human error,
- maintain a clear and repeatable calculation process.

---

## How currency conversion works

Currency rates are retrieved from the **Frankfurter API**, which is based on  
**European Central Bank (ECB)** official exchange rates.

This means:
- **real, bank-grade exchange rates** are used,
- data is not simulated or artificially generated,
- no API key or authentication is required,
- the solution runs **entirely in the browser (client-side)**.

Data source:

---

## What the calculator does

- Automatically converts invoice amounts to EUR,
- Calculates broker cost, client price, and profit,
- Allows selection of different percentage scenarios,
- Compares calculation variants,
- Generates **ready-to-use client communication text** (LT / EN / RU),
- All calculations are performed **in real time in the browser**.

---

## Why the project has a “limited scope” status

Although the solution is **fully functional and usable**, it has intentionally defined limitations:
- no backend server or database,
- no user management,
- no SLA or long-term support commitments,
- no integration with internal enterprise systems.

These limitations are **deliberate design decisions**, not technical shortcomings.

---

## Disclaimer

This project is **non-commercial**, yet **fully functional**.  
It uses publicly available, official currency exchange data and can be used in practical scenarios without additional infrastructure.

---

© Donatas Vitenas
