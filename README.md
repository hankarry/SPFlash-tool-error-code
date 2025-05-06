# SPFlash-tool-error-code 报错代码合集-中文

## 1. BROM 错误 


### 1.1 S_UNKNOWN_TARGET_BBCHIP 

**描述** 
 
- 不支持的目标基带芯片类型！

**解决方案** 
 
- 请升级到最新版 Flash Tool 并重试。



---



### 1.2 S_UNSUPPORTED_VER_OF_BOOT_ROM 

**描述** 
 
- 不受支持的 Boot ROM 版本！

**解决方案** 
 
- 请升级到最新版 Flash Tool 并重试。



---



### 1.3 S_SEC_INFO_NOT_FOUND 

**描述** 
 
- 当前 ROM 文件未启用安全特性！启用安全的基带必须配合启用安全的 ROM 文件启动。

**解决方案** 
 
- 请使用启用安全特性的 ROM 文件后再试。



---



### 1.4 S_UART_CHKSUM_ERROR 

**描述** 
 
- **硬件** ：通过 UART 回读 SEC_RO 或 CUST_PARA 时，校验和与 BROM DLL 计算值不一致！

**解决方案** 
 
- 请检查 UART 连接线是否稳定。



---



### 1.5 S_BROM_DOWNLOAD_DA_FAIL 

**描述** 
 
- **硬件** ：无法将 DA 下载到基带芯片内部 SRAM！

**可能原因** 
 
2. Flash Tool 与 Boot ROM 之间的通讯线路异常。
 
4. 目标设备意外关机或失去供电。
 
6. 选择的 DA 文件不正确。

**解决方案** 
 
2. 重试一次。
 
4. 检查下载线及目标设备端口硬件。
 
6. 监控目标设备是否掉电。



---



### 1.6 S_BROM_BBCHIP_HW_VER_INCORRECT 

**描述** 
 
- **硬件** ：目标基带芯片与所选镜像文件不匹配！

**解决方案** 
 
- 请选择与目标基带芯片匹配的镜像文件。



---



### 1.7 S_BROM_FAIL_TO_GET_BBCHIP_HW_VER 

**描述** 
 
- **硬件** ：无法获取目标基带芯片硬件版本！

**可能原因** 
 
2. Flash Tool 与 Boot ROM 之间的通讯线路异常。
 
4. 目标设备可能意外关机。

**解决方案** 
 
2. 重试一次。
 
4. 检查下载线及目标设备 UART 通路。
 
6. 监控目标设备是否掉电。



---



### 1.8 S_BROM_AUTOBAUD_FAIL 

**描述** 
 
- **硬件** ：已发送 Boot ROM 启动命令，但自动协商波特率失败！

**可能原因** 

同 1.7。
**解决方案** 
 
2. 重试。
 
4. 在高级模式（**Ctrl + Alt + V** ）启用“加速 Boot ROM 波特率”后再试。
 
6. 检查硬件连线。
 
8. 监控目标掉电情况。



---



### 1.9 S_BROM_SPEEDUP_BAUDRATE_FAIL 

**描述 / 原因 / 解决方案** 
 
- 与 **1.8**  相同。



---



### 1.10 S_BROM_EXCEED_MAX_DATA_BLOCKS 

**描述** 
 
- **MAUI** ：多文件下载数量超过 10 个！

**解决方案** 
 
- 请避免生成超过 10 个二进制文件。



---



### 1.11 S_DA_INT_RAM_ERROR 

**描述** 
 
- 下载的镜像与手机内部存储不匹配。

**解决方案** 
 
- 选择与手机存储匹配的正确镜像后重试。



---



### 1.12 S_DA_EXT_RAM_ERROR 

**描述** 
 
- **硬件** ：DA 未检测到外部 RAM。

**解决方案** 
 
- 可能是 SMT 或 EMI 问题，请使用另一部手机尝试下载。



---



### 1.13 S_DA_RAM_FLOARTING 

**描述** 
 
- **硬件** ：DA 检测到 DRAM 浮空。

**解决方案** 
 
- 格式化全部闪存，或换机重试。



---



### 1.14 S_DA_DEVICE_NOT_FOUND 

**描述** 
 
- **硬件** ：DA 未检测到外部 SRAM/DRAM。

**可能原因** 
 
2. SMT 或 EMI 问题。
 
4. NOR/NAND 尚未验证。

**解决方案** 
 
- 请更换设备尝试下载。



---



### 1.16 S_DA_NAND_UNSUPPORTED_DEV_ID 

**描述** 
 
