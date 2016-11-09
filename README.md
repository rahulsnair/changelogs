====================
     11-09-2016
====================


   * build/
2c839fa Merge branch 'cm-14.1' of github.com:CyanogenMod/android_build into bs7.1
a0ae508 build: Require devices to opt-in for SDCLANG

   * device/motorola/athene/
ef78a04 sepolicy: it never ends
6687589 sepolicy: more denials
430bf6b Merge pull request #9 from ejjohnson1999/cm-14.1
73f60d0 disable discard on userdata
dc877d2 Merge pull request #8 from ejjohnson1999/patch-1
6fb5603 lmk disable debug and fast_run as well

   * device/qcom/common/
3d9d25c qc: Add guard makefile for binaries repo

   * frameworks/av/
c3c767d Merge tag 'android-7.1.0_r7' of https://android.googlesource.com/platform/frameworks/av into HEAD

   * frameworks/base/
a0e3fd7 PackageInstallerSession: use ftruncate if fallocate is ENOTSUP

   * frameworks/opt/telephony/
c5c2808 Merge tag 'android-7.1.0_r7' of https://android.googlesource.com/platform/frameworks/opt/telephony into HEAD

   * hardware/qcom/audio-caf/msm8996/
0feef69 Revert "hal: Add abstraction for soundtrigger session"

   * hardware/qcom/audio/default/
930f147 Merge tag 'android-7.1.0_r7' of https://android.googlesource.com/platform/hardware/qcom/audio into HEAD

   * kernel/motorola/msm8952/
adef65a Revert: security/selinux: force permissive

   * packages/apps/Bluetooth/
699645f Merge tag 'android-7.1.0_r7' of https://android.googlesource.com/platform/packages/apps/Bluetooth into HEAD

   * packages/apps/Launcher3/
53eefc5 Merge tag 'android-7.1.0_r7' of https://android.googlesource.com/platform/packages/apps/Launcher3 into HEAD

   * packages/providers/DownloadProvider/
9bfe375 Merge tag 'android-7.1.0_r7' of https://android.googlesource.com/platform/packages/providers/DownloadProvider into HEAD

   * system/media/
adae89b Merge tag 'android-7.1.0_r7' of https://android.googlesource.com/platform/system/media into HEAD

   * vendor/beanstalk/
047ded8 Merge branch 'cm-14.1' of github.com:CyanogenMod/android_vendor_cm into bs7.1
c86fb12 cm: Fix bootanimation sorting

   * vendor/cmsdk/
e085ec0 Merge branch 'cm-14.1' of github.com:CyanogenMod/cm_platform_sdk into bs7.1

====================
     11-08-2016
====================


   * bootable/recovery/
de8de5f Constrain log text output to bottom quarter of the screen.
55ade75 Remove duplicate draw_background_locked() call.

   * device/motorola/athene/
4e5cfe6 athene: bring back README update
8c0f50b omx: use stock N libs
a3ea5c5 athene: Make tree standalone
e9df5e7 athene: rootdir: fix oem script
c0566f5 athene: Switch to stock gps
4617b1e athene: use source audio HAL
5058b02 Revert "athene: update cmactions"
c7594c0 Remove sdcard symlink to /storage
138e292 athene: Build CMActions
804bc01 Revert "cmactions: Integrate with Settings"
8128484 Revert "Add CMActions app Icon"
c7d3c21 athene: add ffmpeg codecs support
bda30bc athene: add missing surround files thx @sileshn again...
2a697a9 athene: audio update
5c8aa18 athene: add surround config
e73746b athene: update props from N
b5d3776 athene: Sync proprietary-files.txt with vendor
8db2c69 athene: Move to new generic extract scripts
f5cef2b athene: Add misc entry in fstab.qcom This change is to add misc partition entry in fstab.qcom. This is used by uncrypt module to write into this partition, which is then read by recovery mode to perform appropriate action.
63ce76d athene: cmactions: Integrate with Settings

   * frameworks/av/
fdde5b2 Camera: Support obtaining camera memory from MemoryHeapIon

   * frameworks/base/
b1e4d06 [1/2] base: Screenshot Crop & Share
9dd6045 Add back imports removed from last commit in order to fix build.

   * frameworks/native/
d7b29fa binder: Squashed commit of MemoryHeapBaseIon

   * frameworks/opt/telephony/
ec18aba Add dummy SUB record in CDMA NV mode
6b3b5b8 Send EVENT_NV_READY to GsmCdmaPhone
1bcf4b7 tests: Update SubscriptionInfo parameters to match fwb

   * packages/apps/Settings/
287e3cc Screenshot crop and share

   * system/bt/
7924a32 bt: Use HCI H4 HAL for BT SOC ATH3K

   * vendor/beanstalk/
