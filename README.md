====================
     11-27-2016
====================


   * bootable/recovery/
6a0693f bootloader_message: allow devices to override

   * device/motorola/athene/
bf8982c athene: sync proprietary files with vendor

   * external/toybox/
c3a5a80 losetup: Fix loop mounting

   * frameworks/base/
3d51ae2 Merge "sysui: New google pixel colors fix" into n7.1

   * hardware/qcom/audio-caf/msm8960/
b9282f8 hal: Port the dock support to non-legacy 8960 hal

   * packages/apps/COTA/
a6e92cb Cota: Make notification icon white
6446d22 Cota: Readjust the image to display properly

   * packages/apps/Settings/
438570d Settings: Custom Carrier Label Option for MSIM
e1aa841 Update Italian Translation

   * packages/apps/SoundRecorder/
d309f7d SoundRecorder: Add permission for ACCESS_NETWORK_STATE

====================
     11-26-2016
====================


   * build/
7ab6faa build: kernel: Remove duplicated targets
2e422fe build: Set android jack args to global jack server args if existing

   * device/motorola/athene/
0232da0 athene: add back partitions context
80e6eec fix build

   * external/f2fs-tools/
d895e39 f2fs-tools: hack headers to unbreak darwin build

   * frameworks/base/
e080c5a PhoneStatusBar: Small performance fixes
7c6458f Revert "frameworks: fix system server crash"

   * kernel/motorola/msm8952/
881295f input: synaptics: Add checks of user input data
ef36cdf msm: ipa: Sync reset command between ipa and uC
a7811a6 qseecom: remove entry from qseecom_registered_app_list
aeb08b6 msm: sensor: Adding mutex for actuator power down operations
26ae46c msm: ipa: clear before processing
4587ae0 drivers: qcom: ultrasound: Lock async driver calls
3ae4146 ALSA: usb-audio: Fix double-free in error paths after snd_usb_add_audio_stream() call create_fixed_stream_quirk(), snd_usb_parse_audio_interface() and create_uaxx_quirk() functions allocate the audioformat object by themselves and free it upon error before returning. However, once the object is linked to a stream, it's freed again in snd_usb_audio_pcm_free(), thus it'll be double-freed, eventually resulting in a memory corruption.
a5c315b ALSA: usb-audio: Minor code cleanup in create_fixed_stream_quirk()
6ef5082 BACKPORT: audit: fix a double fetch in audit_log_single_execve_arg()
eb39c56 af_unix: Guard against other == sk in unix_dgram_sendmsg
b390e2f xc2028: avoid use after free
5148d35 block: fix use-after-free in sys_ioprio_get()
2dcee40 HID: core: prevent out-of-bound readings
5272a44 msm: ipa: use GFP_ATOMIC for DMA memory allocation during SSR
632b4e6 msm: kgsl: Fix overflow in sharedmem cache range operation function
eb18298 tcp: fix use after free in tcp_xmit_retransmit_queue()
3e18705 UPSTREAM: perf: Fix race in swevent hash
6cca8a5 qcom: scm: remove printing input arguments
cf308a2 soc: qcom: scm: add check to avoid buffer overflow
97ddddd ASoC: msm: Update machine driver with AVS 2.7 support
aab3c86 ASoC: msm: add support for AVS 2.7 in native drivers
dd9693e ASoC: msm: qdsp6v2: Add support to query adsp version
6aeee49 radio-iris: check argument values before copying the data
9baaf6b Merge "arm: dma-mapping: page align size before flush tlb"
5254c2e msm: mdss: fix pp timeout during transition from LP1 to power on
49e231c msm: mdss: extend mutex ovlock for vsync handler
eecf268 ANDROID: binder: Add strong ref checks
168fbf6 Merge pull request #2 from rahulsnair/cm-14.1

   * packages/apps/COTA/
03cbab4 Cota: Update baseline infrastructure

   * platform_manifest/
a2a8244 manifest: track frameworks/opt/hardware

   * vendor/aoscp/