- 不支持的 NAND Flash 类型！

**解决方案** 
 
- 升级到最新版 Flash Tool 后重试。



---



### 1.18 S_DA_NAND_FLASH_NOT_FOUND 

**描述** 
 
- **硬件** ：DA 未检测到 NAND Flash。

**可能原因** 
 
2. SMT 问题。
 
4. NFI 问题。
 
6. NOR/NAND 尚未验证。

**解决方案** 
 
- 确认镜像与手机匹配后换镜像再试。



---



### 1.21 S_DA_NAND_PAGE_PROGRAM_FAILED 

**描述** 
 
- **硬件** ：DA 写页失败。

**可能原因** 
 
- SMT 问题。

**解决方案** 
 
- 存储可能损坏，请换机下载。



---



### 1.22 S_DA_NAND_SPARE_PROGRAM_FAILED 

**描述 / 原因 / 解决方案** 
 
- 与 **1.21**  相同。



---



### 1.23 S_DA_NAND_BLOCK_DATA_UNSTABLE 

**描述** 
 
- **硬件** ：擦除后区块数据不稳定。

**解决方案** 
 
- 格式化全部闪存或换机下载。



---



### 1.28 S_DA_INVALID_RANGE 

**描述** 
 
- 某个下载镜像的地址或长度无效。

**解决方案** 
 
- 重新选择正确的 scatter 文件，确保地址合法后重试。



---



### 1.31 S_DA_BLANK_FLASH 

**描述 / 解决方案** 
 
- **用户** ：闪存中不存在 MAUI 代码及 SEC_RO（可选）。



> 与描述相同。



---



### 1.32 S_DA_CODE_AREA_IS_BLANK 

**描述** 
 
- **用户** ：闪存中不存在 MAUI 代码。

**解决方案** 
 
- 请选择 MAUI 文件进行下载。



---



### 1.33 S_DA_SEC_RO_AREA_IS_BLANK 

**描述** 
 
- **用户** ：闪存中不存在 SEC_RO（可选）。

**解决方案** 
 
- 请选择 SEC_RO 文件（可选）进行下载。



---



### 1.34 S_DA_UNSUPPORTED_BBCHIP 

**描述** 
 
- **用户** ：当前 BROM DLL 版本过旧，不支持此基带芯片！

**解决方案** 
 
- 升级到最新版 Flash Tool 并重试。



---



### 1.39 S_FT_SET_DOWNLOAD_BLOCK_FAIL 

**描述** 
 
- DA_MEM_CMD 执行失败。

**可能原因** 
 
2. 下载区块超出目标闪存大小。
 
4. 起始地址未按字对齐。
 
6. 长度非字对齐。

**解决方案** 
 
- 使用其他镜像重新下载。



---



### 1.40 S_FT_DOWNLOAD_FAIL 

**描述** 
 
- 写入闪存失败！

**解决方案** 
 
- 按 **Ctrl + Alt + T**  打开调试日志后再次下载。



---



### 1.41 S_FT_READBACK_FAIL 

**描述** 
 
- 读取闪存失败！

**解决方案** 
 
- 按 **Ctrl + Alt + T**  打开调试日志后重新回读。



---



### 1.42 S_FT_NAND_READADDR_NOT_PAGE_ALIGNMENT 

**描述** 
 
- **用户** ：NAND 回读起始地址未按页对齐。

**解决方案** 
 
- 请检查回读起始地址。



---



### 1.43 S_FT_NAND_READLEN_NOT_PAGE_ALIGNMENT 

**描述** 
 
- **用户** ：NAND 回读长度未按页对齐。

**解决方案** 
 
- 请检查回读长度。



---



### 1.44 S_FT_ENABLE_DRAM_FAIL 

**描述** 
 
- **EMI** ：启用 DRAM 失败。

**解决方案** 
 
- 确认镜像与设备匹配后重新下载。



---



### 1.45 S_DL_GET_DRAM_SETTING_FAIL 

**描述** 
 
- **EMI** ：获取 DRAM 设置失败！

**解决方案** 
 
- 检查所用镜像是否与目标机型匹配。



---



### 1.46 S_FT_OTP_ADDR_NOT_WORD_ALIGNMENT 

**描述** 
 
- **用户** ：OTP 操作地址未按字对齐！

**解决方案** 
 
- 请重新确认 OTP 地址。



---



### 1.47 S_FTHND_FILE_IS_NOT_LOADED_YET 

**描述** 
 
- 文件尚未加载！

**解决方案** 
 
2. 检查 DA 路径是否正确。
 
