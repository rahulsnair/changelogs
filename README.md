====================
     11-19-2016
====================


   * device/qcom/common/
4b8412d qc: Fix makefiles

   * packages/apps/Settings/
17132ea Update Italian Translation

   * device/motorola/athene/
   - 	athene:enable flush_merge on userdata
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
