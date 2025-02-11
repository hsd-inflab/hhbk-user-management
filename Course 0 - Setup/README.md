## Course 0: Setup

For the following courses you need to install (If you wish to use Java)

1) **Java 17** 
2) **VsCode** 

on your computer.

##### If you are working with your ***own*** computer, the installation process is shown below: 

<details>
<summary>WINDOWS</summary>

- First, install Chocolatey for easier package and Software installation:
  - open powershell as administrator (right-click: open as administrator) and run:
      ```powershell
      Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
      ```
  - Once the installation is completed, close the Powershell (Admin) or Terminal (Admin) and open it again and run the following commands:        

- Java Open JDK 17
  - via Chocolatey (recommended):
      ```powershell
      choco install oracle17jdk
      ```
  - or via installer (slower): [Adoptium Open JDK installer](https://adoptium.net/)
    
- Visual Studio Code
  - via chocolatey (recommended):  
    ```powershell
    choco install vscode
    ```
    
  - or via installer (slower): [Visual Studio Code Installer](https://code.visualstudio.com/)
    1) Download the vscode installer [from the official website.
      ](https://code.visualstudio.com/)

      ![](../images/48_download_vscode_installer.png)

    2) Locate the vscode installer on your computer (for example in Downloads)
       
       ![](../images/49_find_vscode_installer.png)

    3) Run the vscode installer
       
       ![](../images/50_run_vscode_installer_01.png)

       ![](../images/51_run_vscode_installer_02.png)

       ![](../images/52_run_vscode_installer_03.png)

       ![](../images/53_run_vscode_installer_04.png)

       ![](../images/54_run_vscode_installer_05.png)

       ![](../images/55_run_vscode_installer_06.png)
  
  
- [VSCode Java extension pack](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-pack)


- If you used chocolatey for installation, you can use the command
  ```powershell
  choco list
   ```
- if all installations worked, the output should look like this:
   ```powershell
  maven 3.9.9
  oracle17jdk 17.0.2
  scenebuilder 22.0.0
  vscode 1.94.2
  vscode.install 1.94.2
   ```
   
</details>

<details>
<summary>MACOS</summary>

- Homebrew (If wanted)
  - If wanted you can use homebrew to complete the following installation steps. [Homebrew](https://brew.sh) is a unofficial package manager for macOS, which should help you with installing new software on your system. To get started with homebrew just paste the following command inside your terminal window:
    ```
    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
    ```

- Java Open JDK 17
  - Either via installer: [Adoptium Open JDK installer](https://adoptium.net/)
  - Or via brew:
    ```
    brew install --cask temurin
    ```
- Visual Studio Code
  - Either via installer: [Visual Studio Code Installer](https://code.visualstudio.com/)
    1. Download the vscode App [from the official website.](https://code.visualstudio.com/)
    ![VSCode Download macOS](../images/macos_vscode_install_1.png)

    2. Install the app on your system. Simply drag and drop the downloaded `*.app` file into your Applications folder.
    ![VSCode Install macOS](../images/macos_vscode_install_2.png)
  - Or via brew:  
    ```
    brew install --cask visual-studio-code
    ```
- [VSCode Java extension pack](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-pack)
</details>


<details>
<summary>UBUNTU</summary>

- Java Open JDK 17
  ```bash
  sudo apt install openjdk-17-jdk
  ```
- Visual Studio Code
  - Either via installer: [Visual Studio Code Installer](https://code.visualstudio.com/)
  - Or via snap:  
    ```bash
    sudo snap install code --classic
    ```
- [VSCode Java extension pack](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-pack)
</details>

<br>

### Setup VsCode (do not skip this step!)

1) Click on the "Extension" Icon in the left panel
   
   ![](../images/56_setup_vscode_01.png)

2) search for `java extension pack` in the search field click on the first entry (NOTE: check that the distributor is MICROSOFT and no-one else) and click on the `Install` button to installer the extension pack. Wait until all extensions are installed.
   
   ![](../images/57_setup_vscode_02.png)
   
   ![](../images/58_setup_vscode_03.png)


You can check if your installations of java was successful by typing

```java --version```

into your local terminal.

Once you have finished these installations, you can continue with course 1.