4. 确认所有 ROM 文件存在。
 
6. 验证 scatter 描述与实际 ROM 同步。



---



### 1.48 S_FTHND_LIST_IS_EMPTY 

**描述** 
 
- 下载/回读列表为空或全部被禁用！

**解决方案** 
 
- 至少选择一个条目；**Android**  机型需先加载 scatter 文件。



---



### 1.49 S_DL_REMOTE_FILE_UNSUPPORTED_BY_BL_AUTOLOAD 

**描述** 
 
- **用户** ：Boot Loader 镜像位于远程服务器。

**解决方案** 
 
- 请使用本地电脑中的 Boot Loader 镜像。



---



### 1.50 S_DLIST_BBCHIP_HW_VER_NOT_MATCHED 

**描述** 
 
- **硬件** ：基带芯片与 scatter 文件不匹配！

**解决方案** 
 
- 选择正确的 scatter 文件并重试。



---



### 1.51 S_UNSUPPORTED_VER_OF_AUTH_FILE 

**描述** 
 
- **用户** ：认证文件版本不受支持！

**解决方案** 
 
- 确认使用的是最新版 Flash Tool。



---



### 1.52 S_DL_PROJECT_ID_DIFF_BETWEEN_MAIN_CODE_AND_JUMP_TBL 


> *仅标题，原文未给出描述与解决方案。*



---



### 1.53 S_DL_SCAT_OPEN_FAIL 

**描述** 
 
- **用户** ：无法打开 scatter 文件！

**解决方案** 
 
- 检查 scatter 文件是否存在且未被占用。



---



### 1.54 S_DL_UNSECURE_MAUI_TO_SECURE_BB 


> *仅标题，原文未给出描述与解决方案。*



---



### 1.55 S_SECURITY_SLA_INVALID_AUTH_FILE 

**描述** 
 
- **用户** ：使用了无效的认证文件！

**解决方案** 
 
- 该错误只在 MSP (MTK Secure Platform) 代码中出现，请保持 MSP 版本一致并寻求支持。



---



### 1.56 S_SECURITY_SF_SECURE_VER_CHECK_FAIL 

**描述** 
 
- **用户** ：secure-MAUI 的安全版本低于手机内版本！

**解决方案** 
 
- 请选择安全版本相同或更新的 secure-MAUI。



---



### 1.57 S_SECURITY_SF_HANDSET_SECURE_CUSTOM_NAME_NOT_MATCH 

**描述** 
 
- **用户** ：secure-MAUI 的定制名与手机内不一致！

**解决方案** 
 
- 请选择定制名一致的 secure-MAUI。



---



### 1.58 S_SECURITY_SECURE_CUSTOM_NAME_NOT_MATCH_BETWEEN_AUTH_AND_DL_HANDLE 

**描述** 
 
- **用户** ：认证文件中的定制名与 secure-MAUI 不一致！

**解决方案** 
 
- 认证文件与 secure-MAUI 的定制名必须一致。



---



### 1.59 S_PART_NO_VALID_TABLE 

**描述** 
 
- NAND Flash 无有效分区表！

**解决方案** 
 
- 确认目标机已正确刷写，选择“格式化全部 + 下载”后重试！



---



### 1.60 S_PART_NO_SPACE_FOUND 

**描述** 
 
- 未找到分区表可用空间！

**解决方案** 
 
- 请格式化全部后重新下载。



---



### 1.61 S_DA_UPDATE_BOOTLOADER_FILE_SIZE_EXCEEDS_BOUNDARY_ADDR 

**描述** 
 
- DA 下载引导加载器超出分区边界！

**解决方案** 
 
- 引导区坏块过多，请做物理全格后重刷。



---



### 1.62 S_SECURITY_DAA_FAIL 

**描述** 
 
- DA 安全下载错误！

**解决方案** 
 
- Security DA 未用正确密钥签名，请选择正确 DA 后重试。



---



### 1.63 S_DA_UPDATE_BOOTLOADER_EXIST_MAGIC_NOT_MATCHED 

**描述** 
 
- DA 检测 DSP_BL 失败。

**解决方案** 
 
- 目标机之前的固件无 DSP_BL，格式化全部后重新下载。



---



## 2. Flash Tool 错误 


### 2.1 FT_FIND_USB_ERROR 

**描述** 
 
- **Android USB** ：无法找到 USB 端口！

**解决方案** 
 
2. 目标设备电量不足，请插入电池。
 
4. 数据线硬件问题，请更换。
 
6. 如使用 USB 集线器，可能存在漏电。
 