4f17434 common: add quotes to satisfy kati/bash/make/whatever

   * vendor/cmsdk/
7f19e74 PerformanceManager: Fix power hint values

   * vendor/motorola/
e52865f athene: omx: use stock N libs
ca4b970 Changes for standalone device tree

====================
     11-07-2016
====================


   * frameworks/av/
0e9394b Merge branch 'av-aosp.lnx.2.0.r5-rel' of git://codeaurora.org/platform/frameworks/av into cm-14.1

   * frameworks/base/
8efb5d9 batteryservice: Remove remnants of CAF's HVDCP changes
788b085 connectivity: Configure additional TCP parameters
41bb123 Fix nav bar showing always on the left when rotated to 270 degrees.
9065080 pm: Fix NPE
eccb120 SystemServer: Do not start Atlas Service on lowram devices.
b9a839c Fix long press volume buttons skip tracks
38724d1 services: battery: Don't blink with an hvdcp charger
50e6146 Clean up "Optional screenshot type" code in PhoneWindowManager
efcff01 Fix race condition in setting notification panel height
7f0c7b6 Makes the loading "spinner" animation smoother in non-holo apps
de3e8a3 Fix left clock padding
0e41293 Disable more debugging
b7ea9a6 Reduce log verbosity: Don't spam logcat
be8262f Turn off some debugs
a70bc20 Screenshot delay [1/2]
8939981 Refresh USB tile
4c5aa51e Add back screenshot delay

   * frameworks/opt/setupwizard/
b9dc8b2 Fix setupwizard crashes for tablets

   * frameworks/opt/telephony/
7893415 Telephony: fix SMS NPE
aa9bab9 Phone App crash: process com.android.phone has stopped.
6e91f68 Single digit MMI codes cause CTS to fail
9766216 GsmMmiCode: Fix USSD NPE
2a16b66 For NV-based devices like CDMA only devices, ignore ICC Card status change EVENT.
213e3cd Suppress error pop-ups for single digit dials.
3eae650 MMS: Update apnProfileID for MMS only apn.
a357ec0 telephony: Configure additional TCP parameters
3800210 telephony: Fix NPE when switching data SIM

   * hardware/intel/img/hwcomposer/
09c4a9b intel: hwcomposer: csc mode is only supported on newer blobs
e9b348b intel: hwcomposer: Use ASUS_ZENFONE2_LP_BLOBS instead
158e0af hwc: merrifield_plus: Add legacy LP blob support
bb212e0 Selectivly Revert "Switch away from the deprecated IMG Graphics HAL APIs."

   * hardware/ril-caf/
03a5a1d Properly parcel v6 RIL_CellInfo GSM cell response.

   * kernel/motorola/msm8952/
