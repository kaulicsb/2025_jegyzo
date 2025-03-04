# Jegyzőkönyv - Feszültség követő TL071-es Pinouttal, DAQK Oszcilloszkóppal és Funkció Generátorral

**Dátum**: 2025. február 4.  
**Készítette**: [Kaulics Balázs]

---

## Cél:
A TL071-es feszültség követő működésének vizsgálata és az eredmények megfigyelése DAQK oszcilloszkóppal és funkciógenerátorral.

---

## Használt eszközök:

- **TL071**: JFET bemeneti műveleti erősítő
- **DAQ Oszcilloszkóp**: Mérési és jel analízis
- **Funkció Generátor**: Szinusz, négyszög, háromszög és impulzusjelek generálása
- **Áramkör**: Feszültség követő (Buffer) áramkör

---

## TL071 Pinout:
A TL071 egy három lábas műveleti erősítő, az alábbi pinout szerint:

- **Pin 1 (Offset Null)**: Az offset feszültség beállításához
- **Pin 2 (Inverting Input, -)**: Inverz bemenet
- **Pin 3 (Non-Inverting Input, +)**: Nem inverz bemenet
- **Pin 4 (V-)**: Negatív tápegység csatlakozása
- **Pin 5 (Offset Null)**: Az offset feszültség beállításához
- **Pin 6 (Output)**: Kimeneti jel
- **Pin 7 (V+)**: Pozitív tápegység csatlakozása
- **Pin 8 (NC)**: Nem használt, szabad láb

---

## Módszer:

1. **Áramkör felépítése**:
   - A TL071-et feszültség követő (buffer) konfigurációban használtuk. A nem-inverz bemenet (pin 3) a bemeneti jelhez van csatlakoztatva, míg az inverz bemenet (pin 2) közvetlenül a kimeneti ponthoz (pin 6) csatlakozik.
   - A tápegység (V+ és V-) biztosítja a működéshez szükséges feszültséget.
   
2. **Jel generálás**:
   - A funkció generátor segítségével szinuszos jelet generáltunk különböző frekvenciákon (1 kHz és 10 kHz).
   - Az oszcilloszkópon figyeltük meg a bemeneti és kimeneti jeleket a TL071 működése alatt.

3. **Mérési és megfigyelési pontok**:
   - A bemeneti és kimeneti jeleket az oszcilloszkópon figyeltük, és megvizsgáltuk azok amplitúdóit és fáziskülönbségét.
   - A kimeneti jelnek pontosan követnie kellett a bemeneti jelet, mivel a TL071 feszültség követő funkciót lát el.

---

## Eredmények:

- A TL071 feszültség követő pontosan megközelítette a bemeneti jelet, minimális fáziskülönbséggel és nagyfokú linearitással.
- A bemeneti és kimeneti jel között nem volt mérhető fáziseltolódás (ideális feszültség követő működés).
- A TL071 kimeneti feszültsége a bemeneti jel szintjével megegyezett, azaz a jel nem volt erősítve, csak "átfolyt" rajta.

---

## Következtetés:

A TL071 feszültség követőként történő alkalmazása sikeres volt, az eszköz jól teljesítette a kívánt funkciót, és pontosan követte a bemeneti jelet. Az oszcilloszkóppal és funkciógenerátorral végzett mérések megerősítették, hogy a feszültség követő áramkör ideálisan működik.

---

## Munkafolyamat képei:

- ![Függvénygenerátor kép](https://github.com/user-attachments/assets/4806917d-2804-411b-a4da-73bd14d35d13)
- ![Osszcilloszkóp kép](https://github.com/user-attachments/assets/d1a8e603-40f1-4ede-8828-0d8c4ff5477d)


---

## Jegyzetek:

- A mért eredmények és az alkalmazott konfigurációk további elemzését a későbbiekben tervezem.
- További tesztelés szükséges különböző frekvenciák és jelformák alkalmazásával.
