# How to Set the Path for Environment Variables in Java

Setting the path for environment variables is crucial to run Java programs from any directory on your system. Below are the steps for setting the path on different operating systems.

## Setting the Path in Windows

1. **Right-click** on `This PC` or `My Computer`.
2. Select **Properties**.
3. Click on **Advanced System Settings**.
4. In the System Properties window, click on the **Environment Variables** button.
5. In the Environment Variables window:
   - Under **System Variables**, scroll and find the variable named `Path`.
   - Select it and click **Edit**.
6. In the **Edit Environment Variable** dialog:
   - Click **New** and enter the path to the JDK’s `bin` directory.  
     Example:
     ```bash
     C:\Program Files\Java\jdk_version\bin
     ```
7. Click **OK** to close all dialog boxes and apply the changes.
8. **Verify** the path:
   - Open **Command Prompt**.
   - Type `java -version` and hit Enter to verify the Java installation.