518bc35 CypherOS 3.1.3 Release 12
fba488f Devices: Drop support for Onyx
4f5b922 Configs: Drop support for NFC Enhanced
d7937ca Devices: Update hammerhead makeConfig
a3789e4 extract_utils: Use shasum on macOS
462c3ce vendor_asocp: enable hidden storage manager
78b7a90 Clean up 3G config for Vietnamese network

   * vendor/cmsdk/
81beee6 cmsdk: Ensure CMHW feature constants aren't optimized out

   * vendor/motorola/
97cb133 athene: derp
814e8e8 athene: add missing permissions
069ea8d athene: apply MM sensor blobs
799f2de athene: don't use qti-telephony-common.jar
d1b1207 athene: fix ril & data
42f0690 fix build

====================
     11-25-2016
====================


   * device/motorola/athene/
80e6eec fix build
af3a84f athene: fingerprint update to latest Soak test NPJ25.75-2 > NPJ25.93-9
09c79f0 athene: overlay: update carrier config
754d38b athene: update proprietary files list
698b399 athene: update from last soak test

   * external/f2fs-tools/
0d18747 libf2fs_fmt: Add missing src file

   * packages/apps/PhoneCommon/
430d7ca Automatic translation import

   * packages/providers/DownloadProvider/
aee1af3 Automatic translation import

   * vendor/aoscp/
cd174dc Bring cheesecake to kenzo :) - Welcome Redmi Note 3 (kenzo)

   * vendor/motorola/
42f0690 fix build
42abc4d athene: update from last N soak
====================
     11-24-2016
====================


   * external/libnfc-nci/
3a0daa8 libnfc-nci: set NXP_CHIP_TYPE based on BOARD_NFC_CHIPSET

   * external/toybox/
97ad7b2 toybox: Remove -e from @echo

   * external/vim/
702ccbe vim: kill colors

   * frameworks/base/
d46136b Merge "Upadate Italian Translation" into n7.1

   * packages/apps/Bluetooth/
523d4ec Automatic translation import

   * packages/apps/Calendar/
f0333d7 Automatic translation import

   * packages/apps/Dialer/
dad5de1 Automatic translation import

   * packages/apps/PhoneCommon/
0f4466a Automatic translation import

   * packages/providers/DownloadProvider/
9a8fb27 Automatic translation import

   * vendor/cmsdk/
1c65ef7 PerformanceManager: Fix power hint values

====================
     11-23-2016
====================


   * external/openssh/
613dd5c Merge branch 'master' of https://android.googlesource.com/platform/external/openssh into cm-14.1

   * packages/apps/Camera2/
566dafc Automatic translation import

   * packages/apps/Camero/
2454874 Merge changes I9474219c,I51e0a5c9,I69232e4f,Ib0a63f86,Iac39b930, ... into n7.1-dev

   * packages/apps/CellBroadcastReceiver/
69e754d Automatic translation import

   * packages/apps/Contacts/
31c6ef5 Automatic translation import

   * packages/apps/ContactsCommon/
b9e413b Automatic translation import

   * packages/apps/DeskClock/
2cb0615 Automatic translation import

   * packages/apps/ExactCalculator/
677ff23 Automatic translation import

   * packages/apps/Gallery2/
f13eaf7 Automatic translation import

   * packages/apps/Nfc/
bdd0352 Automatic translation import

   * packages/apps/SafetyRegulatoryInfo/
884079c Automatic translation import

   * packages/apps/Settings/
ab49bd8 Settings: Small cleanup

   * packages/apps/SoundRecorder/
de75853 Automatic translation import

   * packages/apps/Stk/
19af7b3 Automatic translation import

   * packages/apps/Terminal/
1127958 Automatic translation import

   * packages/apps/TvSettings/
e7aa3df Automatic translation import

   * packages/inputmethods/LatinIME/
5bb754f Automatic translation import

   * packages/providers/CalendarProvider/
a37b133 Automatic translation import

   * packages/providers/CallLogProvider/
68557e2 Automatic translation import

   * packages/providers/ContactsProvider/
ac1ff69 Automatic translation import

   * packages/providers/MediaProvider/
ba47c2f Automatic translation import

   * packages/providers/TelephonyProvider/
ec791e8 Automatic translation import

   * packages/providers/UserDictionaryProvider/
