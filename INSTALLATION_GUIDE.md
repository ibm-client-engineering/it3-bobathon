# IBM Bob Installation & Setup Guide

This guide provides instructions for downloading, installing, and logging into IBM Bob on a personal computer (macOS, Windows, or Linux).

---

## 1. Download IBM Bob

Navigate to the download page in your browser:
👉 **[bob.ibm.com/download](https://bob.ibm.com/download)**

Select the installer corresponding to your operating system:

| Operating System | Architecture / Type | Installer Format |
| :--- | :--- | :--- |
| **macOS** | Apple Silicon (M1/M2/M3/M4) | `.pkg` (recommended) or `.dmg` (`mac-ARM`) |
| **macOS** | Intel Processor | `.pkg` (recommended) or `.dmg` (`mac-intel`) |
| **Windows** | 64-bit (x64) | `.exe` installer |
| **Linux (Debian/Ubuntu)** | x86_64 / amd64 | `.deb` package |
| **Linux (RHEL/Fedora)** | x86_64 | `.rpm` package |

> **macOS tip:** Check your chip type by clicking the Apple logo () in the top-left menu $\rightarrow$ **About This Mac** $\rightarrow$ **Chip** / **Processor**.

---

## 2. Install the Application

### Windows
1. Double-click the downloaded `.exe` installer.
2. Follow the setup wizard prompts (default installation path is recommended).
3. Click **Finish** once the installation completes.

### macOS
* **`.pkg` installer (recommended):** Double-click the downloaded `.pkg` file and follow the on-screen installation steps.
* **`.dmg` installer:** Double-click the downloaded `.dmg` file, then drag and drop the **IBM Bob** icon into your **Applications** folder.

### Linux
* **Debian / Ubuntu:**
  ```bash
  sudo apt install ./IBM-Bob-linux-amd64-*.deb
  ```
* **Red Hat / Fedora:**
  ```bash
  sudo dnf install ./IBM-Bob-linux-x64-*.rpm
  ```

---

## 3. Log In and Authenticate

1. Open **IBM Bob** from your Applications menu or Desktop shortcut.
2. On first launch, you will be prompted to sign in.
3. Your default web browser will open to `bob.ibm.com/login`.
4. Enter the email address associated with your Bob account / IBMid:
   * **Corporate SSO:** If your organization uses Single Sign-On (SSO), entering your work email will automatically redirect you to your company's identity provider.
   * **IBMid:** If your account uses standard IBMid authentication, enter your IBMid credentials.
5. After completing sign-in in the browser, return to the IBM Bob application. Your session will establish automatically.

---

## 4. Troubleshooting & Tips

* **Browser Redirect Issues:** If your browser does not open automatically, copy the login link displayed in the Bob IDE and paste it directly into your browser.
* **Firewall / Network:** If you encounter network connectivity errors when signing in on a restricted network, verify outbound HTTPS traffic is allowed to `*.ibm.com` and `bob.ibm.com`.
