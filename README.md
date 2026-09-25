# SpartaBok – nedladdningar

SpartaBok är ett lokalt bokföringsprogram för svenska småföretag. Bokföringen lagras krypterad på din
egen dator. Det här repot innehåller bara färdiga versioner av programmet.

**Ladda ner den senaste versionen under [Releases](https://github.com/husiki/SpartaBok-releases/releases/latest).**

| System | Fil |
|---|---|
| Linux (x64) | `SpartaBok-<version>-linux-x64.tar.gz` |
| Windows (x64) | `SpartaBok-<version>-win-x64.zip` |
| macOS, Apple silicon | `SpartaBok-<version>-osx-arm64.zip` |
| macOS, Intel | `SpartaBok-<version>-osx-x64.zip` |

Varje release har en `SHA256SUMS.txt` som du kan kontrollera nedladdningen mot
(`sha256sum -c SHA256SUMS.txt --ignore-missing`).

## Installera

- **Linux:** packa upp och starta `SpartaBok`. Kör `./install-desktop-entry.sh` för att lägga till
  appen i programmenyn.
- **Windows:** packa upp och starta `SpartaBok.exe`. Programmet är ännu inte kodsignerat, så
  SmartScreen varnar första gången: välj *Mer information → Kör ändå*.
- **macOS:** packa upp och flytta `SpartaBok.app` till *Program*. Appen är inte notariserad, så
  första gången startar du den med högerklick → *Öppna*.

## Uppdatera

SpartaBok meddelar när en ny version finns (det går att stänga av under *Hjälp*). Ladda ner den nya
versionen och ersätt den gamla programmappen eller `SpartaBok.app`. Din bokföring ligger i en separat
datakatalog och påverkas inte. Om den nya versionen behöver uppgradera en databas sparas först en
kopia i bolagets `backups/`-mapp.

Säkerhetskopiera mappen `keys/` i datakatalogen separat: utan den går krypterad bokföring inte att
öppna efter en återställning.

Versioner märkta *Pre-release* är testversioner och erbjuds inte av uppdateringskontrollen.
