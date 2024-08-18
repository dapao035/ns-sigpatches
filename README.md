#### 注意：按照此教程最后生成的 sigpatches 只适用于你选择的的系统固件版本以及大气层版本，不向上或向下兼容。
# 你都得准备点啥？
* 最新版 [IPS Patch Creator](https://gbatemp.net/download/ips-patch-creator-1-5-8.38703/)
* 下载你当前使用的设备系统固件。可以在 [Darthsternie's Firmware Archive](https://darthsternie.net/switch-firmwares/) 或 [THZoria/NX_Firmware](https://github.com/THZoria/NX_Firmware/releases) 进行下载。
* 下载你需要使用的[大气层](https://github.com/Atmosphere-NX/Atmosphere/releases)版本。
# 第一步 - 提取密钥
1. 解压下载好的 IPS Patch Creator。
2. 在解压好的文件夹中创建名为 Firmware 的文件夹，将下载好的系统固件压缩包中的所有文件解压到 `/Firmware/` 文件夹中。
3. 打开 `IPS_Patch_Creator.exe` 。转到 KeyData 选项卡并按 KeyGen 按钮，系统会要求您选择一个文件夹，选择刚刚创建的有最新系统的 `/Firmware/` 文件夹。
4. 会自动获取到对应系统的`keys.dat`，OK保存
# 第二步 - 生成签名补丁（sigpatches）
1. 在 IPS Patch Creator 文件夹中解压下载好的大气层压缩包。
2. 打开 `IPS_Patch_Creator.exe` 。在 IPS Creator 下的 Loader 选项卡中，点击文字框下方的 Make Patch 按钮。在弹出的对话框中选择解压的大气层中 `/atmosphere/` 文件夹中的 `package3` 文件，点击打开。
3. 切换至 ES 选项卡，点击 Make Patch 按钮。在弹出的对话框中选择 IPS Patch Creator 文件夹中的 `/Firmware/` 文件夹，点击确定。
4. 切换至 ES2 选项卡，点击 Make Patch 按钮。在弹出的对话框中选择 IPS Patch Creator 文件夹中的 `/Firmware/` 文件夹，点击确定。
5. 切换至 FS 选项卡，点击 Make Patch 按钮。在弹出的对话框中选择 IPS Patch Creator 文件夹中的 `/Firmware/` 文件夹，点击确定。
6. 切换至 NFIM 选项卡，点击 Make Patch 按钮。在弹出的对话框中选择 IPS Patch Creator 文件夹中的 `/Firmware/` 文件夹，点击确定。
# 第三步 - 完成
1. 将 IPS Patch Creator 文件夹中的 `atmosphere` 和 `bootloader` 两个文件夹复制到 SD 卡根目录。
   * 若提示有相同文件，选择覆盖即可。
2. 开玩！

