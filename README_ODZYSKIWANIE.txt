================================================================================
          INSTRUKCJA ODZYSKIWANIA SYSTEMU SECOND BRAIN I ASYSTENTA HERMES
================================================================================
Kiedy stosować:
- W razie awarii laptopa lub dysku.
- Po reinstalacji systemu Linux na laptopie.
- Po przeniesieniu środowiska na nowy komputer.

Do wyboru masz 2 niezależne, w pełni zautomatyzowane metody odzyskiwania:
METODA 1: Skrypt PowerShell (uruchamiany z Twojego komputera PC Windows)
METODA 2: Asystent Antigravity (uruchamiany poleceniem w czacie AI)

--------------------------------------------------------------------------------
METODA 1: ODZYSKIWANIE PRZEZ POWERSHELL (Z KOMPUTERA PC)
--------------------------------------------------------------------------------
Zastosowanie: Gdy wolisz jedno kliknięcie z poziomu Windowsa na stacjonarnym PC.

WYMAGANIA WSTĘPNE NA NOWYM/ODŚWIEŻONYM LAPTOPIE:
1. Laptop ma zainstalowany Linux (np. Linux Mint / Ubuntu), jest wpięty do sieci
   lokalnej i ma włączony serwer SSH:
   sudo apt install -y openssh-server && sudo systemctl enable --now ssh
2. Twój użytkownik to 'maciek', a hasło to Twoje standardowe hasło lokalne.

JAK URUCHOMIĆ ODZYSKIWANIE W POWERSHELL:
1. Na komputerze PC otwórz program PowerShell (wyszukaj 'PowerShell' w menu Start).
2. Przejdź do folderu drugiego mózgu poleceniem:
   cd "D:\second_braim"
3. Uruchom skrypt odzyskiwania:
   powershell -ExecutionPolicy Bypass -File .\Restore-Hermes.ps1

CO ROBI SKRYPT POWERSHELL:
- Łączy się z laptopem po SSH.
- Instaluje niezbędne pakiety (git, python3, pip, rclone, curl).
- Klonuje Twoje notatki z GitHuba (https://github.com/maciej-mycek/second-brain)
  do katalogu ~/Desktop/second brain/second brain/.
- Rozpakowuje zapisaną konfigurację Hermesa (SOUL.md, klucze .env, config.yaml,
  skrypty dojazdów i synchronizacji).
- Przywraca harmonogram zadań crontab (dojazdy 8:45, backup 3:00, raporty wt/pt 10:00).
- Włącza i uruchamia usługi systemd w tle (hermes-gateway, hermes-shopping-sync).
- Po 2-3 minutach cały system działa w identycznym stanie jak przed awarią.

--------------------------------------------------------------------------------
METODA 2: ODZYSKIWANIE PRZEZ ASYSTENTA ANTIGRAVITY (CZAT AI)
--------------------------------------------------------------------------------
Zastosowanie: Najprostsza metoda konwersacyjna. Nie musisz niczego klikać ani
pamiętać poleceń – asystent AI zrobi wszystko za Ciebie w tle.

JAK URUCHOMIĆ ODZYSKIWANIE PRZEZ ANTIGRAVITY:
1. Otwórz Antigravity na komputerze PC i rozpocznij nową sesję czatu.
2. Wklej do czatu poniższy komunikat (lub zbliżony):

   "Cześć, postawiłem świeży system na laptopie. Proszę przywróć całe środowisko
   Second Brain oraz konfigurację Hermesa z GitHuba i kopii zapasowej.
   IP laptopa to 192.168.1.42 (lub podaj aktualne IP, jeśli router zmienił)."

CO ZROBI ANTIGRAVITY:
- Asystent odczyta stałą regułę systemową (z zapisanymi ścieżkami i parametrami).
- Połączy się z laptopem bez pytania o hasło (używając skonfigurowanego klucza SSH).
- Skonfiguruje dostęp do GitHuba i pobierze repozytorium second-brain.
- Odtworzy archiwum logiki Hermesa, uprawnienia i pliki systemd.
- Zweryfikuje działanie bota Telegrama i zaraportuje Ci pomyślny wynik w czacie.

--------------------------------------------------------------------------------
GDZIE ZNAJDUJĄ SIĘ KOPIE ŹRÓDŁOWE:
--------------------------------------------------------------------------------
1. Baza notatek i wiedzy Obsidian:
   https://github.com/maciej-mycek/second-brain (repozytorium prywatne)
2. Mózg i logika Hermesa (SOUL.md, skrypty, usługi):
   Paczka: Archiwum_Fizyczne/Backups/hermes_logic_latest.tar.gz
   Kopia w chmurze: Dysk Google -> folder 'Archiwum_Second_Brain/Backups_Hermes_Logic/'
3. Ciężkie oryginały zdjęć, skanów i PDF:
   Dysk Google -> folder 'Archiwum_Second_Brain/'
================================================================================
