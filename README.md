# 🤖 Waydroid sa Steam Deck - Terminal Commands Cheatsheet

Ito ang aking personal na listahan ng mga madalas gamiting commands para sa pagpapatakbo, pag-stop, at pag-aayos ng Waydroid sa SteamOS Desktop Mode.

---

## 🚀 1. Pagpapatakbo at Pag-stop ng Waydroid

* **Simulan ang Waydroid Session:**
  ```bash
  waydroid session start
  ```

* **Buksan ang Waydroid UI (Android Screen):**
  ```bash
  waydroid show-full-ui
  ```

* **I-stop o Patayin ang Waydroid (Para makatipid sa RAM/Baterya):**
  ```bash
  waydroid session stop
  ```

---

## 🛠️ 2. Pamamahala sa System Services

* **Simulan ang Waydroid Container Container Service (Kailangan ng sudo password):**
  ```bash
  sudo systemctl start waydroid-container
  ```

* **I-restart ang Service kung nagka-error o nag-hang:**
  ```bash
  sudo systemctl restart waydroid-container
  ```

---

## 📦 3. Pag-install ng Apps (.apk)

* **Mag-install ng Android App gamit ang Terminal:**
  ```bash
  waydroid app install /path/to/your/app.apk
  ```

---

## 📌 Paalala sa Pag-update ng Notebook na ito:
Maaari kong i-edit ang file na ito direkta sa aking browser upang magdagdag ng mga bagong commands o solusyon sa mga errors na aking mararanasan.

