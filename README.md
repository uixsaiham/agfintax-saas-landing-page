# AGFinTax SaaS Portal & Landing Redesign

A premium, interactive web portal and SaaS landing page redesign for **AGFinTax**. This project is built using the **Design Canvas / Omelette** client-side template framework, showcasing rich aesthetics, modern typography, glassmorphism, responsive grid layouts, and advanced micro-animations.

---

## 📂 Project Structure

Below is an overview of the key files and directories in this repository:

### 🌐 Pages & Templates (`*.dc.html`)
These are client-side templated pages that leverage the custom `<x-dc>` components:
*   **[AGFinTax Landing.dc.html](file:///c:/Users/user/Downloads/AGFinTax%20SaaS%20Landing%20redesign/uploads/AGFinTax%20intake%20redesign%20%281%29/AGFinTax%20Landing.dc.html)**: The primary public SaaS landing page. It showcases core tax services (Planning, Compliance, Advisory, Bookkeeping, R&D Credits, Wealth Management), case studies for targeted audiences (Small Business Owners, Real Estate Investors, etc.), and recent resources.
*   **[AGFinTax App.dc.html](file:///c:/Users/user/Downloads/AGFinTax%20SaaS%20Landing%20redesign/uploads/AGFinTax%20intake%20redesign%20%281%29/AGFinTax%20App.dc.html)**: The primary application layout. Contains the onboarding milestone tracker side-navigation, progress logic, and acts as the wrapper/shell for the onboarding steps.
*   **[AGFinTax Intake.dc.html](file:///c:/Users/user/Downloads/AGFinTax%20SaaS%20Landing%20redesign/uploads/AGFinTax%20intake%20redesign%20%281%29/AGFinTax%20Intake.dc.html)** & **[AGFinTax Intake v2.dc.html](file:///c:/Users/user/Downloads/AGFinTax%20SaaS%20Landing%20redesign/uploads/AGFinTax%20intake%20redesign%20%281%29/AGFinTax%20Intake%20v2.dc.html)**: Interactive multi-step onboarding/intake wizard flows for gathering entity details, filing preferences, and document uploads.
*   **[Dashboard.dc.html](file:///c:/Users/user/Downloads/AGFinTax%20SaaS%20Landing%20redesign/uploads/AGFinTax%20intake%20redesign%20%281%29/Dashboard.dc.html)**: The client portal homepage featuring upcoming milestones, documents overview, messaging center, and status cards.
*   **[Consult.dc.html](file:///c:/Users/user/Downloads/AGFinTax%20SaaS%20Landing%20redesign/uploads/AGFinTax%20intake%20redesign%20%281%29/Consult.dc.html)**: Consultation scheduling page with advisor details and questionnaire forms.
*   **[Implement.dc.html](file:///c:/Users/user/Downloads/AGFinTax%20SaaS%20Landing%20redesign/uploads/AGFinTax%20intake%20redesign%20%281%29/Implement.dc.html)**: Real-time onboarding status tracking page for document review and validation.
*   **[Report.dc.html](file:///c:/Users/user/Downloads/AGFinTax%20SaaS%20Landing%20redesign/uploads/AGFinTax%20intake%20redesign%20%281%29/Report.dc.html)**: Final reports & tax delivery center, featuring visual summaries, interactive feedback requests, and secure signature integration.

### 🛠️ Runtime & Assets
*   **[support.js](file:///c:/Users/user/Downloads/AGFinTax%20SaaS%20Landing%20redesign/uploads/AGFinTax%20intake%20redesign%20%281%29/support.js)**: The core compiler and component parser for the **Design Canvas** runtime system. It compiles `<x-dc>` elements, parses props, and runs custom template directives (like `<sc-for>` and `<sc-if>`).
*   **[image-slot.js](file:///c:/Users/user/Downloads/AGFinTax%20SaaS%20Landing%20redesign/uploads/AGFinTax%20intake%20redesign%20%281%29/image-slot.js)**: The Web Component implementation for `<image-slot>`, handling customizable image shapes, cropping, masks, and stock-photo fallbacks.
*   **[uploads/](file:///c:/Users/user/Downloads/AGFinTax%20SaaS%20Landing%20redesign/uploads/AGFinTax%20intake%20redesign%20%281%29/uploads)**: Contains logo assets, test PDFs, and preview images referenced dynamically in the interface layouts.

---

## 🚀 Design System & Technology Stack

1.  **Core Syntax**: HTML templates embedded within `<x-dc>` parent wrappers, featuring custom component syntax like `<sc-for>` and `<sc-if>`.
2.  **Styles**: Plain, highly-optimized CSS in `<style>` blocks using premium curated typography (**Satoshi** from Fontshare, **Inter** from Google Fonts) and standard layout APIs (Flexbox, Grid).
3.  **Client-Side Reactivity**: Enabled through `support.js` which registers and renders bindings using React and ReactDOM under the hood.

> [!NOTE]
> Some pages (e.g. `AGFinTax Landing.dc.html`) reference external asset files at `../../assets/`. When hosting or packaging this repository, ensure that the relative paths are correct or update them to point to your hosted assets.

---

## 🖥️ How to Run & View Locally

To preview these pages locally, run a local web server in the project directory.

### Option 1: VS Code Live Server
Right-click on any `.dc.html` file (e.g. `AGFinTax Landing.dc.html`) and select **"Open with Live Server"**.

### Option 2: Python HTTP Server
Run the following command in your terminal:
```bash
python -m http.server 8000
```
Then navigate to `http://localhost:8000` in your web browser.

### Option 3: Node.js (npx serve)
Run the following command:
```bash
npx serve .
```
Then visit the URL displayed in the console (usually `http://localhost:3000`).
