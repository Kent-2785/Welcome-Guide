# Welcome-Guide
![Image of Kent Logo](https://www.kent-school.edu/sites/default/files/styles/schoolyard_core_800_width/public/theme/logo.png) </br>
Brave coders of Kent Robotics taking on the unknown realm of coding: This page will help you get started with the coding environment. **Whoever's in charge should upgrade it at the start of the year**

# Setting Up The Environment:
Since you've decided to join Kent Robotics, follow these directions to get started with the coding environment:

1. Download JAVA and follow the instruction (I hope this is right): https://www.java.com/en/ </br>
2. Download VS Code for FRC: https://github.com/wpilibsuite/allwpilib/releases </br>
 2-1. Remember to install VS Code </br>
 ![Image to download VS Code](https://docs.wpilib.org/en/stable/_images/ExecuteInstall.png)
3. Download Pheonix Framework (Remember to download the lastest release): http://www.ctr-electronics.com/hro.html#product_tabs_technical_resources
4. Download Pheomix Firmware (Remember to download the lastest release): http://www.ctr-electronics.com/control-system/motor-control/talon-srx.html#product_tabs_technical_resources

# Getting Started with Code

1. Open VS Code and click on the WPI icon to access the Command Palette </br>
 ![Image for direction 1](https://docs.wpilib.org/en/stable/_images/wpilib-extension-commands.png)

2. Click on Create New Project </br>
 ![Image for direction 2](https://docs.wpilib.org/en/stable/_images/create-new-project.png)
 
3. Enter the fields accordingly </br>
 ![Image for direction 3](https://docs.wpilib.org/en/stable/_images/new-project-creator.png) </br>
 3-1: Project Type: The kind of project we wish to create. Select template. </br>
 3-2: Language: This is the language (C++ or Java) that will be used for this project. Select Java.</br>
 3-3: Project Base: If this is a template project, this specifies the type of template that will be used. Selected Command Robot(not the old type).</br>
 3-4: Project Location: This determines the folder in which the robot project will be located. </br>
 3-5: Create New Folder: If this is checked, a new folder will be created to hold the project within the previously-specified folder. If it is not checked, the project will be located directly in the previously-specified folder. An error will be thrown if the folder is not empty and this is not checked. </br>
 3-6: Project Name: The name of the robot project. This also specifies the name that the project folder will be given if the Create New Folder box is checked. </br>
 3-7: Team Number: The team number for the project, which will be used for package names within the project and to locate the robot when deploying code. Put in 2785. </br>

4. Click on the icon again and type in Manage Vendor Libraries. Click on Install new libraries (offline) </br>
 ![Image for direction 4](https://docs.wpilib.org/en/stable/_images/adding-offline-library.png)
5. Select the latest firmware version and install </br>

# Setting up the Robot(Do at the start of the year)

## Uninstall Old Software
1. Before installing the new version of the FRC Game Tools it is recommended to remove any old versions. The new version will likely co-exist with the old version (note that the DS will overwrite old versions), but all testing has been done with FRC 2020 only. Then click Start >> Add or Remove Programs. Locate the entry labeled “National Instruments Software”, and select Uninstall. </br>
![Image to software](https://docs.wpilib.org/en/stable/_images/uninstall_old_control_panel.png) </br>
2. In the dialog box that appears, select all entries. The easiest way to do this is to de-select the “Products Only” check-box and select the check-box to the left of “Name”. Click Remove. Wait for the uninstaller to complete and reboot if prompted. </br>
![Image to uninstall](https://docs.wpilib.org/en/stable/_images/uninstall_select_components.png)

## Install New Software
1. [New Software](https://www.ni.com/en-us/support/downloads/drivers/download.frc-game-tools.html#333285 "Link to new software") </br>
2. .NET Framework 4.6.2:The Game Tools installer may prompt that .NET Framework 4.6.2 needs to be updated or installed. Follow prompts on-screen to complete the installation, including rebooting if requested. Then resume the installation of the FRC Game Tools, restarting the installer if necessary. </br>
3. Follow the direction (I'm not gonna copy and reformat the instructions from FRC Docs. It's too long and I'm lazy)

## Imaging roboRIO(Robot Must be On)
1. Establish USB Connection: Connect a USB cable from the roboRIO USB Device port to the PC. This requires a USB Type A male (standard PC end) to Type B male cable (square with 2 cut corners), most commonly found as a printer USB cable. **(We have the cable in one of the boxes. It is black)** </br>
![Image of roboRIO](https://docs.wpilib.org/en/stable/_images/usb-connection.png) </br>
2. Launch Imaging Tool: The roboRIO imaging tool and latest image are installed with the NI FRC Game Tools. Launch the imaging tool by double clicking on the shortcut on the Desktop. If you have difficulties imaging your roboRIO, you may need to try right-clicking on the icon and selecting Run as Administrator instead. </br>
![Image of roboRIO tool](https://docs.wpilib.org/en/stable/_images/launching-the-imaging-tool.png) </br>
3. Update Firmware: roboRIO firmware must be at least v5.0 to work with the 2019 image. If your roboRIO is at least version 5.0 (as shown in the bottom left of the imaging tool) you do not need to update. To update roboRIO firmware: </br>
   -Make sure your roboRIO is selected in the top left pane.</br>
   -Select Update Firmware in the top right pane. </br>
   -Enter a team number in the Team Number box. </br>
   -Select the latest firmware file in the bottom right. </br>
   -Click the Update button. </br>
![Image to update firmware](https://docs.wpilib.org/en/stable/_images/imaging-the-roborio.png) </br>

## Pgrogramming The Radio
**Programmed Configuration:** </br>
![Config Image](https://docs.wpilib.org/en/stable/_images/radioLight.png) </br>

 **Pre-Requisites:** The FRC Radio Configuration Utility requires the Java Runtime Engine (JRE). If you do not have Java installed, you can download the JRE from here: https://www.java.com/en/download/ . The FRC Radio Configuration Utility requires Administrator privileges to configure the network settings on your machine. The program should request the necessary privileges automatically (may require a password if run from a non-Administrator account), but if you are having trouble, try running it from an Administrator account. </br>

1. Install Software: Download the software Download the latest FRC Radio Configuration Utility Installer from the following link: https://firstfrc.blob.core.windows.net/frc2020/Radio/FRC_Radio_Configuration_20_0_0.zip </br>
2. Allow the program to make changes in prompted
3. Use the pop-up window to select the which ethernet interface the configuration utility will use to communicate with the wireless bridge. On Windows machines, ethernet interfaces are typically named “Local Area Connection”. The configuration utility can not program a bridge over a wireless connection. </br>
   -If no ethernet interfaces are listed, click “Refresh” to re-scan for available interfaces. </br>
   -Select the interface you want to use from the drop-down list. </br>
   -Click “OK”. </br>
![Image for network](https://docs.wpilib.org/en/stable/_images/select-network-connection.png) </br>
4. Select a bridge model and operating mode: </br>
   -Select which radio you are configuring using the drop-down list. </br>
   -Select which operating mode you want to configure. For most cases, the default selection of 2.4GHz Access Point will be sufficient. If your computers support it, the 5GHz AP mode is recommended, as 5GHz is less congested in many environments. </br>
![Image for bridge model](https://docs.wpilib.org/en/stable/_images/select-bridge-model-mode.png)
5. Selected Options(Not really needed): The default values of the options have been selected to match the use case of most teams, however, you may wish to customize these options to your specific scenario: </br>
   -Robot Name: This is a string that gets appended to the SSID used by the radio. This allows you to have multiple networks with the same team number and still be able to distinguish them. </br>
   -Firewall: If this box is checked, the radio firewall will be configured to attempt to mimic the port blocking behavior of the firewall present on the FRC field. For a list of open ports, please see the FRC Game Manual. </br>
   -BW Limit: If this box is checked, the radio enforces a 4MB/s bandwidth limit like it does when programmed at events. Note that in AP mode, this is a total limit, not per client, so streaming video to multiple clients simultaneously may cause undesired behavior.  </br>
![Image for options](https://docs.wpilib.org/en/stable/_images/select-options.png)
6. Start the configuration and wait for it to complete.

#### Troubleshooting: Disabling Network Adapters
If you get an error message about “NPF adapter” when attempting to load firmware, you need to disable all other adapters. This is not always the same as turning the adapters off with a physical button or putting the PC into airplane mode. The following steps provide more detail on how to disable adapters. Go the Control Panel and search for **Change adapter settings**. For each adapter other than the one connected to the radio, right click on the adapter and select Disable from the menu. </br>
![Image for troubleshooting](https://docs.wpilib.org/en/stable/_images/disable-network-adapter.png)

# Building and Running the Code
To build and deploy a robot project, do one of (just pick 1 from 3): </br>
    1. Open the Command Palette and enter/select “Build Robot Code” (or) </br>
    2. Open the shortcut menu indicated by the ellipses in the top right corner of the VS Code window and select “Build Robot Code” (or) </br>
    3. Right-click on the build.gradle file in the project hierarchy and select “Build Robot Code” </br>
 ![Image to build robot code](https://docs.wpilib.org/en/stable/_images/building-code-options.png) </br>
 Deploy robot code by selecting “Deploy Robot Code” from any of the three locations from the previous instructions. That will build (if necessary) and deploy the robot program to the roboRIO. If successful, we will see a “Build Successful” message (2) and the RioLog will open with the console output from the robot program as it runs (1). </br>
 ![Image to deploy robot code](https://docs.wpilib.org/en/stable/_images/build-successful.png) 


# Useful Links

[FRC Dos](https://docs.wpilib.org/en/stable/ "FRC Lib Docs") </br>
[WPI API](https://first.wpi.edu/FRC/roborio/release/docs/java/ "FRC API") </br>
[Phenox Documentation for anything CTRE](https://phoenix-documentation.readthedocs.io/en/latest/index.html "Pheonix Documentation for anything CTRE") </br>
[Pheonix API](https://www.ctr-electronics.com/downloads/api/java/html/index.html "Pheonix API") </br>
