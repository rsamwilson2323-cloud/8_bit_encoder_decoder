# ⚡ 8-Bit Encoder & Decoder — Text to Binary Converter

> **Every message has a binary story. Decode it. Encode it. Share it.**
>
> Convert plain text into 8-bit binary and decode binary back into readable text — instantly, using a lightweight, browser-based tool. No installation, no server, and no dependencies required.

---

## ✨ Features

🌐 **8-Bit Binary Encoding**
- Convert text into 8-bit binary representations.
- Each byte is displayed as a group of 8 bits.
- Automatically separates binary groups with spaces.
- Supports English text, symbols, numbers, and many Unicode characters through UTF-8.

🔓 **Binary Decoding**
- Convert 8-bit binary into readable text.
- Accept binary groups separated by spaces or new lines.
- Validate binary input before decoding.
- Display clear error messages for invalid input.

⚡ **Instant Conversion**
- Fast, browser-based processing.
- No API calls or backend server required.
- Works offline after the HTML file is available.
- No account or registration required.

🎨 **Modern User Interface**
- Stylish purple glass-inspired design.
- Dedicated Text → Binary and Binary → Text modes.
- Responsive layout for desktop, tablets, and mobile devices.
- Clean input fields and readable output panels.

📋 **Convenient Controls**
- Copy encoded binary with one click.
- Copy decoded text with one click.
- Clear input and output fields.
- Load example messages instantly.
- Real-time validation and status notifications.

🔒 **Privacy-Friendly**
- Text conversion takes place locally in your browser.
- No message uploads to a remote server.
- No database or account system.
- Your input is not intentionally transmitted by the application.

---

## 📂 Project Structure

```text
8_bit_encoder_decoder/
│
├── 8_bit_encoder_decoder.html   ← Complete web application
├── LICENSE                      ← Project license
└── README.md                    ← Project documentation
```

The entire application is contained in a single HTML file, including the HTML structure, CSS styling, and JavaScript logic.

---

## ⚙️ Installation

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/rsamwilson2323-cloud/8_bit_encoder_decoder.git
```

### 2️⃣ Open the Project Folder

```bash
cd 8_bit_encoder_decoder
```

### 3️⃣ Run the Application

Open `8_bit_encoder_decoder.html` in any modern web browser.

**Windows users:** Double-click `8_bit_encoder_decoder.html` to launch the application in your default browser.

✅ No installation process required.

---

## 📦 Requirements

```text
HTML5             Built-in browser support
CSS3              Modern interface and responsive styling
JavaScript        Encoding and decoding logic
TextEncoder       UTF-8 encoding
TextDecoder       UTF-8 decoding
Modern Web Browser Chrome, Edge, Firefox, etc.
```

**No additional dependencies are required.**

- No Node.js
- No Python
- No npm packages
- No database
- No backend server

---

## 🚀 Live Demo

You can run the application directly from your browser using GitHub Pages, once it has been enabled for the repository.

**Repository:**  
https://github.com/rsamwilson2323-cloud/8_bit_encoder_decoder

**Application file:**  
https://github.com/rsamwilson2323-cloud/8_bit_encoder_decoder/blob/main/8_bit_encoder_decoder.html

> To publish a live website, open the repository's **Settings → Pages**, select the `main` branch and `/ (root)` folder, and save. Once GitHub Pages publishes the site, the application will be accessible through its generated website URL.

---

## ▶️ Usage

### 📝 1. Encode Text into Binary

1. Open the application.
2. Select **Text → Binary**.
3. Enter a message in the text box.
4. Click **Encode to 8-bit**.
5. View the generated binary output.
6. Click **Copy binary** to copy the result.

**Example input:**

```text
I miss you
```

**8-bit binary output:**

```text
01001001 00100000 01101101 01101001
01110011 01110011 00100000
01111001 01101111 01110101
```

**Decoded message:**

```text
I miss you
```

### 🔓 2. Decode Binary into Text

1. Select **Binary → Text**.
2. Enter binary data using groups of 8 bits.
3. Separate each group with a space or a new line.
4. Click **Decode message**.
5. View the decoded text.
6. Click **Copy text** to copy the result.

**Example input:**

```text
01001000 01101001
```

**Decoded output:**

```text
Hi
```

### 🧹 3. Clear or Load Examples

- Click **Load example** to insert a sample message.
- Click **Clear** to remove the current input and output.
- Use the copy buttons to quickly reuse conversion results.

---

## 🧠 How It Works

### Text → Binary

The application uses JavaScript's `TextEncoder` to convert text into UTF-8 bytes. Each byte is then represented as an 8-bit binary number.

For example, the letter `H` has the ASCII value `72`.

```text
Character: H
Decimal:   72
Binary:    01001000
```

### Binary → Text

The decoder reads each group of 8 bits, converts it into a byte, and uses `TextDecoder` to reconstruct the original UTF-8 text.

```text
Binary:    01001000 01101001
Bytes:     72 105
Text:      Hi
```

### Conversion Flow

```text
       ENCODER
           │
           ▼
      Plain Text
           │
           ▼
      UTF-8 Bytes
           │
           ▼
     8-Bit Binary
           │
           ▼
       DECODER
           │
           ▼
    Readable Text
```

---

## 🛠️ Key Technical Details

| Feature | Implementation |
|---|---|
| Frontend | HTML5 |
| Styling | CSS3 |
| Application logic | Vanilla JavaScript |
| Text encoding | UTF-8 using `TextEncoder` |
| Text decoding | UTF-8 using `TextDecoder` |
| Binary representation | 8 bits per byte |
| Input validation | JavaScript regular expressions |
| Clipboard | Clipboard API with fallback selection |
| Data storage | None |
| Backend | Not required |
| Internet connection | Not required for conversion |

---

## 📌 Important Notes

- Each binary group must contain exactly **8 bits**, consisting only of `0` and `1`.
- Spaces and new lines can separate binary groups.
- Standard ASCII characters are represented by one byte each.
- UTF-8 characters outside the ASCII range may require multiple bytes.
- The binary output represents encoded data, not encrypted data.
- Anyone who knows the encoding format can decode the message.
- Clipboard functionality may depend on browser permissions and security restrictions.
- Very large inputs may be limited by available browser memory.

---

## 🚀 Future Improvements

- 🔗 Generate shareable encoded messages.
- 📄 Export binary output as a `.txt` file.
- 📂 Import text and binary files.
- 🔢 Add decimal, hexadecimal, and octal conversion.
- 🎨 Add light and dark themes.
- 📊 Display character count, byte count, and binary length.
- 📱 Improve the mobile interface with additional controls.
- 🔐 Add a separate encryption feature for secure messages.

---

## ⚠️ Disclaimer

This project is intended for educational and personal use. It demonstrates binary representation, UTF-8 encoding, and decoding using web technologies.

**This is an encoding tool, not a security or encryption tool.** Do not use plain binary encoding to protect sensitive information.

---

## 👨‍💻 Author

**Sam Wilson**

🌐 GitHub: https://github.com/rsamwilson2323-cloud

💼 LinkedIn: https://www.linkedin.com/in/sam-wilson-14b554385/

---

## 📜 License

This project is distributed under the license provided in the repository's `LICENSE` file.

---

<div align="center">

### ⚡ 8-Bit Encoder & Decoder

**From plain text to binary — and back again.**

*Built with HTML, CSS, and JavaScript.*

</div>