0d59b58 Automatic translation import

   * packages/screensavers/Basic/
7d8b698 Automatic translation import

   * packages/screensavers/PhotoTable/
c412483 Automatic translation import

   * packages/services/Telecomm/
9cf0e3b Automatic translation import

   * packages/wallpapers/LivePicker/
566f4a0 Automatic translation import

   * vendor/aoscp/
b478271 Merge "vendor: Remove unneeded 'endif'" into n7.1

====================
     11-22-2016
====================


   * device/motorola/athene/
c699c6a Merge changes Ic3ab7bac,Ib011fcdd,Ifeaab563 into n7.1

   * kernel/motorola/msm8952/
b6f2606 athene: disable fp as home button (reverted from commit 184efa90ca91241802419cde86ad3f2f32df7eb9)

   * platform_manifest/
7276976 Revert "manifest: stop tracking Camera2" Track Camera2 : Start tracking camera2 Some devices like kenzo having camera switching and vide recording working better only in camera2 Other camera apps are crashing, let's users give a choice to use camero & camera2 until we fix it.

====================
     11-21-2016
====================


   * device/qcom/common/
680823c qcom: extractors: Add msm8960 graphics list

   * device/qcom/sepolicy/
139f082 msm8974: add common sepolicy needed for M blobs on N

   * frameworks/opt/telephony/
14b6666 Update carrier services on EVENT_NV_READY

   * hardware/qcom/media/
068d0fa mm-video: vidc: Remove hardcoding of BufCountActual

====================
     11-20-2016
====================


   * libcore/
77335d6 Modify j.t.DateFormat.set24HourTimePref() to take a Boolean

====================
     11-19-2016
====================


   * device/qcom/common/
4b8412d qc: Fix makefiles

   * packages/apps/Settings/
17132ea Update Italian Translation

   * device/motorola/athene/
I93e861   athene:enable flush_merge on userdata
	  athene:cleanup ramdiskk
	  athene:increase touchboost ms	
	  athene: update mount options for user accessable partitions	
	  athene: add some ramdisk tweaks

====================
     11-18-2016
====================


   * device/motorola/athene/
3d754e9 athene: Update CarrierConfig overlay from stock

   * frameworks/base/
4d823ea Merge "QSPanel: Brightness icon switch[2/2]" into n7.1

   * packages/apps/Settings/
e2e889b Settings: Fix device storage menu when using Adopted Storage

   * platform_manifest/
6c0ce25 Merge "manifest: track Camero's dev branch" into n7.1

   * vendor/aoscp/
b3143d4 Merge changes Ibba28bfe,I11568ce5 into n7.1

   * vendor/motorola/
e3e5f35 Revert: athene: omx: use stock N libs (reverted from commit e52865f05729686e3c061f70131a6fa8c103ea4a)


====================
     11-17-2016
====================


   * device/motorola/athene/
2dfe23b athene:tweak power config a little bit
        athene:add osprey liblights

   * packages/apps/Settings/
fc797ae Merge changes I8076bccf,I21dd6c25 into n7.1

   * vendor/aoscp/
589cea3 vendor: add required props for Google SetupWizard


====================
     11-16-2016
====================


   * frameworks/base/
e583316 Update Polish Translation

   * hardware/qcom/media/
0124a88 media: Add missing links

   * packages/apps/Bluetooth/
168ecad bluetooth: Prevent null pointer crashes in A2DP initNative

   * packages/apps/COTA/
7fea794 Cota: Update imageview to display correctly

   * frameworks/base/
cc194e9 Merge "Fwb: [SQUASH] Battery styles [2/2]" into n7.1

   * hardware/qcom/media/
1a4a797 Update qcom-media    * path guard

   * packages/apps/Dialer/
30c87de Clean up volume boost button logic.

   * platform_manifest/
123cf04 Merge "manifest: stop tracking Camera2" into n7.1

====================
     11-15-2016
====================


   * build/
6870728 build: Remove unneeded endif

   * packages/apps/Settings/
38a8c2c Settings: Battery styles [1/2]

   * packages/services/Telecomm/
b115d74 Telecom: Ues proper sub IDs

   * packages/services/Telephony/
