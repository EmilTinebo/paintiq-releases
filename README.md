# PaintIQ

**Från PDF-ritning till färdigt anbud – direkt på din egen dator.**

PaintIQ är ett program för kalkylatorer på måleriföretag. Du öppnar en ritning, mäter rum och ytor,
och programmet räknar fram material, arbetstid och pris enligt dina egna regler och din egen prislista.
Resultatet blir ett anbud som du kan skicka, och en kalkyl där varje rad går att följa tillbaka till
hur den räknades fram.

Programmet är byggt för att göra så mycket som möjligt automatiskt när det gäller att läsa ut skala,
mått och rum ur ritningen – men du ser alltid vad som mäts och kan dra i det. Priset bygger aldrig på
en gissning som du inte kan kontrollera.

> **Beta.** PaintIQ är under utveckling. Funktionerna nedan finns i den här versionen, men standardregelverkets
> tal (åtgångar, arbetstider, påslag) är exempelvärden som du ska justera efter ert företag innan du lämnar ett anbud.

## Vad programmet gör

**Ritningar**
- Öppna en eller flera PDF-ritningar per projekt, vektor- såväl som inskannade. Zooma, panorera och rotera sidor.
- Sätt skalan genom att mäta mot ett känt mått. PaintIQ kan också föreslå skala utifrån ritningen
  (skalangivelse eller dörrslag) – du bekräftar förslaget.

**Mätning**
- Mät längder direkt på ritningen. Mått sparas i millimeter och räknas om till ytor utifrån rummets takhöjd.
- Organisera mätningarna i rum, väggar, tak och öppningar (dörrar, fönster) med avdrag och smygar.
- Ångra och gör om hela vägen.
- Programmet frågar när något saknas – till exempel takhöjd, underlag eller behandling – i stället för att gissa.

**Priser och regler**
- Importera din prislista från Excel eller CSV, med kontroll av varje rad innan något sparas.
- Regelverket – vilka arbetsmoment ett material ger, mätregler, svårighetsfaktorer och påslag – är
  inställningar som du kan läsa och ändra, inte inbyggd logik. Ändringar sparas som nya versioner.

**Kalkyl**
- Se kalkylen i tre nivåer: översikt, per rum och per moment.
- Klicka på en rad och se hur den räknades fram, steg för steg.
- Slå av och på påslag och lägg till manuella justeringar.
- Spara kalkylen som en version, räkna om den senare och jämför två versioner rad för rad
  ("varför blev revision B 18 000 kr dyrare?").

**Anbud och export**
- Anbud som PDF med valfri detaljnivå: bara totalsumma, per rum, eller per rum och moment.
  Interna uppgifter som timpriser, materialåtgång och påslagsprocent visas aldrig för kunden.
- Hela kalkylen som Excel-fil, så att en kollega kan kontrollräkna.
- Projektpaket (`.paintiq`) med ritningar, mätningar och regler, för att dela ett projekt med en kollega.

## Dina uppgifter stannar hos dig

Ritningar, projekt och kalkyler lagras på din egen dator. Ingenting skickas till någon server när du
arbetar med ett projekt.

## Ladda ner

Hämta senaste versionen under **[Releases](../../releases/latest)**.

| System | Fil |
|---|---|
| Windows 10/11 (64-bit) | `PaintIQ-<version>-win-x64.exe` |
| macOS, Apple-processor (M1 eller senare) | `PaintIQ-<version>-mac-arm64.dmg` |
| macOS, Intel-processor | `PaintIQ-<version>-mac-x64.dmg` |

### Första start (versionerna är ännu inte kodsignerade)

Betaversionerna är inte signerade med något utgivarcertifikat, så operativsystemet varnar första gången.
Programmet är inte skadligt – varningen beror bara på att certifikatet saknas.

- **Windows:** när SmartScreen visar *Windows skyddade din dator*, välj **Mer info → Kör ändå**.
- **macOS:** dra PaintIQ till Program, högerklicka sedan på appen och välj **Öppna** (bekräfta i dialogen).
  Om macOS ändå vägrar, öppna Terminal och kör:
  `xattr -dr com.apple.quarantine /Applications/PaintIQ.app`

## Vart är det på väg

Riktningen är mer automatik: att läsa ut rum, mått och öppningar ur vektorritningar och föreslå dem för
dig att godkänna, så att mätningen går från manuellt arbete till kontroll. Det som kommer ut ur
ritningen är alltid förslag som du ser och bekräftar innan det påverkar priset.

## Feedback

Hittar du något som inte stämmer, eller saknar du något? Öppna ett ärende under
**[Issues](../../issues)**. Bifoga gärna inga kundritningar – beskriv vad som hände i stället.
