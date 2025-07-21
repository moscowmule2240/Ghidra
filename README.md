# Readme
https://thinkit.co.jp/article/38169

# chocolatey
choco upgrade chocolatey -y

# java
choco install temurin -y

# ghidra
choco install ghidra --version=11.3.2 -y

# Ghidra Extension
hidra ExtensionをリポジトリのReleasesからZIPファイル(GhidraMCP-release-X-X.zip)をダウンロードしてください。

ダウンロードしたZIPファイルを解凍すると、ZIPファイルのGhidra Extensionのファイル(GhidraMCP-X-X.zip)が入っています。このファイルを解凍する必要はありません。ZIPのままGhidraに読み込ませることができます。

Ghidraを起動してFileメニューからInstall Extensionsを選択してください。新たに表示されたウィンドウで[+]ボタンをクリックしてください。

Select Extensionというウィンドウが表示されたら、先ほど解凍したGhidraMCP-X-X.zipを選択してください。

# Visual Studio Code  (GitHub Copilot)
GitHub Copilot's agent mode can connect to MCP servers over both stdio and sse. To set up GhidraMCP as a "tool" in VSCode's Copilot chat, you need to first make sure you are in "Agent" mode. Then, click on the tools icon in the chat box:

![image](https://github.com/user-attachments/assets/096c9639-c0f3-4217-bdab-f2a0f364ac9c)

In the drop down menu that appears, select "Add More Tools" and then "Add MCP Server"

![image](https://github.com/user-attachments/assets/9c7482d1-5cc5-4fa2-9bf4-e47b2a352304)

Select "Command (stdio)" and enter `python3 C:\path\to\bridge_mcp_ghidra.py --ghidra-server http://localhost:8080/` as the command. Make sure to replace the path to the Python script with the actual path on your machine.

![image](https://github.com/user-attachments/assets/400ae37c-4b9f-4101-a52b-eb316b09411d)

![image](https://github.com/user-attachments/assets/c57e510e-6ac5-436a-a560-44949d04eed3)

Lastly, give your MCP connection a name for VSCode.

![image](https://github.com/user-attachments/assets/e1f58c66-8c20-4f05-aa3a-392724c383b0)
