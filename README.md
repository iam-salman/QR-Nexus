# 🚀 QR Nexus

A modern, feature-rich QR code generator built with Next.js and Tailwind CSS. Create, style, and download high-quality QR codes with an intuitive and responsive interface.

[**✨ Live Demo ✨**](https://your-website-link.com)

### Core Features

  - **⚡ Real-time Generation:** Instantly see your QR code update as you type.
  - **📝 Any Content:** Supports URLs, text, contact info, and more.
  - **🖼️ Logo Integration:** Brand your QR codes by uploading your own logo (PNG, JPG, SVG).

### Advanced Customization

  - **🎨 Color Control:**
      - **Single Color:** Independently set colors for the foreground, background, and eyes.
      - **Gradients:** Apply beautiful linear or radial gradients with full rotation control.
  - **🔮 Shape & Style:**
      - **Body Shape:** Choose from multiple dot styles (Square, Dots, Rounded, Classy).
      - **Eye Shapes:** Customize the eye frames and balls separately.
      - **Quiet Zone:** Adjust the margin for better scannability.
  - **✍️ Text Label:**
      - Add a custom text label below the QR code.
      - Style the label's font, size, color, and weight (bold/italic).
      - Set a background color for the label to make it pop.

### High-Quality Export

  - **📁 Multiple Formats:** Download as **PNG**, **JPEG**, **WEBP**, or **SVG** (vector).
  - **📏 Advanced Sizing:** Use the quality slider for quick exports or specify exact dimensions in **px**, **in**, **cm**, or **mm** for professional use.
  - **🧠 Intelligent Scaling:** Text labels and margins automatically scale with resolution.

### Powerful Bulk Generation

  - **📊 CSV Upload:** Generate hundreds of QR codes at once from a single `.csv` file.
  - **⚙️ Per-Row Customization:** Override global styles for each QR code directly from your CSV.
  - **📦 ZIP Download:** All generated codes are conveniently bundled into a single `.zip` file.

### Excellent User Experience

  - **🌗 Light & Dark Mode:** A sleek interface with automatic or manual theme switching.
  - **📱 Fully Responsive:** A seamless experience on desktop, tablet, and mobile.
  - **🔔 Notifications & Modals:** Get clear feedback with non-intrusive toasts and modals.

-----

## 💻 Technology Stack

  - **Framework:** [Next.js](https://nextjs.org/) / [React](https://reactjs.org/)
  - **Styling:** [Tailwind CSS](https://tailwindcss.com/)
  - **QR Engine:** [qr-code-styling](https://www.npmjs.com/package/qr-code-styling)
  - **Animation:** [Framer Motion](https://www.framer.com/motion/)
  - **Icons:** [Lucide React](https://lucide.dev/)
  - **Utilities:** [PapaParse](https://www.papaparse.com/) (CSV) & [JSZip](https://stuk.github.io/jszip/) (ZIP)

-----

## ⚙️ Getting Started

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/your-username/qr-nexus.git
    cd qr-nexus
    ```

2.  **Install dependencies:**

    ```bash
    npm install
    # or
    yarn install
    ```

3.  **Run the development server:**

    ```bash
    npm run dev
    # or
    yarn dev
    ```

-----

## 📄 Bulk Generation: CSV Format

Your `.csv` file needs a `data` column (required). All other columns are optional and override the UI settings for that row.

| Column | Required? | Description | Example |
|---|---|---|---|
| **`data`** | ✅ **Yes** | QR code content (e.g., URL, text). | `https://mywebsite.com` |
| `label` | No | Text below the QR code. | `Scan Me!` |
| `fgColor` | No | Foreground (dot) color. | `#FF5733` |
| `bgColor` | No | Background color. | `#FFFFFF` |
| `eyeFrameColor`| No | Color of the corner eye frames. | `#000000` |
| `eyeBallColor` | No | Color of the corner eye balls. | `#000000` |
| `gradientStart`| No | Starting color for a gradient. | `#8E2DE2` |
| `gradientEnd` | No | Ending color for a gradient. | `#4A00E0` |
| `dotType` | No | Style of the main QR dots. | `dots` |
| `labelColor` | No | Color of the text label. | `#333333` |
<<<<<<< HEAD
| `labelSize` | No | Font size of the label (in px). | `20` |
=======
| `labelSize` | No | Font size of the label (in px). | `20` |
>>>>>>> a17cc0fd636e04465f1c22ee7b690e5e45d045cf
