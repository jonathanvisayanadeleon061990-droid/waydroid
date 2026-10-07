# ⚠️ Waydroid Troubleshoot & Error Logs Cheatsheet

Ito ang listahan ng mga naging error sa aking Steam Deck (SteamOS Stable Channel) habang sinusubukang i-setup ang Waydroid at ang mga solusyon para rito.

---

## 🛑 1. Failed to connect to socket
* **Error Message:** `Waiting for waydroid container service... org.freedesktop.DBus.Error.FileNotFound: Failed to connect to socket`
* **Solusyon sa Terminal:**
  ```bash
  sudo systemctl start waydroid-container
  ```

---

## 🛑 2. Command Not Found (APT Error)
* **Error Message:** `sudo: apt: command not found`
* **Solusyon:** Ang SteamOS ay nakabase sa Arch Linux at hindi gumagamit ng `apt`. I-disable muna ang read-only protection kung kinakailangan:
  ```bash
  sudo steamos-readonly disable
  ```

---

## 🛑 3. Git Push Errors & Repository Not Found
* **Error Message:** `fatal: repository 'https://github.com' not found`
* **Solusyon:** Siguraduhing buo ang URL ng iyong repository bago mag-push:
  ```bash
  git remote set-url origin https://github.comjonathanvisayanadeleon061990-droid/waydroid.git
  git push -u origin master
  ```