7fd6723 fix merge derp
c10a03a msm: vidc: Change video clocks when operating rate is changed
fc9bf9d cdc_ncm: do not call usbnet_link_change from cdc_ncm_bind usbnet_link_change will call schedule_work and should be avoided if bind is failing. Otherwise we will end up with scheduled work referring to a netdev which has gone away.
eb7abb0 ASoC: msm8x16-wcd: Remove 20ms sleep in rx chain PMD
0b3a35c ANDROID: binder: Clear binder and cookie when setting handle in flat binder struct
4af774c arm64: perf: reject groups spanning multiple HW PMUs
2b02ad3 tcp: make challenge acks less predictable
8254d0e ARM: perf: reject groups spanning multiple hardware PMUs
4d08360 binder: prevent kptr leak by using %pK format specifier
828e2f9 net: Fix use after free in the recvmmsg exit path
9156c19 KEYS: Fix ASN.1 indefinite length object parsing
757d8fc mfd: wcd9xxx: avoid slimbus read/write during ADSP reset
d62d9ed ASoC: msm: lock read/write when add/free audio ion memory
7ab0a26 fs:fuse: Disable shortcircuit when mmap is called on a file
4da8972 cfg80211: Define macro to indicate support for cfg80211 abort scan api
4abab24 cfg80211: Add support for aborting an ongoing scan
8a645fe9 msm: camera: Change MAX_CID_CH macro to 3
e15bbbb drivers: dma-removed: use memset_io for ioremap region
44fd802 input: synaptics_dsx: allocate heap memory for temp buf
72c15c0 perf: Tighten (and fix) the grouping condition
7180609 idle: add a check for need_resched() after rcu_idle_enter
f74f091 ion: use %pk instead of %p which respects kptr_restrict sysctl
45618d4 ASoC: msm: qdsp6v2: set token for stereo_to_custom_stereo command
02b7c8c net: ipc_router: fix NULL pointer de-reference issue
ba377e790 sched: Fix integer overflow in sched_update_nr_prod()
8edb16b msm: camera: cpp: Add validation for v4l2 ioctl arguments
6ae9a8d netfilter: x_tables: validate e->target_offset early
4c3b8f9 ASoC: msm: initialize the params array before using it
7e0c10d qseecom: Change whitelist_support flag to false if TZ failed to check
9734647 ASoC: soc: change audio drivers to use %pK
0c150efd ASoC: soc: change audio cpe drivers to use %pK
1b84501 ASoC: msm: qdsp6v2: Change audio drivers to use %pK
e10d08f unix: avoid use-after-free in ep_remove_wait_queue
a57626b msm: camera: Change %p into %pK
772549b msm: mdss: Move PP programming aptly for video and cmd modes
013c381 ASoC: wcd-mbhc: correct cross connection check
8cdebe8 ASoC: wcd-mbhc: fix inconsistent detection of euro headset
c753ac6 qcedev: Validate Source and Destination addresses
9fc3118 ASoC: msm: Add Buffer overflow check
2e57626 ASoC: utils: initialize dummy_codec before use
ace55e6 netfilter: x_tables: make sure e->next_offset covers remaining blob size
7ff44bc ecryptfs: forbid opening files without mmap handler
95ca6a4 ASN.1: Fix non-match detection failure on data overrun
6ab0492 msm: sensor: validate the i2c table index before use
a4e0755 rmnet_data: Changing format specifier to %pK
3ddb356 ASoC: wcd9335: reduce speaker teardown latency
a3752a1 net: rmnet_data: Stop adding pad bytes for MAPv3 uplink packets
c965cff net: rmnet_data: Stop adding pad bytes for MAPv4 uplink packets
4da3b10 Don't show empty tag stats for unprivileged uids
80b8a5e msm: mdss: Disable histogram interrupt in ISR
194fc65 msm: mdss: Fix potential NULL pointer dereferences
f15ff8c msm: mdss: enable tearcheck while entering LP1 state
5acc923 defconfig: arm64: msm-perf: Disable HSLite and HSConsole
a6db46d msm: mdss: add support to read current VIC from sysfs node
6fe131e msm:vidc: Add null check for handle in smem buffer comparision.
0ab1947 qos: wake up cores based on the qos updated cpu mask
160dc45 msm: vidc: Set constrained intra refresh property
cc2c5d2 defconfig: arm: setting mmap_rnd_bits
e04e315 msm: camera: Restructure data handling to be more robust
76246c1 coresight: fix the dangling pointer issues on coresight
44180f6 msm: camera: sensor: Fix use after free condition
22c6f09 trace: resolve stack corruption due to string copy
7ea2899 misc: qcom: qdsp6v2: initialize config_32
60f9f67 ASoC: msm: set pointers to NULL after kfree
dbc65b9 defconfig: msm: Enable MODULE_RONX
b60c8dd msm: mdss: hide kernel addresses from unprevileged users
953a458 qseecom: allocate sglistinfo buffer for kernel clients
d048365 qseecom: support whitelist memory for qseecom_send_modfd_cmd
9732801 qseecom: make change to support sg list entry number larger than 512
7b09466 cfg80211: Define macro to indicate support for new cfg80211 connect api
c2004bf cfg80211: Add option to report the bss entry in connect result
bb34c15 cfg80211: Define macro to indicate prev_bssid connect support
c2f18b4 cfg80211: Add option to specify previous BSSID for Connect command
8ba9ba8 cfg80211: Define macro to indicate bssid based scan support
35e7972 cfg80211: Allow a scan request for a specific BSSID
59fecf2 Revert "ANDROID: mmc: move to a SCHED_FIFO thread"
f6a5a66 msm: sensor: Avoid potential stack overflow
5edcd8f tty: Fix unsafe ldisc reference via ioctl(TIOCGETD)
a605f33 msm-core: debug: Update the number of supported pstates
aa919ce msm-core: debug: Fix the number of arguments for sysfs nodes
2ba73dd misc: qcom: qdsp6v2: initialize wma_config_32
de9e31b misc: qcom: qdsp6v2: Add missing initialization
f49d16a msm: msm_bus: limit max chars read by sscanf
2c5b67f ASoC: wcd9335: Fix compander disable after SSR
c174306 msm: kgsl: Change %p to %pK in debug messages
7d7fd54 adf: Zero out the mapping data
138eeae ipv6: add complete rcu protection around np->opt
f5f11a6f msm: vidc: use %pK instead of %p which respects kptr_restrict sysctl
f8e332b msm: perf: validate input argument of ev_constraints functions
c94bde9 msm: mdss: configure DSI PHY when resuming from ulps suspend
0e1a857 defconfig: Enabling config INET_DIAG_DESTROY
2ab66fe defconfig: arm64: msm-perf: Enable SERIAL_MSM_HS
e81bf45 Revert "Revert "ARM: dts: msm: update memory map for msm8976/8956/8952 for External release""
147a0a6 soc: qcom: smp2p: Fix kernel address leak
020cce3 Fixing copyright markings
5845d56 ASoC: msm: qdsp6v2: DAP: Enable non DAP modules on DAP disable
fb8b981 USB: fix invalid memory access in hub_activate()
e2862f2 msm: vidc: Add control to set csc coefficients to firmware
8959730 msm: vidc: Add support for color space information
7042055 msm: vidc: Add SEI extradata.
22180a4 net: fix infoleak in rtnetlink
d66123b msm_defconfig: Enable config for b/29119870
68fc06e FROMLIST: security,perf: Allow further restriction of perf_event_open
2c2bf68 BACKPORT: perf tools: Document the perf sysctls
2d3583a ALSA: seq: Fix race at timer setup and close
457315f net: validate the range we feed to iov_iter_init() in sys_sendto/sys_recvfrom
f4e0c2a msm: crypto: Fix integer over flow check in qcrypto driver
1432d87 ARM: dts: msm: Add Bluetooth configuration for 8976 devices
945fdc4 ARM: dts: msm: Enable blsp1 uart0 core
88875b2 ARM: dts: msm: Add Bluetooth voltage configuration for 8976 devices
ed19fc2 crypto: msm: qcrypto: Fix spinlock deadlock issue
1a8be9c cnss: Reset QCA Card during WLAN SubSystem Recovery
0609ca9 ARM: dts: msm: add pmic gpio_2 to 8976 target
e1301b4 arm: dts: add bus bandwidth support for sdio wlan module
1e114dc ARM: dts: msm: Enable QCA VReg and cnss node based on board id
ef6c2bd msm: ipa: handle information leak on ADD_FLT_RULE_INDEX ioctl
053dcd9 Replace %p with %pK to prevent leaking kernel address
97c415d msm: ipa: fix potential race condition ioctls
72a5291 msm: kgsl: Allow 0 as a valid ion file descriptor
9bf2fbd perf: stop deadlock when cpu_up fails
1291ca0 cfg80211: Define macro to indicate bssid hint backport support
f2c208c net: cnss_prealloc: Add memory for high latency SDIO interface
28bf722 net: cnss_prealloc: Add skb prealloc support
307edce cnss: Update prealloc memory table
b3f25f3 ASoC: Fix freed memory access of pcm stream kctl
32b98ac net: cnss: add bus bandwidth support for sdio wlan module
bee533c net: cnss: refactor PM QoS request wrapper API
6be9267 net: cnss_sdio: add PM QoS support in cnss sdio platform driver
6a64ca9 Net: CNSS_SDIO: Add cnss_get_restart_level CNSS API
c13409a cnss: sdio: Define OOB interrupt interfaces.
dd8b145 net: wireless: add conditional compilation flag for cnss
bbc109f cnss-sdio: Dynamically allocate ramdump memory
c83d4bd ARM :dts :msm: Add QCA6174 dts node and voltage regulator
abb8db8 Net: CNSS_SDIO: add sdio wlan driver registration
45890f1 net: cnss: remove 3.3v PMIC gpio enable feature
6b02f03 net: cnss: enable rome_vreg_dsrc regulator for dsrc
314bb0e wcnss: Fix compilation issue for wcnss crypto module
97660e9 net: cnss platform driver for SDIO WLAN module
27f90b3 power: qpnp-smbcharger: Handle USB removal during pulsing
6405d62 msm: mdss: update rotator frame rate in the pipe configuration
3a81a0d msm: vidc: use %pK instead of %p which respects kptr_restrict sysctl
525eb0f msm: mdss: Fix memleak in framebuffer register and remove
e9df1ef diag: Perform member-wise copy instead of memcpy
82c1bbd power: reset: msm: Handle dm-verity and keys reset reasons
c44265d msm: mdss: Fix to validate data copied from user space
cb5e126 msm: crypto: Fix integer over flow check in qcedev driver
1150348 msm: mdss: Fix potential NULL pointer dereferences
e5b0311 spmi: prevent showing the address of spmidev
eed06fe arm64: dma-mapping: always clear allocated buffers
78a3364 ASoC: wcd9335: Enable standalone ldo_h
c025396 ARM: dts: msm: add perf-events support for msm8952
690649f msm: mdss: Fix memleak in panel_debug_reg_write
7cfc013 msm: kgsl: Verify the pointer isn't NULL before using it for kref
6c67c9e qseecom: validate the inputs of __qseecom_send_modfd_resp
2f623ed coresight: fix use-after-free in stm on secure boot devices
44c7d34 mmc: block: Add check to mmc_blk_part_switch
196c1c0 msm: mdss: Notify backlight change in update backlight function
629d575 mmc: core: Remove flag MMC_PM_WAKE_SDIO_IRQ in mmc_resume_host
3767228 ARM: dts: msm: add qcom,broken-pwr-cycle-host to SDHC3 in MSM8976
0f364fb mmc: sdhci-msm:Add qcom,broken_pwr_cycle_host capability using DT
3e48521 mmc: sdio: Add MMC_CAP2_BROKEN_PWR_CYCLE & fix mmc_sdio_init_card
dbcf3df mmc: card: Fix card quirk bit setting value
3de0612 msm: dma_test: Initialize newly allocated memory
d3dee6c ASoC : msm: qdsp6v2: Add size check in audio cal ioctl
283c972 wcnss: Avoid user buffer overloading for write cal data
34c6622 drivers: soc: Add buffer overflow check for svc send request
d400632 ASoC: msm: qdsp6v2: DAP: Update check to validate data length
bf1ca1d msm: mdss: Correct the format specifiers in sscanf function
32ed764 msm: mdss: keep tear check enabled in LP1 power state
e0263a6 msm: mdss: restructure tearcheck config
89ceb16 msm: mdss: reset intf_stopped flag for sctl when exiting LP states
8d6f9b4 hrtimer: don't send an IPI unnecessarily during migration
857e5eb ASoC: dapm: correct the macro to SND_SOC_DAPM_CLASS_RUNTIME
d4614b8 AIO: properly check iovec sizes
ee86abd msm: perf: Protect buffer overflow due to malicious user
a95ad05 msm: mdss: remove usage of DSI ctrl mutex during ESD/suspend path
a772e99 msm: mdss: fix mdp busy wait race condition
db10a99 msm: mdss: delay dma commands for split-dsi cmd mode panels
df195c5 msm: camera: Fix memory read by adding bounds check

   * packages/apps/CMParts/
