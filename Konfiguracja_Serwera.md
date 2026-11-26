# Konfiguracja Serwera

*Ostatnia aktualizacja: 2026-11-26*

## Dostęp SSH
- **Serwer:** `ssh maciek@192.168.1.42`

## Hermes Agent
- **Konfiguracja:** `~/.hermes/config.yaml`
  - Aktywny model: `gemini-4-neon`
  - `reasoning_effort: medium` (linia 1222)
- **Restart bramki Telegrama:**
  ```bash
  systemctl --user restart hermes-gateway.service
  ```

## Skrypty i bazy
- **Skrypt rozliczeń:** `~/.hermes/scripts/billing_check.py`
- **Baza stanu:** `~/.hermes/state.db`

## Second Brain (Obsidian)
- **Katalog notatek:** `/home/maciek/Desktop/second brain/second brain/`
