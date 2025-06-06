# 适用于入门维修人员的 Windows 电脑维修指南

:calendar: 2025 年 4 月 15 日	多个参与者

本文提供在软件层面上的简易 Windows 电脑维修指南，适用于入门维修人员学习和参考。

**使用浏览器中的「在页面上查找」功能，或者目录快速定位问题和解决方法。**

> [!NOTE]
>
> 本文假定读者已有一定 Windows 计算机的基础认识，如果遇到任何**不能完全理解的操作**，**不要贸然尝试**。
>
> 本文主要提供维修思路而非针对每一种情况的手把手指导，实际维修时需要适当变通。



**本文内容**

[TOC]

## 无论如何先重启一次

无论遇到什么问题，重启都有可能解决，尤其那些偶发的问题。重启了问题仍复现再考虑着手修复。

> [!WARNING]
>
> **不到万不得已，不应当优先考虑在客户的设备上执行 重装系统、使用 DiskGenius 在 PE 中重分配磁盘空间 等可能具有毁灭性的操作。**
>
> **确认必须执行操作后，一定要告知客户可能存在的风险，做好备份准备，并且只允许在插电的情况下执行。**



## 只安装一个最合适的杀毒软件

现代 Windows 自带 Windows Defender 杀毒软件，在大多数情况下可以胜任全部杀毒要求。部分品牌自带的电脑管家包含杀毒功能（例如联想的联想电脑管家就是定制版火绒），不需要额外安装杀软。

杀毒软件监测系统会消耗资源、多个杀毒软件同时运行会导致计算机卡顿、耗电变快，甚至互相攻击，并且**不会变得更安全**。

部分杀软为盈利会携带广告弹窗以及捆绑安装行为。

> [!TIP]
>
> **如果客户的电脑已经安装了 2345、金山毒霸、McAfee、Avira、360（严重程度递减）中的一个或多个**
>
> 询问他们是否还需要这个（些）杀软。确认不需要或者不确定就卸载。
>
> **如果客户的电脑任务管理器中 `Antimalware Service Executable` 进程占据大量 CPU 算力**
>
> 此为 Windows Defender 出故障。考虑重启，或者安装火绒。



## 浏览器管理

### **在 Windows 上，推荐使用的浏览器有且仅有：**