6bfd759 Merge branch 'cm-14.1' of https://github.com/CyanogenMod/android_packages_apps_CMParts into bs7.1
b62ecf7 CMParts: rotation: Clean up UI and code

   * packages/apps/CarrierConfig/
0af4ed4 Resolve NZ roaming entry

   * packages/apps/Dialer/
1e5c3de Re-add call recording feature.
c4ac6d5 Revert "nCallUI: Add support for call recording"
425abd4 InCallUI: Fix background colour of tabs on DSDA phones
c1e1098 Fix reveal animation for outgoing calls.

   * packages/apps/OmniSwitch/
5d2e7bf OmniSwitch: time for a fresh look

   * packages/apps/Settings/
a0e68ab WirelessSettings: Remove NFC category if there's no NFC adapter
1d80686 Remove kerneladuitor from dashboard settings.  Kind of pointless.
7509418 Settings: fix battery icon in dashboard
fabfca3 Settings: cm-ify wireless settings screen
3fea6b6 Fix searched item isn't highlighted
1f08060 Settings: Fix Crash when switch user
6934eeb Settings: fix the "force close" in Settings at monkey-test.
785e0d3 Settings: Occurred "com.android.phone" force close 9 times at monkey test.
607c54a Settings:  Fix settings force close in monkey test.
5f75617 Settings: "Back" icon not work on Settings-Security-Encrypt phone
6643e1b Settings: Make APN of CT can be edited and be saved.
f657dd2 Settings: Fix settings force close in monkey test.
db2d733 Settings: Fix settings force close in monkey test.
90d4302d Settings: Fix settings force close in monkey test.
1cf709b Settings: Fix AssertionError in monkey
0077460 Settings: Fix SparseArray null pointer issue in monkey issues
ee8fd7b Hide the accounts which added for data pack
570a214 SAP: Enable 5Ghz AP band option only when a valid country code is received
cedb551 Hide the accounts which added for data pack
1f0f410 Settings: The APN cannot be edited after tapping right of APN
dc20dee Make America build again.
3c21880 Screenshot delay [2/2]
91f3e83 Revert "Use same technology type for LTE/4G"

   * packages/services/Telecomm/
