# ⚡️ AirShare: 局域网隔空快传工具

> **LAN Peer-to-Peer File Transfer Tool.** Zero setup, zero dependencies. Share files and text across Mac, Windows, and iOS via a single browser page.

## 🔗 访问链接 (Access URL)

请在您的浏览器中打开此地址以启动应用：

[**https://wen7.space/**](https://wen7.space/)

---

## 🚀 核心特性 (Key Features)

| 中文描述 | Description |
| :--- | :--- |
| **⚡️ 极速传输 (Lightning Fast):** 基于 WebRTC (点对点通信)，文件在设备间直接传输，速度取决于您的局域网环境。 | Built on WebRTC (Peer-to-Peer), files transfer directly between devices. Speed is limited only by your local network (LAN) environment. |
| **🌐 零配置 (Zero Configuration):** 无需安装 App 或运行命令行，只需一个浏览器标签页。 | No need to install apps or run command line interfaces (CLI). All you need is a single URL. |
| **🛡️ 隐私安全 (Privacy Guaranteed):** 文件经过加密，**绝不会**上传到任何服务器（包括 GitHub 或您的主机）。 | Files are encrypted and **never** uploaded to any server (including GitHub or your host). |
| **💻 跨平台 (Cross-Platform):** 完美支持 Mac、Windows、iOS、Android 手机浏览器。 | Seamlessly supports browsers on Mac, Windows, iOS, and Android. |

---

## 💡 如何使用 (How to Use)

AirShare 的工作原理是：先开一个房间（主机），然后其他设备扫码或者输入配对码加入（访客）。

### 1. 启动主机 (Launch the Host)

在您希望发送或接收文件的主设备（Mac/Windows）上，打开网址。

- 在页面上输入配对码生成主机。
- 在需要接收或者发送的设备上输入配对码。
- 页面会自动生成一个独特的 **二维码** 。
- 此设备将保持为 **主机状态**，等待连接。

### 2. 扫码连接 (Connect the Guest)

在另一台设备（iPhone/Windows/Mac）上：

- 使用 **相机** 或 浏览器 **扫描主机页面上显示的二维码**。
- 访客设备将自动尝试建立连接。

### 3. 开始互传 (Start Transferring)

- 一旦连接状态变为 **"✅ 已安全连接"**，双方即可开始互传。
- **发送文件：** 将文件直接拖拽到页面中央的虚线框内。
- **接收文件：** 文件传输完成后，点击列表中的 **"下载"** 按钮即可保存。

---

## 🔒 安全性与隐私声明 (Security & Privacy Statement)

**AirShare 的设计核心在于保护您的数据，我们无法获取您的任何文件。**

| 概念 | 中文说明 | 英文说明 |
| :--- | :--- | :--- |
| **文件不经服务器** (No Server Middleman) | AirShare 使用 WebRTC DataChannel 技术。这意味着文件数据是 **点对点 (P2P)**，直接从您的设备 A 传输到设备 B，中间不经过托管服务器。 | AirShare utilizes the **WebRTC DataChannel** technology. File data is **Peer-to-Peer (P2P)**, moving directly from your device A to device B without passing through the hosting server. |
| **仅用于信令 (Signaling Only)** | GitHub Pages 或您的服务器，仅用于托管 UI 代码和 WebRTC 握手的 **信令 (Signaling)** 信息，只负责让两台设备找到对方。 | The hosting server is only used for serving the UI code and facilitating the **Signaling** process (like a phone book connecting two parties). |
| **自动加密 (Mandatory Encryption)** | WebRTC 连接强制使用 DTLS 和 SRTP 协议，您的数据在传输过程中是默认**加密**的。 | WebRTC connections enforce the use of DTLS and SRTP protocols, ensuring your data is **encrypted** during transmission by default. |

---
