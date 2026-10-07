# 📦 BoxBuddy + Ubuntu sa Steam Deck Guide

Ito ang aking personal na gabay para sa pamamahala ng aking **Ubuntu container** gamit ang **BoxBuddy** sa SteamOS Desktop Mode.

---

## 🚀 1. Katayuan ng Aking Setup
* **BoxBuddy Application:** Naka-install at gumagana sa aking Steam Deck.
* **Linux Distribution:** Ubuntu subsystem/container ang kasalukuyang tumatakbo sa loob ng BoxBuddy.
* **Network Status:** Konektado at gumagana nang normal ang internet sa loob ng Ubuntu subsystem.

---

## 🛠️ 2. Paano Gamitin ang BoxBuddy Ubuntu Terminal

Kapag binuksan mo ang terminal ng iyong Ubuntu sa loob ng BoxBuddy, ito ang mga pangunahing utos na magagamit mo:

* **Mag-update ng System Packages (Ubuntu):**
  ```bash
  sudo apt update && sudo apt upgrade -y
  ```
  *(Paalala: Sa loob ng BoxBuddy Ubuntu, gumagana ang `apt` command dahil ito ay isang Ubuntu container, hindi tulad ng mismong SteamOS terminal na gumagamit ng `pacman`).*

* **Mag-install ng mga kapaki-pakinabang na tools:**
  ```bash
  sudo apt install curl ca-certificates -y
  ```

---

## 📌 Paalala sa Pag-aayos (Troubleshooting)
* **Kung sakaling hindi mabuksan:** Siguraduhing tumatakbo ang Flatpak or container system ng Steam Deck.
* **Network Verification:** Kung walang internet sa loob ng Ubuntu, i-restart ang BoxBuddy application o i-check ang iyong Huawei Wi-Fi router connection.