529106c Fix sporadic crashes with MSIM devices and inactive SIMs
d37a99e Telecomm: Update icon to Material

   * packages/services/Telephony/
8e786fd Merge branch 'cm-14.1' of github.com:CyanogenMod/android_packages_services_Telephony into bs7.1
eb055fa Telephony: Redirect to roaming SIM network setting(Dual SIM)
80416fe EditPhoneNumberPreference: Prevent empty text from being set
9022fda Switch back to Auto selection if Manual fail's
2ae24ed PhoneApp Crash: Multiple times due to permission issue
21bd850 MSIM: Show Enhanced 4G LTE mode option for IMS subscription
ac96ab8 Revert "Single digit MMI codes invalid." Feijao: Single digit MMI codes are valid when in-call
1608ed1 Apply correct theme color to USSD progress dialog.
b027031 Fix MSIM voicemail notification icons.
fcc98cb Single digit MMI codes invalid.
36673a9 Fix CDMA vs. WCDMA typo in cs translations
2d191b7 Fix removal of 'all accounts' preference.
49433ec Order SIM accounts properly.
245ca39 Telephony: Exit call features if our error is unrecoverable.
91d68d8 Remove hard-coded CDMA roaming mode restrictions.
e12b716 Change string "Cellular" to "Mobile"
c867378 Fix multiple apn items issue

   * system/sepolicy/
