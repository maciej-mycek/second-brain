# 🛒 Stan prac nad 3-kierunkową listą zakupów (Garmin Fenix 8, Telefon, Hermes)
Data zapisu: 2026-11-14

## Co zostało już wdrożone i działa w 100%:
1. **Laptop / Hermes:**
   - Działa usługa systemowa w tle: `hermes-shopping-sync.service` (synchronizuje Google Tasks z plikiem `/home/maciek/Desktop/second brain/second brain/Zakupy.md`).
   - Skrypt zarządzający: `/home/maciek/.hermes/scripts/shopping_sync.py` (obsługuje dodawanie, odznaczanie, usuwanie i czyszczenie).
   - Hermes w `SOUL.md` ma regułę: gdy wyślesz na Telegramie zdjęcie (kartki, lodówki, zrzutu ekranu), analizuje je Vision i zasila listę zakupów.
   - Połączone konto Google: `konto.tanie.ai@gmail.com`.
2. **Garmin Fenix 8:**
   - Połączony przez Task Link (WCH Apps): `https://wchapps.com/app?watchAppId=f851eae5-b781-42de-9456-39d5b75deddd`.
   - Zsynchronizowana lista: `Lista zakupów`.

---

## Otwarty temat do decyzji po ponownym uruchomieniu PC:
**Pytanie użytkownika:** *Jakie są dalsze kroki z listą zakupów?*
**Kontekst:** Na oficjalnym widżecie Google Tasks na telefonie odznaczone artykuły znikają z pulpitu (Google Tasks nie ma w oficjalnym widżecie opcji pokazywania ukończonych na pulpicie, trafiają one tylko do wnętrza aplikacji do sekcji "Zrealizowane").

### Opcje do wyboru dla użytkownika:
1. **Opcja 1 (Rekomendowana): Widżet Tasks.org na telefonie**
   - Pozostajemy w 100% przy obecnym Google Tasks i obecnej konfiguracji zegarka Garmin.
   - Na telefonie instalujesz darmowy widżet `Tasks.org` (z Google Play) podłączony do tego samego konta `konto.tanie.ai@gmail.com`.
   - W ustawieniach widżetu włączasz opcję: *„Pokaż ukończone zadania”*.
   - **Efekt:** Na pulpicie telefonu odznaczone artykuły zostają na dole z widocznym przekreśleniem i czekają na usunięcie.

2. **Opcja 2: Zostajemy przy oficjalnej aplikacji Google Tasks bez zmian**
   - Pozycje na pulpicie znikają, ale po wejściu w aplikację Google Tasks na dole rozwijasz sekcję *„Zrealizowane”*, gdzie wszystkie są przekreślone.

3. **Opcja 3: Przejście na Google Keep lub Todoist**
   - Widżet Google Keep na pulpicie natywnie trzyma skreślone rzeczy na dole, ale wymagałoby to sprawdzenia obsługi Keep na zegarku lub użycia Todoist (który jest natywnie wspierany przez Task Link na Fenixie 8).