4776eac PhoneUtils: Drop support for DSDA

   * system/core/
7e3a4d5 init: Fix possible open file pointer

   * vendor/aoscp/
da98900 devices: add support for Moto G4 Plus (Athene)

====================
     11-14-2016
====================


   * frameworks/opt/net/wifi/
a5190f3 WifiQualifiedNetworkSelector: turn down the logspam

   * kernel/motorola/msm8952/
6de8a8c athene: disable evbug module

   * packages/inputmethods/LatinIME/
c356a1d LatinIME: disable sound on keypress on all devices by default

====================
     11-13-2016
====================


   * external/fsck_msdos/
674d58f fsck_msdos: Don't use Snapdragon LLVM

====================
     11-12-2016
====================


   * frameworks/av/
c1382b7 OMXNodeInstance: Fix legacy HAL1 after merge of android-7.1.0_r7

   * packages/apps/Camero/
49d524f Camera: Initial bringup

   * packages/apps/Contacts/
45d4272 Fix NPE when 'merge contacts' encounters unknown names.

   * prebuilts/snapdragon-llvm/toolchains/llvm-Snapdragon_LLVM_for_Android_3.8/prebuilt/linux-x86_64//
7f4cfb9 Qcom LLVM

====================
     11-09-2016
====================


   * bootable/recovery/
de8de5f Constrain log text output to bottom quarter of the screen.

   * device/motorola/athene/
ef78a04 sepolicy: it never ends

   * frameworks/base/
6afec1e Fix left clock padding

   * hardware/qcom/audio-caf/msm8996/
0feef69 Revert "hal: Add abstraction for soundtrigger session"

   * kernel/motorola/msm8952/
adef65a Revert: security/selinux: force permissive

   * vendor/cmsdk/
1cc7931 CMSettingsProvider: Fix instance of provider class

====================
     11-08-2016
====================


   * frameworks/av/
fdde5b2 Camera: Support obtaining camera memory from MemoryHeapIon

   * frameworks/native/
d7b29fa binder: Squashed commit of MemoryHeapBaseIon

   * frameworks/opt/setupwizard/
b9dc8b2 Fix setupwizard crashes for tablets

   * frameworks/opt/telephony/
ec18aba Add dummy SUB record in CDMA NV mode

   * hardware/ril-caf/
03a5a1d Properly parcel v6 RIL_CellInfo GSM cell response.

   * packages/apps/Dialer/
1e5c3de Re-add call recording feature.

   * packages/apps/Settings/
efe1892 Fixing things

   * packages/services/Telephony/
0a86af6 Telephony: Redirect to roaming SIM network setting(Dual SIM)

   * prebuilts/cmsdk/
3f6383f No idea why I need this all the suddon, well here it is

   * system/bt/
7924a32 bt: Use HCI H4 HAL for BT SOC ATH3K

   * vendor/aoscp/
153b1fb vendor: cm: Move fuseblk to system/sepolicy

   * vendor/motorola/
e52865f athene: omx: use stock N libs

====================
     11-07-2016
====================


   * build/
b556050 OtaFromTargetFiles: Properly include override_prop

   * hardware/intel/img/hwcomposer/
09c4a9b intel: hwcomposer: csc mode is only supported on newer blobs

   * packages/apps/CarrierConfig/
0af4ed4 Resolve NZ roaming entry

   * packages/apps/Contacts/
bb83402 [1/2] Contacts: make shapes great again

   * packages/apps/ContactsCommon/
0da306c [2/2] ContactsCommon: make shapes great again

   * packages/services/Telecomm/
529106c Fix sporadic crashes with MSIM devices and inactive SIMs

   * platform_manifest/
3f2f491 For the confused children

   * system/sepolicy/
a35663a Add rules required for TARGET_HAS_LEGACY_CAMERA_HAL1

====================
     11-06-2016
====================


   * packages/apps/COTA/
ad28af7 Cota: Updates for 7.1 Nougat

====================
     11-05-2016
====================


   * frameworks/opt/net/wifi/
8594d48 wifi: Set the mode at native layer

   * hardware/qcom/media-caf/msm8974/
79be6bb Remove leftover QCMediaPlayer files