2e053ed Merge branch 'cm-14.1' of github.com:CyanogenMod/android_system_sepolicy into bs7.1
a35663a Add rules required for TARGET_HAS_LEGACY_CAMERA_HAL1

   * vendor/beanstalk/
aa17bdb remove prebuilt kerneladiutor.  Not a fan of forcing unnecessary packages on users.  Not sure why I've kept it this long.  Anyways, easily downloaded from play store if the user wants it.
beec750 Merge branch 'cm-14.1' of github.com:CyanogenMod/android_vendor_cm into bs7.1
143269c vendor: cm: Move fuseblk to system/sepolicy
1bbf3e9 envsetup: block SDCLANG on Darwin for now
3e169cb Merge branch 'cm-14.1' of github.com:CyanogenMod/android_vendor_cm into bs7.1

   * vendor/cmsdk/
a75c1b2 Merge branch 'cm-14.1' of github.com:CyanogenMod/cm_platform_sdk into bs7.1
abe4122 cmhw: Fix boot handling

   * vendor/motorola/
f0d1a03 Switch to stock gps

====================
     11-06-2016
====================


   * device/qcom/sepolicy/
8259f14 Merge remote-tracking branch 'caf/LA.BR.1.2.9_rb1.8' into cm-14.1

   * frameworks/av/
dc61dbf libstagefright: Support for legacy camera/encoder buffers

   * kernel/motorola/msm8952/
