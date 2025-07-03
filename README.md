# 🚀 QR Nexus

A modern, feature-rich, and highly customizable QR code generator built with Next.js, React, and Tailwind CSS. Create, style, and download high-quality QR codes for personal or professional use with an intuitive and responsive interface.

[**Live Demo (Link to your deployed website)**](https://www.google.com/search?q=%23)


## ✨ Features

QR Nexus is packed with features to give you full control over your QR codes.

### Core Functionality

  - **Real-time Generation:** Instantly see your QR code update as you type.
  - **Any Content:** Supports URLs, text, and any other data you need to encode.
  - **Logo Integration:** Brand your QR codes by uploading your own logo (PNG, JPG, SVG).

### Advanced Customization

  - **Color Control:**
      - **Single Color:** Independently set the color for the foreground, background, and eye frames/balls.
      - **Gradient Foreground:** Apply beautiful linear or radial gradients with full rotation control.
  - **Shape & Style:**
      - **Body Shape:** Choose from multiple dot styles (Square, Dots, Rounded, Classy, etc.).
      - **Eye Shapes:** Customize the shape of the eye frames and eye balls separately.
      - **Quiet Zone:** Adjust the margin (quiet zone) around the QR code for better scannability.
  - **Text Label:**
      - Add a text label directly below the QR code.
      - Customize the label's font, font size, color, weight (bold), and style (italic).
      - Add a background color to the label for better visibility.

### High-Quality Export

  - **Multiple Formats:** Download your QR code as **PNG**, **JPEG**, **WEBP**, or **SVG** (vector).
  - **Simple & Advanced Download:**
      - **Simple Mode:** Use a single quality slider (from 300px to 4000px) for quick, high-resolution exports.
      - **Advanced Mode:** Specify exact dimensions for professional print or design work using units like **Pixels (px)**, **Inches (in)**, **Centimeters (cm)**, or **Millimeters (mm)**.
  - **Intelligent Scaling:** Text labels and margins automatically scale with the download resolution to maintain visual consistency.

### Powerful Bulk Generation

  - **CSV Upload:** Generate hundreds of QR codes at once by uploading a single `.csv` file.
  - **Per-Row Customization:** Override global styles for each QR code directly from your CSV file (e.g., set a different color, label, or content for each row).
  - **ZIP Download:** All generated codes are conveniently bundled and downloaded in a single `.zip` file.

### Excellent User Experience

  - **Light & Dark Mode:** A sleek, modern interface with theme support that respects your system preference or can be toggled manually.
  - **Fully Responsive:** A seamless experience on desktop, tablet, and mobile devices.
  - **Toasts & Modals:** Get clear feedback with non-intrusive notifications and user-friendly modals.
  - **Client-Side Navigation:** Fast and smooth navigation between pages (Generator, About, Help, Settings) using URL hashes.

## 💻 Technology Stack

This project is built with a modern, production-grade technology stack:

  - **Framework:** [Next.js](https://nextjs.org/) / [React](https://reactjs.org/)
  - **Styling:** [Tailwind CSS](https://tailwindcss.com/)
  - **QR Code Engine:** [qr-code-styling](https://www.npmjs.com/package/qr-code-styling)
  - **Animation:** [Framer Motion](https://www.framer.com/motion/)
  - **Icons:** [Lucide React](https://lucide.dev/)
  - **CSV Parsing:** [PapaParse](https://www.papaparse.com/)
  - **ZIP Archiving:** [JSZip](https://stuk.github.io/jszip/)

## ⚙️ Getting Started

To run this project locally, follow these steps:

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
    


## 📄 Bulk Generation: CSV File Format

To use the Bulk Generation feature, your `.csv` file must follow a specific format. The `data` column is required. All other columns are optional and will override the styles set in the UI for that specific row.

| Column                | Required? | Description                                                                                              | Example Value              |
| --------------------- | --------- | -------------------------------------------------------------------------------------------------------- | -------------------------- |
| **`data`** | **Yes** | The content to be encoded in the QR code.                                                                | `https://mywebsite.com`    |
| `label`               | No        | The text to display below the QR code.                                                                   | `Scan Me!`                 |
| `fgColor`             | No        | Foreground (dot) color.                                                                                  | `#FF5733`                  |
| `bgColor`             | No        | Background color of the QR code.                                                                         | `#FFFFFF`                  |
| `eyeFrameColor`       | No        | Color of the corner eye frames. Defaults to `fgColor` if not set.                                        | `#000000`                  |
| `eyeBallColor`        | No        | Color of the corner eye balls. Defaults to `fgColor` if not set.                                         | `#000000`                  |
| `gradientStart`       | No        | The starting color for a gradient. Overrides `fgColor`.                                                  | `#8E2DE2`                  |
| `gradientEnd`         | No        | The ending color for a gradient. Must be used with `gradientStart`.                                      | `#4A00E0`                  |
| `gradientType`        | No        | The type of gradient. Can be `linear` or `radial`.                                                       | `radial`                   |
| `dotType`             | No        | The style of the main QR dots.                                                                           | `dots`                     |
| `eyeFrameType`        | No        | The style of the corner eye frames.                                                                      | `extra-rounded`            |
| `eyeBallType`         | No        | The style of the corner eye balls.                                                                       | `dot`                      |
| `labelColor`          | No        | The color of the text label.                                                                             | `#333333`                  |
| `labelSize`           | No        | The font size of the text label (in px).                                                                 | `20`                       |
| `labelWeight`         | No        | The font weight of the text label.                                                                       | `900`                      |
| `labelItalic`         | No        | Whether the text label is italic.                                                                        | `true`                     |
| `labelFont`           | No        | The font family for the text label.                                                                      | `Roboto`                   |
| `labelBgColor`        | No        | The background color for the text label.                                                                 | `#EFEFEF`                  |

