# 🌡️ Temperature Converter

A simple **Python GUI application** for converting temperatures between **Celsius, Fahrenheit, and Kelvin**.
Built with **Tkinter**, Python's standard GUI library.

---

## 🚀 Features

* Convert **Celsius ↔ Fahrenheit**
* Convert **Celsius ↔ Kelvin**
* Convert **Fahrenheit ↔ Kelvin**
* Simple and beginner-friendly interface
* Lightweight, no external dependencies required

---

## 🔢 Conversion Formulas

The program uses the standard temperature conversion formulas:

* **Celsius ➝ Fahrenheit**
  $F = \frac{9}{5} \times C + 32$

* **Fahrenheit ➝ Celsius**
  $C = \frac{5}{9} \times (F - 32)$

* **Celsius ➝ Kelvin**
  $K = C + 273.15$

* **Kelvin ➝ Celsius**
  $C = K - 273.15$

* **Fahrenheit ➝ Kelvin**
  $K = \frac{5}{9} \times (F - 32) + 273.15$

* **Kelvin ➝ Fahrenheit**
  $F = \frac{9}{5} \times (K - 273.15) + 32$

---

## ❓ Why 9/5?

The factor **9/5** (or **1.8**) appears because the interval between the freezing and boiling points of water is **100 degrees** on the Celsius scale (0°C → 100°C) and **180 degrees** on the Fahrenheit scale (32°F → 212°F). Therefore one Celsius degree equals 180/100 = 9/5 Fahrenheit degrees.

---

## 🖥️ How It Works

1. Enter a temperature value into the input box.
2. Select the unit you want to convert **from** and **to**.
3. Click **Convert**.
4. The converted result will appear in the output area.

---

## 🧭 User Flow

This section describes the typical user flow and the UI interactions in the app so contributors and designers can understand how users will move through the converter.

### Primary Flow (Convert a single value)

1. **Launch app** — The main window opens and shows:

   * an input field for the temperature value
   * a dropdown/select for the input unit (Celsius, Fahrenheit, Kelvin)
   * a dropdown/select for the output unit (Celsius, Fahrenheit, Kelvin)
   * a **Convert** button
   * a results area
2. **Enter value** — User types a numeric temperature into the input field.
3. **Choose units** — User selects the `From` unit and the `To` unit from the dropdowns.
4. **Convert** — User clicks **Convert**.
5. **Show result** — App validates the input, performs conversion using the formulas above, and displays the result (rounded as needed).
6. **Repeat or clear** — User may change the input or units and convert again, or click **Clear** to reset the form.

### Alternate Flows

* **Invalid input**: If the input is non-numeric or empty, the app shows an error message (e.g., "Please enter a valid number") and does not attempt conversion.
* **Same units selected**: If `From` and `To` units are the same, the app simply echoes the entered value (optionally formatting it) and may show a small note that units are identical.

### Optional Extra Flows

* **Swap units**: A `Swap` button toggles `From` and `To` units and immediately updates the result if an input exists.
* **History**: An optional history panel logs previous conversions with timestamp.
* **Precision control**: A settings area to choose decimal places for results.

### Simple ASCII Flowchart

```
[Start]
   |
[Open App]
   |
[Enter value] --> [Invalid?] -Yes-> [Show error] -> [Enter value]
   |No
[Choose From unit]
   |
[Choose To unit]
   |
[Click Convert]
   |
[Compute using formula]
   |
[Show result]
   |
[Repeat / Clear / Exit]
```

---

## 📦 Installation

Clone this repository:

```bash
git clone https://github.com/mrakakam/temp-converter.git
cd temp-converter
```

No extra installation needed, since **Tkinter comes pre-installed with Python**.

---

## ▶️ Usage

Run the program with:

```bash
python converter.py
```

---

## 📖 Example

**Input:** `100 °C`
**Output:** `212 °F` and `373.15 K`

---

## 🔧 Technologies Used

* **Python 3**
* **Tkinter** (built-in GUI library)

---

## 🤝 Contributing

Contributions are welcome!
Feel free to open an issue or submit a pull request.

---

## 📜 License

This project is licensed under the MIT License.

