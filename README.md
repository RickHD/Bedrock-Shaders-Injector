# Bedrock Shaders Injector

**Version**: 1.0  
**Author**: [oRichter & ChatGPT]

[Leia em Português Brasileiro](README_pt-BR.md)

## 📑 Table of Contents
- [🚀 Overview](#-overview)
- [✨ Features](#-features)
- [🛠️ Technologies Used](#️-technologies-used)
- [📋 Requirements](#-requirements)
- [🔧 Installation](#-installation)
- [📖 Usage](#-usage)
- [❓ F.A.Q.](#-faq)
- [🤝 Contribution](#-contribution)
- [📜 License](#-license)
- [🙌 Acknowledgements](#-acknowledgements)

---

## 🚀 Overview
Bedrock Shaders Injector is a Windows PowerShell-based tool designed to simplify the process of replacing `.bin` shader files in Minecraft Bedrock Edition. With a user-friendly graphical interface, it allows you to manage shader files effectively and securely.

---

## ✨ Features
- **File Movement**: Automates the process of moving `.bin` files to the appropriate directory.
- **Graphical Interface**: Built using Windows Forms for an intuitive user experience.
- **Permission Management**: Temporarily grants and revokes folder permissions to ensure file operations.
- **Support for `.mcpack`**: Provides functionality to open and manage `.mcpack` shader files.
- **F.A.Q. Section**: Integrated FAQ to help resolve common issues.

---

## 🛠️ Technologies Used
- **PowerShell**: For scripting and automation.
- **Windows Forms**: To create the graphical user interface.
- **ICACLS**: To manage file permissions on Windows.

---

## 📋 Requirements
- **Operating System**: Windows 10 or later.
- **Minecraft Bedrock Edition**: Installed from the Microsoft Store.
- **PowerShell**: Version 5.0 or later.

---

## 🔧 Installation
1. **Download the script**:
   - Visit the [Releases Page](https://github.com/your-username/bedrock-shaders-injector/releases) to download the latest version.

2. **Prepare your environment**:
   - Ensure PowerShell is added to your system's PATH environment variable.
   - Run PowerShell as Administrator.

3. **Run the script**:
   - Open PowerShell in the script directory.
   - Execute the script:
     ```powershell
     .\BedrockShadersInjector.ps1
     ```

---

## 📖 Usage
1. **Launch the script**: Double-click the `.ps1` file or run it via PowerShell.
2. **Follow these steps in the GUI**:
   - Decide whether to use a `.mcpack` file.
   - Select the source folder containing `.bin` files.
   - Choose the destination folder (default is the Minecraft installation path).
   - Click "Move Files" to transfer shaders.
3. **Review the status**: Check the status label or dialog messages for operation success or errors.

---

## ❓ F.A.Q.
### 1. "PowerShell is not recognized as an internal or external command"
#### Solution:
1. Open "System Properties":
   - Press `Win + R`, type `sysdm.cpl`, and press Enter.
2. Navigate to the **Advanced** tab and click **Environment Variables**.
3. Under "System variables", find the variable named `Path` and click **Edit**.
4. Add the following directory to the list:
   ```
   C:\Windows\System32\WindowsPowerShell\v1.0
   ```
5. Click **OK** to save changes and restart your computer.

### 2. "ICACLS is not recognized"
#### Solution:
1. Ensure `ICACLS` is available on your system:
   - Open Command Prompt and type `icacls`. If the command is not recognized, proceed to the next step.
2. Check if the executable exists in the `System32` directory:
   - Navigate to `C:\Windows\System32` and search for `icacls.exe`.
3. If not found, ensure your Windows installation is complete and up to date.

### 3. "Access is denied"
#### Solution:
- Run the script as Administrator:
  1. Right-click on the `.ps1` script file.
  2. Select "Run as Administrator".

### 4. "Files not found or moved"
#### Solution:
- Verify the source folder contains valid `.bin` files:
  1. Confirm the correct source folder is selected.
  2. Ensure the `.bin` files are extracted if zipped.

### 5. "Issues with opening .mcpack files"
#### Solution:
- Ensure Minecraft Bedrock is associated with `.mcpack` files:
  1. Right-click the `.mcpack` file.
  2. Select "Open with" and choose Minecraft Bedrock.

---

## 🤝 Contribution
Contributions are welcome! Feel free to open an issue or submit a pull request if you have suggestions or improvements.

### Steps to Contribute
1. Fork the repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add your message here"
   ```
4. Push to the branch:
   ```bash
   git push origin feature/your-feature-name
   ```
5. Open a pull request.

---

## 📜 License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## 🙌 Acknowledgements
Special thanks to the Minecraft community and contributors who inspired this project.