8. 未安装 Android 下载驱动，请先安装对应驱动。



---



### 2.2 FT_FIND_GADGET_USB_ERROR 

**描述** 
 
- **Android USB** ：无法找到 Gadget Serial USB 端口！

**解决方案** 

与 2.1 相同，但第 4 条需安装 Gadget Serial USB 驱动。


---



### 2.3 FT_DL_PLATFORM_ERROR 

**描述** 
 
- **平台错误** ：加载文件与目标设备不一致！

**解决方案** 
 
- 依据目标设备选择正确固件并下载。



---



### 2.4 FT_UPGRADE_FOLDER_OVERLAPPED 

**描述** 
 
- **Android 固件升级** ：备份目录将被覆盖！

**解决方案** 
 
- 目标备份文件夹已存在，请移动并删除旧目录后再备份。



---



### 2.5 FT_UPGRADE_FOLDER_NOT_EXSIT 

**描述** 
 
- **Android 固件升级** ：恢复文件不存在！

**解决方案** 
 
- 在 “Tool folder\BackupNvram\芯片ID” 下找不到 NVRAM 校准文件，请重新下载。



---



### 2.6 FT_UPGRADE_DIR_CREATE_FAIL 

**描述** 
 
- **Android 固件升级** ：创建备份目录失败！

**解决方案** 
 
- 无法在 “Tool folder\BackupNvram” 下创建备份目录，请检查文件夹权限。



---



### 2.7 FT_UPGRADE_FILE_NOT_EXSIT 

**描述 / 解决方案** 
 
- 与 **2.5**  相同。



---



### 2.8 FT_UPGRADE_BACKUP_ROM_NOT_EXSIT 

**描述** 
 
- **Android 固件升级** ：恢复 ROM 镜像不存在！

**解决方案** 
 
- 在 scatter 文件中未找到对应镜像，请确认 scatter 文件未被修改。



---



### 2.9 FT_FIND_NVRAM_ERROR 

**描述** 
 
- 手机数据损坏，找不到 NVRAM 信息。

**解决方案** 
 
- 选择与目标匹配的固件后重新下载。



---



### 2.10 FT_INVALID_FORMAT_ADDR_ERROR 

**描述** 
 
- 无效的格式化地址。

**解决方案** 
 
2. 检查格式化地址或选择自动格式化后重试。



---



### 2.11 FT_FIND_PLATFORM_ERROR 

**描述** 
 
- 找不到 platform.xml！

**解决方案** 
 
- 检查安装目录下是否存在 platform.xml，然后再试。



---



### 2.12 FT_FIND_STORAGE_ERROR 

**描述** 
 
- 找不到 storage_setting.xml！

**解决方案** 
 
- 检查安装目录下是否存在 storage.xml，然后再试。



---



### 2.13 FT_FIND_IMAGEMAP_ERROR 

**描述** 
 
- 找不到 image_map.xml！

**解决方案** 
 
- 确认安装目录下存在该文件，否则请重新安装工具。



---



### 2.14 FT_INVALID_SESSION_KEY 

**描述** 
 
- 无效的会话密钥！

**解决方案** 
 
- 关闭工具并重新打开。



---



### 2.15 ERROR_BL_INCONSISTENT 

**描述** 
 
- 引导加载器需同时全选或全不选。

**解决方案** 
 
- 检查下载页已勾选的镜像项。



---



### 2.16 ERROR_ROM_MUST_ENABLE 

**描述** 
 
- 下载镜像已调整。

**解决方案** 
 
- 选择“格式化全部 + 下载”并重试。



---



### 2.17 ERROR_PMT_UNAVAILABLE 

**描述** 
 
- 手机内部数据损坏或为新机。

**解决方案** 
 
- 选择“格式化全部 + 下载”后重试。



---



### 2.18 ERROR_DATA_LOST 

**描述** 
 
- 分区变化过大，NVRAM 数据将丢失。

**解决方案** 
 
- 选择“格式化全部 + 下载”重试。



---



### 2.19 ERROR_UNKNOWN_ROM 

**描述** 
 
- 加载的镜像包含无法识别的 ROM。

**解决方案** 
 
- 检查 scatter 文件并加载正确文件。



---



### 2.20 ERROR_ILLEGAL_ADDRESS 

**描述** 
 
- 目标 ROM 或 PMT 地址非法。

**解决方案** 
 
- 重新选择并加载目标镜像后重试。



---



### 2.21 ERROR_FILE_NOT_EXIST 

**描述** 
 
- 备份文件不存在。

**解决方案** 
 
