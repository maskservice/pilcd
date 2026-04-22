# pilcd


👉 **DSI jest lepszy jeśli chcesz niski pobór prądu i mniejsze obciążenie systemu**
👉 **HDMI jest lepszy jeśli chcesz prostotę i kompatybilność**

---

# ⚡ Pobór prądu 

* **DSI:** ok. **1–2 W**
* **HDMI:** ok. **3–5 W** ([kadidisplay.com][1])

👉 czyli DSI potrafi zużywać nawet **~40% mniej energii** ([ODG Electronics][2])

Dodatkowo:

* DSI może być zasilany bezpośrednio z Raspberry Pi
* HDMI ekran zwykle ma **osobne zasilanie**

---

# 🧠 Obciążenie systemu (Debian / Raspberry Pi OS)

### DSI:

✔ niższe opóźnienia (<10 ms) ([kadidisplay.com][1])
✔ bezpośrednie połączenie z GPU
✔ mniej narzutu (brak konwersji sygnału)

### HDMI:

❌ większe opóźnienia (20–50 ms) ([kadidisplay.com][1])
❌ dodatkowa logika (HDMI → kontroler LCD)
❌ często osobny kontroler dotyku (USB)

👉 w praktyce:

* GUI działa płynniej na DSI (szczególnie dotyk)
* HDMI nie “zabija” CPU, ale jest mniej efektywne

---

# 🔌 Różnice praktyczne

| Cecha          | DSI         | HDMI          |
| -------------- | ----------- | ------------- |
| Pobór prądu    | 🔋 niski    | 🔌 wysoki     |
| Obciążenie     | 🟢 mniejsze | 🟡 większe    |
| Plug & play    | ❌ trudne    | ✅ łatwe       |
| Kompatybilność | ❌ mała      | ✅ ogromna     |
| Dotyk          | ✅ lepszy    | ❌ przez USB   |
| Rozdzielczość  | średnia     | bardzo wysoka |

---

# 🧠 Co wybrać w praktyce?

## 👉 Wybierz **DSI**, jeśli:

* robisz projekt embedded / kiosk / panel
* chcesz **minimalny pobór prądu**
* używasz dotyku
* ekran jest na stałe podłączony

## 👉 Wybierz **HDMI**, jeśli:

* chcesz coś co **po prostu działa**
* używasz monitora / TV
* testujesz / debugujesz system
* nie chcesz walczyć z driverami

---

# 💡 Najważniejszy wniosek

👉 Jeśli Twoim celem jest:

* **niski pobór prądu**
* **małe obciążenie systemu**
* **kompaktowy projekt**

➡️ **DSI wygrywa bez dyskusji**

👉 Jeśli Twoim celem jest:

* wygoda
* kompatybilność

➡️ **HDMI wygrywa**

---

# 🧩 Dla Twojego Waveshare

Twój:

* Waveshare 8" DSI

👉 to dobry wybór pod:

* kiosk
* panel sterowania
* projekt embedded