| **名称**                            | **图标**                                                     | 优点                                                         | 缺点                                                         |
| ----------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Microsoft Edge                      | <img src="https://edgestatic.azureedge.net/shared/cms/lrs1c69a1j/section-images/2c3f3c46bd764335beec466a0acfde0e-png-w639.webp" alt="Microsoft Edge" style="zoom:10%;" /> | 与系统高度结合；功能强大易用；可以很方便地安装浏览器插件；手机电脑多端同步；很适合 PDF 阅读和批注。 | 臃肿；系统软件无法卸载。                                     |
| Mozilla Firefox<br />（火狐浏览器） | <img src="https://assets-prod.sumo.prod.webservices.mozgcp.net/media/uploads/products/2020-04-14-08-36-13-8dda6f.png" alt="https://assets-prod.sumo.prod.webservices.mozgcp.net/media/uploads/products/2020-04-14-08-36-13-8dda6f.png" style="zoom:40%;" /> | 自由开源浏览器，快速、安全、保护隐私，可以很方便地安装浏览器插件。 | 由于法律原因，国内无法在 Firefox 上安装广告拦截插件；有的网页不适配 Firefox；设置多而复杂；没有内置的网页翻译。 |
| Google Chrome<br />（谷歌浏览器）   | ![https://www.google.cn/chrome/static/images/chrome-logo-m100.svg](https://www.google.cn/chrome/static/images/chrome-logo-m100.svg) | 浏览器的代名词；（在国内大部分地方）纯粹快速的浏览器；外观现代简洁；快速。 | 由于不知道的原因，国内大部分地方在 Chrome 上安装插件和使用网页翻译需要额外付出努力；以及 Chrome 是被仿冒最多的浏览器之一，许多打着「AI」和「双核」浏览器的名号的仿冒浏览器会诱导下载，找到官网下载地址比较困难。 |

> **如何设置默认浏览器**
>
> 访问 [在 Windows 中设置默认应用](https://support.microsoft.com/zh-cn/windows/%E5%9C%A8-windows-%E4%B8%AD%E6%9B%B4%E6%94%B9%E9%BB%98%E8%AE%A4%E5%BA%94%E7%94%A8-e5d82cad-17d1-c53b-3505-f10a32e1894d)



### **推荐将下列页面的一个设置为主页：**

- 默认新标签页\*
- [go.itab.link](https://go.itab.link/)
- www.limestart.cn
- www.bing.com\*\*
- www.baidu.com\*\*

\* 对于 Microsoft Edge，默认新标签页含有新闻推送，考虑将页面布局设为「仅标题」。

\*\* 对于 Google Chrome，默认主页的搜索引擎绝大多数情况无法使用，将搜索引擎改为必应或百度，主页会随之变化。

> [!TIP]
>
> **如何更改主页**
>
> 访问 [更改浏览器主页](https://support.microsoft.com/zh-cn/microsoft-edge/%E6%9B%B4%E6%94%B9%E6%B5%8F%E8%A7%88%E5%99%A8%E4%B8%BB%E9%A1%B5-a531e1b8-ed54-d057-0262-cc5983a065c6)
>
> **如果客户的浏览器主页被劫持**
>
> 访问 [浏览器主页被劫持了怎么办？解决方法大全-知乎](https://zhuanlan.zhihu.com/p/480969879)



### **推荐使用 必应 作为搜索引擎**

> [!TIP]
>
> **如何更改搜索引擎**
>
> 访问 [在 Microsoft Edge 中更改默认搜索引擎](https://support.microsoft.com/zh-cn/microsoft-edge/%E5%9C%A8-microsoft-edge-%E4%B8%AD%E6%9B%B4%E6%94%B9%E9%BB%98%E8%AE%A4%E6%90%9C%E7%B4%A2%E5%BC%95%E6%93%8E-cccaf51c-a4df-a43e-8036-d4d2c527a791)



### **对于 Microsoft Edge，推荐安装下列扩展：**

- [AdGuard 广告拦截器](https://microsoftedge.microsoft.com/addons/detail/adguard-%E5%B9%BF%E5%91%8A%E6%8B%A6%E6%88%AA%E5%99%A8/pdffkfellgipmhklpdmokmckkkfcopbh)
- [沉浸式翻译](https://microsoftedge.microsoft.com/addons/detail/%E6%B2%89%E6%B5%B8%E5%BC%8F%E7%BF%BB%E8%AF%91-%E7%BD%91%E9%A1%B5%E7%BF%BB%E8%AF%91%E6%8F%92%E4%BB%B6-pdf%E7%BF%BB%E8%AF%91-/amkbmndfnliijdhojkpoglbnaaahippg)



### **卸载不用的或者来路不明的浏览器**

> [!WARNING]
>
> **卸载前务必确认客户没有历史记录、收藏夹和密码保管在浏览器中，如果有就不能卸载！**



## 默认应用设置

> [!TIP]
>
> **如何设置默认应用**
>
> 访问 [在 Windows 中设置默认应用](https://support.microsoft.com/zh-cn/windows/%E5%9C%A8-windows-%E4%B8%AD%E6%9B%B4%E6%94%B9%E9%BB%98%E8%AE%A4%E5%BA%94%E7%94%A8-e5d82cad-17d1-c53b-3505-f10a32e1894d)

### **推荐的默认应用**

**（推荐顺序从左往右递减、加粗的可以在 Microsoft Store 安装）：**

- 浏览器：**Microsoft Edge**、Mozilla Firefox、Google Chrome
- 音频和视频：**Windows 媒体播放器**、**mpv**、PotPlayer、**VLC**
- 图片：**Windows 照片**
- 文档：Microsoft 365（或其以年代结尾的衍生版本，例如 Microsoft Office 2024）\*、**WPS Office**
- PDF：**Microsoft Edge**、**Adobe Acrobat Reader\*\***、**WPS Office**
- 压缩包：7-zip、**NanaZip**、**Bandizip**

\* Microsoft 365 是按年/月订阅制的软件，Microsoft Office 20XX 是买断制软件。部分生产商附赠并预先安装 Microsoft Office 家庭和学生版 20XX（价值 798 人民币元）。如果用户没有 Microsoft 365 订阅，或者没有已激活的 Office，请为他们安装 WPS Office。

** Adobe Acrobat Reader 不能编辑 PDF，也不能将 PDF 转换为 Word，只能做简单的批注划线。高级功能为付费版 Acrobat 订阅者独占。

> PDF 转 Word 比较难，但 Word 转 PDF 只需要在 Word 中按 F12 另存为 PDF 文件！



## 卸载应用并去残留

安装 [Geek Uninstaller](https://geekuninstaller.com/download)

使用管理员权限运行 Geek Uninstaller，即可卸载软件并去除注册表等残余信息。

> [!TIP]
>
> 授人以鱼不如授人以渔，教会客户如何在控制面板或者设置正确卸载软件，最好也解释清楚**为什么删掉桌面快捷方式不是完全卸载**。
>
> 另外告知客户，某些软件会伪装卸载按钮，真正按钮可能是灰色小字。

> [!WARNING]
>
> **再三确认要卸载的软件客户的确不需要，并且没有重要信息保留！**



## 开机自启动管理

随意让任何软件开机自启拖慢开机速度，并且有可能导致故障

> [!TIP]
>
> **如果客户电脑上安装了火绒**
>
> - 火绒安全 → 扩展工具 → 启动项管理
> - 重点关注：
>     - 计划任务中的残留项（Task Scheduler 残留）
>     - 服务项中的第三方模块（非 Microsoft Corporation 签发）
>     - 资源管理器扩展（Explorer Shell Extension）
>
> > 其他杀软可能也携带此功能，多找找看
>
> **如果客户电脑上没有火绒并且没必要安装火绒**
>
> - 打开任务管理器 → 启动
> - 重点关注：
>     - 非驱动程序
>     - QQ、微信、钉钉、学习通（如果客户不想开机自启他们的话）
>     - 云盘、来路不明的软件

> [!WARNING]
>
> **不要错误禁用系统驱动服务，可能导致故障发生！**



## 高级重启

### 重启到安全模式

现代 Windows 不再支持开机时在 Windows Boot Manger （Windows 启动管理器）中按 `F8` 进入高级启动界面，这意味着我们进入安全模式的方式会改变。

如果需要进入安全模式，用户只能通过输入账户密码来解锁，指纹和人脸将不可用。

访问来自 DELL 的这篇 [帮助文档](https://www.dell.com/support/kbdoc/zh-cn/000124344/%E5%A6%82%E4%BD%95%E5%90%AF%E5%8A%A8%E8%BF%9B%E5%85%A5-windows-11-%E6%88%96-windows-10-%E7%9A%84%E5%AE%89%E5%85%A8%E6%A8%A1%E5%BC%8F)，查看操作视频。

**步骤**：

1. 点击开始菜单的电源按钮，按住 `shift` 同时鼠标点 「重启」
2. 重启后，选择「疑难解答」，然后选择「高级选项」，再选择「启动设置」
3. 选择 `4` 或 `F4` 以安全模式启动计算机。如果必须使用互联网，请选择 `5` 或 `F5` 以进入带网络连接的安全模式。

> [!IMPORTANT]
>
> 开启了**设备加密**的客户不仅需要输入锁屏密码，也需要获得他们设备的 BitLocker 恢复密钥。
>
> 界面形如：
>
> ### BitLocker
>
> 输入密钥以进行恢复
>
> [									]
>
> 恢复密钥 ID（用于识别密钥）: 45613A9F-6429-4914-A77D-0DBA32085CC5
>
> 驱动器标签：DESKTOP-A1B2C3D OS 2023/12/25
>
> 【继续】



> [!TIP]
>
> **解决步骤**：
>
> 1. 让客户在另一台设备访问 https://account.microsoft.com/devices/recoverykey 并登录自己的 Microsoft 账户
>
> 2. 这时会进入一个形如下面所示的页面：
>
>     > [!CAUTION]
>     >
>     > 保护好这页中的信息，不要外传。任何拥有这些信息的人可以在物理层面拿到你的硬盘后绕开保护机制完全控制其中数据！
>
>     ### BitLocker 恢复密钥
>
>     | 设备名称        | 密钥 ID  | 恢复密钥\*                                              | 驱动器 | 密钥上传日期 |
>     | --------------- | -------- | ------------------------------------------------------- | ------ | ------------ |
>     | DESKTOP-A1B2C3D | 45613A9F | 111111-222222-333333-444444-555555-666666-777777-888888 | OSV    | 2023/12/25   |
>     | DESKTOP-A1B2C3D | 123D45E6 | 112233-223344-334455-445566-556677-667788-778899-889900 | FDV    | 2023/12/25   |
>
> 3. 首先，我们知道前面驱动器标签给出了设备名称 `DESKTOP-A1B2C3D`，在客户名下有多台设备时可以定位第一列的设备
>
> 4. 随后，我们知道恢复密钥 ID 最开头一串是 `45613A9F`，看第二列哪个是 `45613A9F`，这时候我们已经可以确定例子中第一行第三列 `111111-222222-333333-444444-555555-666666-777777-888888` 是要输入进去的恢复密钥
>
> 5. 仔细输入正确的密钥，在电脑上点继续就能进入安全模式
>
> 
>
> \* BitLocker 的恢复密钥由 8 组 6 位 11 的倍数组成，此处瞎编了但没有完全瞎编。同样，如果输入 100000 这样显然不是 11 的倍数的数字出现就要再好好看清了

### 重启到 UEFI 和 PE

> [!NOTE]
>
> 很多电脑有开机进入 BIOS/UEFI 的快捷键，此方法稍麻烦但比较通用

进入上一节所述的高级启动界面，选择「故障排除」>「高级选项」>「UEFI 固件设置」

进入 UEFI 后选择启动设备为 PE 恢复 U 盘可以进入 PE

> [!IMPORTANT]
>
> 开启了**设备加密**的客户可能在进入 PE 时遇到问题



## 无线与网络

### 断网

如果客户电脑断网，首先排查所连接网络的问题。确认连接的网络密码正确，信号良好。

> [!TIP]
>
> **如果客户电脑上安装了火绒**
>
> - 火绒安全 → 扩展工具 → 断网急救箱
>
> - 点击「全面诊断」
>
> - **诊断结果处理**：
>     - 如果是黄色警告：表示有问题但可自动修复，点"立即修复"
>     
>     - 如果是红色错误：可能需要手动操作或联系网络运营商
>     
>     - 修复完成后建议重启电脑
>     
> - **能修复的问题**：
>
>     - DNS配置错误
>     - 网络协议异常
>     - 浏览器代理设置被篡改
>
> **如果客户电脑上没有火绒**
>
> - 尝试使用手机 USB 共享热点，看能否联网
>     - 如果 USB 共享热点可以连接网络但无线网络不行，考虑更新网卡驱动，或咨询生产商维修网卡。
>     - 如果 USB 共享热点也不能连接，需要咨询生产商维修网卡。

## 蓝牙

蓝牙鼠标、耳机无法连接时，查看其型号所对应的说明书以正确配对电脑。以及检查蓝牙开关的状态。

可能需要更新相关固件的驱动程序，如果没有改善需要咨询生产商维修。



## 磁盘空间清理与管理

对于现代 SSD，需要保留一部分空间完成 Trim。如果剩余空间不足可能导致客户系统卡顿。

一般来说系统会自己处理好 Trim，这一部分不需要干预。

> [!TIP]
>
> **打开「存储感知」**
>
> 在设置中搜索「存储感知」并开启，可以设定自动化清理（例如回收站文件满 30 天清理）
>
> **快速清理磁盘空间**
>
> 1. 运行「磁盘清理」工具（按 `Win+S` 搜索"磁盘清理"）
> 2. 勾选以下项目：
>     - 临时文件
>     - 下载的程序文件
>     - 缩略图
>     - 回收站（确认重要文件已备份）
> 3. 点击「清理系统文件」可删除 Windows 更新缓存
>
> **大文件定位技巧**
>
> - 使用 [TreeSize Free](https://www.jam-software.com/treesize_free) 可视化分析磁盘占用
> - 重点检查：
>     - `C:\Users\[用户名]\Downloads`
>     - `C:\Windows\Temp`
>     - `C:\Users\[用户名]\AppData\Local\Temp`



> [!WARNING]
>
> **不要手动删除以下内容**：
>
> - `System32` 文件夹内的文件
> - 任何你不认识的 .dll/.sys 文件
> - 未确认性质的 `Program Files` 文件夹内容



## 软件维修工具箱推荐

### **必备工具清单**

- PE启动盘：微PE工具箱

> [!IMPORTANT]
>
> 制作 PE 启动盘需要一个**不小于 4GB** 的闲置 U 盘，制作过程会**抹除 U 盘的全部数据**
>
> 涉及到重装系统，在 [MSDN，我告诉你](https://next.itellyou.cn/Original/) 使用 BT 磁力下载镜像。

- 卸载工具：Geek Uninstaller

- 系统修复：Dism++/WinNTSetup

- 磁盘管理：DiskGenius



## 服务质量保证

> [!IMPORTANT]
>
> 良好的服务流程比技术更重要！专业、耐心、透明的服务态度能显著提升客户信任度和问题解决效率

### **沟通要求**

- 使用简明的语言与客户交流，不要让专业术语把客户弄糊涂
- 保持尊重，**不要使用指责性表达**（“肯定是你弄错了”、“你想的不对”），也多加注意**不要造成对客户的贬低**（“这个不是很简单的吗”）
- 坦诚对待客户，如果自己能力有限修不了就如实告知，而不是贸然尝试

### **操作要求**

- 任何有破坏性的举动都要先告知客户，经过客户了解并同意了再操作
- **执行用时不确定且不允许中断的操作必须插电**
- 电脑重启可能需要客户输入密码，**不要去问客户的密码然后自己代为输入**，也**不要在客户输密码时旁观**
- 客户在不属于他的设备上登录任何东西，需提醒他退出登录

### **维修完成后务必做到**

1. 让客户当面验收所有功能
2. 教会用户如何处理再次出现的问题或如何避免问题