df195c5 msm: camera: Fix memory read by adding bounds check
855059f ASoc: wcd9335: Fixed supported sample rates in tash_mad1 DAI
1a86439 ASoC: compress: fix unsigned integer overflow check
8dff7eb staging: android: Change %p to %pK in debug messages
d5a21b6 msm: qpnp-haptic: add debug messages for RC clock error correction
77d90ad msm: qpnp-haptic: add DT property for back-emf generation delay
b8775bc ARM: dts: msm: change auto resonance calibraiton period to 4 cycles
e856e9e ARM: dts: msm: add PON regulator support for PMI8952 haptics
fd4fec1 char: msm_smd_pkt: Fix the TIOCMSET IOCTL argument reading
51ecda9 msm: mdss: Fix memory leak in panel_debugfs_create_array func
b4b2f5c ASoC: msm: qdsp6v2: DAP: Add check to validate data length
0eccf22 Merge "mmc: cmdq_hci: Move Qos calls before Data/DCMD desc write"
1437552 Merge "defconfig: remove CONFIG_MSM_BUSPM_DEV reference."
c0dcc42 msm: qpnp-haptic: add PON regulator support
4fc745b ASoC: open ASM session with 24 bit for 24 bit playback.
3de9e8c msm: mdss: xlog: Add support to dump registers from interrupt context
3fb69ed msm: mdss: Allocate max size cursor image buffer
ea8e883 ARM: dts: msm: add PON regulator for PMI8950
48a5936 lowmemorykiller: Introduce sysfs node for ALMK and PPR adj threshold
c05d735 msm: mdss: avoid FIFO overflow handling when error is masked
bd1da5f soc: qcom: spm: Poll for the PMIC_STATE after updating the VCTL register
87d0282 ASoC: msm: qdsp6v2: DAP: Add check to validate param length
8f5e6b8 ASoC: msm: qdsp6v2: DAP: Allocate param buffer with correct size
a4b5997 msm: ipa: Fix to polling mode
5659926 mmc: sdhci-msm: use PIO for tuning commands
d0c53ec mmc: sdhci: Add new quirk to use PIO for eMMC tuning commands
ff2e26b mmc: sdhci-msm: enable quirk to define non standard tuning
729492a mmc: sdhci: add a quirk to define non standard tuning
ae56e0c mmc: sdhci: Implement set_transfer_params() cmdq host op
20d2c2a Merge "power: qpnp-smbcharger: add support to control hvdcp3 detection dynamically"
ee613a4 mmc: cmdq_hci: add set_transfer_params() to CQ unhalt
7218cf3 mmc: cmdq_hci: set block size as part of CQ unhalt process
a95fc56 mmc: host: set correct state when suspend fails
20a6e28 ion: destroy ion handles under client->lock
3b14bcd qseecom: Change format specifier %p to %pK
f7946f0 input: synaptics_dsx: remove array declaration in write function
629b4ea power: qpnp-smbcharger: do not float DP/DM lines during QC3.0 detection
a6f8c14 msm: qpnp-haptic: update play sequence for QWD mode
9178d6b msm: mdss: fix possible overflow errors in panel_debug_base_reg_read
37b7841 msm: wlan: Add new country XA
37bedca Merge "msm: thermal: Add support to monitor only one tsens for MX restriction"
f1ea144 Merge "msm: thermal: Maintain state in the mitigation device monitor"
665c394 msm: mdss: Properly free memory in error case
7004c47 ASoC: wcd9335: add support for packed 24 bit.
13fef9a regualtor: spm-regulator: Add additional settling delay for FTS2.5 SMPS
a11117c tpacket: Notify userspace about packets with CHECKSUM_UNNECESSARY
508ac0d Revert "net: tun: Implement TUN_NOCHECKSUM"
3dcb823 msm: vidc: add ion_handle checking before mapping buffers.
f578614 NFC: Fix crash due to invalid use of ese gpio
49b06af NFC: eSE power request implementation
d0d0385 mmc: cmdq_hci: Move Qos calls before Data/DCMD desc write
6b50d4a mfd: wcd9xxx-slimslave: Change slim driver to use %pK
de548d4 ASoC: msm: qdsp6v2: Change audio drivers to use %pK
426ea03 msm: mdss: Correct block id check for mdss_mdp_misr_table
a7923ce ARM: dts: msm: Modify nq device node for 8952/8976
3902d83 NFC: Error handling correction in probe
b505bb5 NFC: CE transaction failed during system suspend
7dd949f NFC: Remove DMA allocation and stack use in write
b99da88 NFC: Remove sleep from irq handler
7103478 nq-nci: XO shut down issue fix
ac8b294 nq-nci: enable NFCC hardware check and clock to NQxx
a8c5205 NFC: Fix function descriptions
8eb71ae power: qpnp-fg: Re-enable empty soc interrupt configuration
66d0c6f msm: mdss: fix possible overflow errors in panel_debug_base_reg_read
f42e07a USB: android: Ensure at least two serial ports are initialized
da81976 tun: Set CHECKSUM_UNNECESSARY if userspace passes this indication
70e68fb net: rmnet_data: Change the print format for addresses
b019337 ASoC: WCD9335: important changes on tasha codec
22e20e6 qcom: ssr: Fix possible overflow when copying firmware name
9734fca ASoC: msm: qdsp6v2: Increase period size for pcm driver.
9d43925 diag: Fix possible kernel addresses leak
8f6b4d7 usb: type_c: pericom: Register with dual_role_usb class for role switch
eca11d4 usb: dual-role: make stub functions inline
c3f9741 msm: vidc: refine DCVS for low fps video
460d8fc Bluetooth: Replace %p with %pK
cb0d083 net: ipv6: allow choosing optimistic addresses with use_optimistic
ad368fd net: ipv6: Add a sysctl to make optimistic addresses useful candidates
c9aa8f7 msm: perf: Do not allocate new hw_event if event is duplicate.
d57650e Merge "slim-msm-ngd:Avoid using stale pipe handle"
772dbc2 msm: mdss: reset DSI LANE control register during initialization
a80b5a9 msm: camera: Setting actuator to initial position
d6e7515 msm: kgsl: Check the address range before mapping to GPU
d8bb404 net: core: neighbour: Change the print format for addresses
754c6a1 msm: kgsl: Add property to determine GPU bitness
139aa0a ASoC: msm8952: add support for packed 24 bit.
40cc087 ASoC: msm8x16-wcd: add support for packed 24 bit.
33909a9 ASoC: msm8x16-wcd: add support for packed 24 bit.
005699f ASoC: msm: qdspv2: add support for MULTI_CHANNEL_PCM_V3 command
375711c ASoC: msm: qdsp6v2: pull mode playback and push mode record.
63abbd5 msm: mdss: fix backlight update between unblank and kickoff
2b2ac5b Revert "msm: mdss: Fix support for ARGB1555 and ARGB4444"
200233c msm: thermal: Check clients request just after frequency thread init
54d1a9b USB: dwc3: debugfs: Add boundary check in dwc3_store_ep_num()
0004e70 USB: gadget: serial: Fix debugfs crash
bd1a45a lpm_levels: Avoid race by preventing hotplug during lpm probe
c5aa9f0 net: core: To send ARP probe when neighbor state is NUD_STALE
d35be5f08 msm: mdss: set default resolution of DBA driver during boot
2687ab7 ARM: dts: msm: Enable all the csiphy clks in csiphy_init
23062a9 msm: kgsl: Change GPU RAC hardware clockgating
cd3f937 msm: camera: isp: Fix warning and errors based on static analysis
2bb4293 driver core: fix race between creating/querying glue dir and its cleanup
4fefed4 Merge "msm: kgsl: Zero the pointer to the dmabuf sg list before freeing"
84b797a spmi-pmic-arb: add support to dispatch interrupt based on IRQ status
b53e294 msm: camerav2: sensor: Avoid csiphy release when used in combo mode
1111e31 qcom: scm: Support register x6 to pass the session id
c7ed1ca msm: isp2: Issue REG_UPDATE when only RAW stream exist per session
8ff417f ASoC: msm: audio-effects: fix stack overread and heap overwrite
f5bae99 arm64: ftrace: fix function_graph tracer panic
5bfcb8a msm: kgsl: Avoid race condition in ioctl_syncsource_destroy
892798e arm64: kernel: pause/unpause function graph tracer in cpu_suspend()
6a0ca52 ASoC: msm: audio-effects: misc fixes in h/w accelerated effect

   * packages/apps/CMBugReport/