- 请联系工具维护者获取帮助。



---



### 2.22 ERROR_CHKSUM_FAIL 

**描述** 
 
- 下载镜像数据已损坏。

**解决方案** 
 
- 请更新下载镜像后重试。



---



### 2.23 E_APP_ADD_RB 

**描述** 
 
- 需要选择要回读的项目。

**解决方案** 
 
2. 点击 **Add**  按钮添加回读条目。
 
4. 至少勾选一个已添加的条目后再试。



---



### 2.24 E_APP_ADDR_ALIGN_RB 

**描述** 
 
- 回读条目的地址或长度未对齐：NAND 须对齐到 4096，EMMC 须对齐到 512 字节。

**解决方案** 
 
2. 检查回读条目的地址与长度是否对齐。
 
4. 若未对齐，双击该条目，在“Readback block start address”对话框中修改起始地址或长度。



---



### 2.25 E_APP_BAT_DATA 

**描述** 
 
- 错误：下载数据长度为 0。

**解决方案** 
 
- 检查加载文件的大小，确保其大于 0 字节。



---



### 2.26 E_APP_BAT_DECRYPT 

**描述** 
 
- 解密下载数据失败。

**解决方案** 
 
- 请检查输入数据是否正确。



---



### 2.27 E_APP_LOAD_AUTH 

**描述** 
 
- 错误：认证文件为空。

**解决方案** 
 
- 点击 **Auth File**  按钮，在执行 DL Certification 之前选择指定的认证文件。



---



### 2.28 E_APP_LOAD_DA 

**描述** 
 
- 进行下载、格式化、回读等操作前需要加载 Download Agent。

**解决方案** 
 
- 点击 **Download Agent**  按钮，选择正确的 DA 文件后重试。



---



### 2.29 E_APP_LOAD_PRELOADER 

**描述** 
 
- 未加载或未启用 preloader 镜像。

**解决方案** 
 
2. 点击 **Scatter‑loading**  按钮加载 scatter 文件。
 
4. 勾选 preloader 镜像后重试。



---



### 2.30 E_APP_LOAD_SCATTER 

**描述** 
 
- 必须先加载 scatter 文件，才能执行下载、格式化、回读等操作。

**解决方案** 
 
- 点击 **Scatter‑loading**  按钮，选择正确的 scatter 文件。



---



### 2.31 E_APP_NONROM_SELECT 

**描述** 
 
- 错误：所选 ROM 文件为空。

**解决方案** 
 
- 请确保在 ROM 列表中至少勾选一个 ROM 条目。



---



### 2.32 E_APP_NULL_READ_FILE_OTP 

**描述** 
 
- 点击 **Update**  前未指定读取参数。

**解决方案** 
 
2. 检查读取信息是否为空。
 
4. 如为空，点击 **Setting** ，在 **OTP Read Setting**  对话框中填写 OTP 参数。



---



### 2.33 E_APP_NULL_WRITE_FILE_OTP 

**描述** 
 
- 点击 **Update**  前未指定写入参数。

**解决方案** 
 
2. 检查写入信息是否为空。
 
4. 如为空，点击 **Setting** ，在 **OTP Write Setting**  对话框中填写 OTP 参数。



---



### 2.34 E_APP_SCATTER_FAILED 

**描述** 
 
- 错误：该 platform 或 storage 不被工具支持。请检查所加载 scatter 文件名是否合法。

**解决方案** 
 
- 确认加载的 scatter 文件受当前工具版本支持。



---



### 2.35 E_APP_SEC_IMAGE 

**描述** 
 
- 错误：加载的 sec 镜像不是签名镜像或解锁镜像。

**解决方案** 
 
- 双击 sec 镜像位置重新加载，选择已签名的锁定镜像后重试。



---



### 2.36 E_APP_SEC_UNLOCK 

**描述** 
 
- 错误：加载的 sec 镜像为解锁镜像。

**解决方案** 
 
- 双击 sec 镜像位置，重新加载锁定镜像后重试。



---



### 2.37 E_APP_START_ASSISTANT 

**描述** 
 
- 应用无法找到 Qt Assistant，或其版本不正确。

**解决方案** 
 
2. 打开工具目录，确认 **assistant.exe**  是否存在。
 
4. 双击 **assistant.exe**  检查能否正常启动。
 
6. 若仍失败，请将错误报告发送给我们。



---



### 2.38 E_SYS_MEMORY_LOW 

**描述** 
 
- 错误：系统内存不足。

**解决方案** 
 
- 关闭部分应用以释放内存后再试。



---