4cf7aad bugreport: Fix permission restrictions

   * packages/apps/Contacts/
bb83402 [1/2] Contacts: make shapes great again

   * packages/apps/ContactsCommon/
0da306c [2/2] ContactsCommon: make shapes great again

   * system/sepolicy/
52a4d3b system: sepolicy: Import fuseblk from vendor/cm

   * vendor/beanstalk/
b0cecb7 Always create a kernel defconfig build artifact

   * vendor/cmsdk/
f133161 cmhw: Fix boot handling

   * vendor/motorola/
6c952c1 Add apk's for Volte support
21bfd4a We use source built gps
bdb64dd athene: use source audio HAL

====================
     11-05-2016
====================


   * build/
8d7c71a Merge branch 'cm-14.1' of github.com:CyanogenMod/android_build into bs7.1

   * frameworks/base/
2fff2a3 Use @hide for screenshot setting
2cdc6b6 Optional screenshot type [1/2]
5c86768 Don't crash if print spooler doesn't have location permission.
828b537 Don't show quotation marks around Wifi network name in Settings.
e68653e Support enforcing a minimum delay between notification sounds of an app.
6eaa5c3 (Optionally) allow vibration during priority zen mode.
21915d5 Revert "Mms: Fix no ringtone for MT SMS during the call."
c36faf6 Add importance level to block lock screen notifications (fixed) (1/2)
cf9a09a Revert "Proximity speaker [1/2]"
0eae757 Revert "Dialer Lookup [1/2]"

   * frameworks/opt/net/wifi/
8594d48 wifi: Set the mode at native layer

   * frameworks/opt/telephony/
a164555 Telephony: handle 3rd party sms apps + 'always ask'

   * packages/apps/AudioFX/
db8cc15 AudioFX: Fix possible RuntimeException
a01d9e0 AudioFX: Fix possible NPE

   * packages/apps/Settings/
182efad Optional screenshot type [2/2]
b3f422c Show SIM name as data usage mobile network category title.
19e7cf3 Integrate mobile network settings into SIM settings for MSIM.
ef422dc Remove a few MSIM tab hosts.
e3a92f5 Add setup UI for minimum delay between an app's notification sounds.
de89d0b Allow selecting vibration mode during zen priority mode.
0ea8bc6 Add importance level to block lock screen notifications (fixed) (2/2)

   * packages/apps/Snap/
70edacf Snap: Fix possible RuntimeException (due to NPE)
3da1aa3 Snap: Fix possible NPE
72e249c CameraNext: dynamically generate available photo resolutions

   * packages/apps/Trebuchet/
7b7aab4 Trebuchet: Remove stats/tracking

   * packages/services/Telephony/
8a4f571 Merge branch 'cm-14.1' of github.com:CyanogenMod/android_packages_services_Telephony into bs7.1

   * system/sepolicy/
df55f36 Merge branch 'cm-14.1' of github.com:CyanogenMod/android_system_sepolicy into bs7.1

   * vendor/beanstalk/
8ab9e00 Added contributors for vegetalte
6ddd835 themes: allow system_server to relabel them dir
8614943 Contributors: Add maintainers for BQ Aquaris M5 (piccolo)
7f3e6df Contributors: Add maintainer for Alcatel Idol 3
6aab884 Merge branch 'cm-14.1' of github.com:CyanogenMod/android_vendor_cm into bs7.1
63984ef ambient: Remove from OSS builds
1998914 vendor_cm: Vodafone TR: Fix mobile data on first boot
26e669b cm: Autodetect SDCLANG in prebuilts/snapdragon-llvm

   * vendor/cmsdk/
91b3848 Merge branch 'cm-14.1' of github.com:CyanogenMod/cm_platform_sdk into bs7.1
