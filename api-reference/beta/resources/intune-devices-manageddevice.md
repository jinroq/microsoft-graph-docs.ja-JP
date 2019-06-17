---
title: managedDevice リソース タイプ
description: Intune 経由で管理または事前登録されるデバイス
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3ee7fd96654fe0b6c2a95332b87287d3ebff3ad2
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995120"
---
# <a name="manageddevice-resource-type"></a><span data-ttu-id="0e17c-103">managedDevice リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="0e17c-103">managedDevice resource type</span></span>

> <span data-ttu-id="0e17c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0e17c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e17c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0e17c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e17c-106">Intune 経由で管理または事前登録されるデバイス</span><span class="sxs-lookup"><span data-stu-id="0e17c-106">Devices that are managed or pre-enrolled through Intune</span></span>

## <a name="methods"></a><span data-ttu-id="0e17c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="0e17c-107">Methods</span></span>
|<span data-ttu-id="0e17c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0e17c-108">Method</span></span>|<span data-ttu-id="0e17c-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0e17c-109">Return Type</span></span>|<span data-ttu-id="0e17c-110">説明</span><span class="sxs-lookup"><span data-stu-id="0e17c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0e17c-111">Get managedDevice</span><span class="sxs-lookup"><span data-stu-id="0e17c-111">Get managedDevice</span></span>](../api/intune-devices-manageddevice-get.md)|[<span data-ttu-id="0e17c-112">managedDevice</span><span class="sxs-lookup"><span data-stu-id="0e17c-112">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="0e17c-113">[managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0e17c-113">Read properties and relationships of the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="0e17c-114">Update managedDevice</span><span class="sxs-lookup"><span data-stu-id="0e17c-114">Update managedDevice</span></span>](../api/intune-devices-manageddevice-update.md)|[<span data-ttu-id="0e17c-115">managedDevice</span><span class="sxs-lookup"><span data-stu-id="0e17c-115">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="0e17c-116">[managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0e17c-116">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="0e17c-117">executeAction アクション</span><span class="sxs-lookup"><span data-stu-id="0e17c-117">executeAction action</span></span>](../api/intune-devices-manageddevice-executeaction.md)|[<span data-ttu-id="0e17c-118">bulkManagedDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="0e17c-118">bulkManagedDeviceActionResult</span></span>](../resources/intune-devices-bulkmanageddeviceactionresult.md)|<span data-ttu-id="0e17c-119">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0e17c-119">Not yet documented</span></span>|
|[<span data-ttu-id="0e17c-120">enableLostMode アクション</span><span class="sxs-lookup"><span data-stu-id="0e17c-120">enableLostMode action</span></span>](../api/intune-devices-manageddevice-enablelostmode.md)|<span data-ttu-id="0e17c-121">None</span><span class="sxs-lookup"><span data-stu-id="0e17c-121">None</span></span>|<span data-ttu-id="0e17c-122">削除モードを有効にする</span><span class="sxs-lookup"><span data-stu-id="0e17c-122">Enable lost mode</span></span>|
|[<span data-ttu-id="0e17c-123">playLostModeSound アクション</span><span class="sxs-lookup"><span data-stu-id="0e17c-123">playLostModeSound action</span></span>](../api/intune-devices-manageddevice-playlostmodesound.md)|<span data-ttu-id="0e17c-124">None</span><span class="sxs-lookup"><span data-stu-id="0e17c-124">None</span></span>|<span data-ttu-id="0e17c-125">リモート ロック</span><span class="sxs-lookup"><span data-stu-id="0e17c-125">Remote lock</span></span>|
|[<span data-ttu-id="0e17c-126">setDeviceName アクション</span><span class="sxs-lookup"><span data-stu-id="0e17c-126">setDeviceName action</span></span>](../api/intune-devices-manageddevice-setdevicename.md)|<span data-ttu-id="0e17c-127">None</span><span class="sxs-lookup"><span data-stu-id="0e17c-127">None</span></span>|<span data-ttu-id="0e17c-128">デバイスのデバイス名を設定します。</span><span class="sxs-lookup"><span data-stu-id="0e17c-128">Set device name of the device.</span></span>|
|[<span data-ttu-id="0e17c-129">rotateFileVaultKey アクション</span><span class="sxs-lookup"><span data-stu-id="0e17c-129">rotateFileVaultKey action</span></span>](../api/intune-devices-manageddevice-rotatefilevaultkey.md)|<span data-ttu-id="0e17c-130">None</span><span class="sxs-lookup"><span data-stu-id="0e17c-130">None</span></span>|<span data-ttu-id="0e17c-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0e17c-131">Not yet documented</span></span>|
|[<span data-ttu-id="0e17c-132">getFileVaultKey 関数</span><span class="sxs-lookup"><span data-stu-id="0e17c-132">getFileVaultKey function</span></span>](../api/intune-devices-manageddevice-getfilevaultkey.md)|<span data-ttu-id="0e17c-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="0e17c-133">String</span></span>|<span data-ttu-id="0e17c-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0e17c-134">Not yet documented</span></span>|
|[<span data-ttu-id="0e17c-135">retire action</span><span class="sxs-lookup"><span data-stu-id="0e17c-135">retire action</span></span>](../api/intune-devices-manageddevice-retire.md)|<span data-ttu-id="0e17c-136">None</span><span class="sxs-lookup"><span data-stu-id="0e17c-136">None</span></span>|<span data-ttu-id="0e17c-137">デバイスを破棄します</span><span class="sxs-lookup"><span data-stu-id="0e17c-137">Retire a device</span></span>|
|[<span data-ttu-id="0e17c-138">wipe action</span><span class="sxs-lookup"><span data-stu-id="0e17c-138">wipe action</span></span>](../api/intune-devices-manageddevice-wipe.md)|<span data-ttu-id="0e17c-139">None</span><span class="sxs-lookup"><span data-stu-id="0e17c-139">None</span></span>|<span data-ttu-id="0e17c-140">デバイスをワイプします</span><span class="sxs-lookup"><span data-stu-id="0e17c-140">Wipe a device</span></span>|
|[<span data-ttu-id="0e17c-141">resetPasscode action</span><span class="sxs-lookup"><span data-stu-id="0e17c-141">resetPasscode action</span></span>](../api/intune-devices-manageddevice-resetpasscode.md)|<span data-ttu-id="0e17c-142">None</span><span class="sxs-lookup"><span data-stu-id="0e17c-142">None</span></span>|<span data-ttu-id="0e17c-143">パスコードをリセットします</span><span class="sxs-lookup"><span data-stu-id="0e17c-143">Reset passcode</span></span>|
|[<span data-ttu-id="0e17c-144">remoteLock action</span><span class="sxs-lookup"><span data-stu-id="0e17c-144">remoteLock action</span></span>](../api/intune-devices-manageddevice-remotelock.md)|<span data-ttu-id="0e17c-145">None</span><span class="sxs-lookup"><span data-stu-id="0e17c-145">None</span></span>|<span data-ttu-id="0e17c-146">リモート ロック</span><span class="sxs-lookup"><span data-stu-id="0e17c-146">Remote lock</span></span>|
|[<span data-ttu-id="0e17c-147">requestRemoteAssistance action</span><span class="sxs-lookup"><span data-stu-id="0e17c-147">requestRemoteAssistance action</span></span>](../api/intune-devices-manageddevice-requestremoteassistance.md)|<span data-ttu-id="0e17c-148">None</span><span class="sxs-lookup"><span data-stu-id="0e17c-148">None</span></span>|<span data-ttu-id="0e17c-149">リモート アシスタンスを要求します</span><span class="sxs-lookup"><span data-stu-id="0e17c-149">Request remote assistance</span></span>|
|[<span data-ttu-id="0e17c-150">disableLostMode action</span><span class="sxs-lookup"><span data-stu-id="0e17c-150">disableLostMode action</span></span>](../api/intune-devices-manageddevice-disablelostmode.md)|<span data-ttu-id="0e17c-151">None</span><span class="sxs-lookup"><span data-stu-id="0e17c-151">None</span></span>|<span data-ttu-id="0e17c-152">紛失モードを無効化します</span><span class="sxs-lookup"><span data-stu-id="0e17c-152">Disable lost mode</span></span>|
|[<span data-ttu-id="0e17c-153">locateDevice action</span><span class="sxs-lookup"><span data-stu-id="0e17c-153">locateDevice action</span></span>](../api/intune-devices-manageddevice-locatedevice.md)|<span data-ttu-id="0e17c-154">None</span><span class="sxs-lookup"><span data-stu-id="0e17c-154">None</span></span>|<span data-ttu-id="0e17c-155">デバイスを検索します</span><span class="sxs-lookup"><span data-stu-id="0e17c-155">Locate a device</span></span>|
|[<span data-ttu-id="0e17c-156">bypassActivationLock action</span><span class="sxs-lookup"><span data-stu-id="0e17c-156">bypassActivationLock action</span></span>](../api/intune-devices-manageddevice-bypassactivationlock.md)|<span data-ttu-id="0e17c-157">None</span><span class="sxs-lookup"><span data-stu-id="0e17c-157">None</span></span>|<span data-ttu-id="0e17c-158">アクティベーション ロックをバイパスします</span><span class="sxs-lookup"><span data-stu-id="0e17c-158">Bypass activation lock</span></span>|
|[<span data-ttu-id="0e17c-159">rebootNow action</span><span class="sxs-lookup"><span data-stu-id="0e17c-159">rebootNow action</span></span>](../api/intune-devices-manageddevice-rebootnow.md)|<span data-ttu-id="0e17c-160">None</span><span class="sxs-lookup"><span data-stu-id="0e17c-160">None</span></span>|<span data-ttu-id="0e17c-161">デバイスを再起動します</span><span class="sxs-lookup"><span data-stu-id="0e17c-161">Reboot device</span></span>|
|[<span data-ttu-id="0e17c-162">shutDown action</span><span class="sxs-lookup"><span data-stu-id="0e17c-162">shutDown action</span></span>](../api/intune-devices-manageddevice-shutdown.md)|<span data-ttu-id="0e17c-163">None</span><span class="sxs-lookup"><span data-stu-id="0e17c-163">None</span></span>|<span data-ttu-id="0e17c-164">デバイスをシャットダウンします</span><span class="sxs-lookup"><span data-stu-id="0e17c-164">Shut down device</span></span>|
|[<span data-ttu-id="0e17c-165">recoverPasscode action</span><span class="sxs-lookup"><span data-stu-id="0e17c-165">recoverPasscode action</span></span>](../api/intune-devices-manageddevice-recoverpasscode.md)|<span data-ttu-id="0e17c-166">None</span><span class="sxs-lookup"><span data-stu-id="0e17c-166">None</span></span>|<span data-ttu-id="0e17c-167">パスコードを回復します</span><span class="sxs-lookup"><span data-stu-id="0e17c-167">Recover passcode</span></span>|
|[<span data-ttu-id="0e17c-168">cleanWindowsDevice action</span><span class="sxs-lookup"><span data-stu-id="0e17c-168">cleanWindowsDevice action</span></span>](../api/intune-devices-manageddevice-cleanwindowsdevice.md)|<span data-ttu-id="0e17c-169">None</span><span class="sxs-lookup"><span data-stu-id="0e17c-169">None</span></span>|<span data-ttu-id="0e17c-170">Windows デバイスをクリーンにします</span><span class="sxs-lookup"><span data-stu-id="0e17c-170">Clean Windows device</span></span>|
|[<span data-ttu-id="0e17c-171">logoutSharedAppleDeviceActiveUser action</span><span class="sxs-lookup"><span data-stu-id="0e17c-171">logoutSharedAppleDeviceActiveUser action</span></span>](../api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser.md)|<span data-ttu-id="0e17c-172">None</span><span class="sxs-lookup"><span data-stu-id="0e17c-172">None</span></span>|<span data-ttu-id="0e17c-173">共有の Apple デバイスのアクティブなユーザーをログアウトします</span><span class="sxs-lookup"><span data-stu-id="0e17c-173">Logout shared Apple device active user</span></span>|
|[<span data-ttu-id="0e17c-174">deleteUserFromSharedAppleDevice action</span><span class="sxs-lookup"><span data-stu-id="0e17c-174">deleteUserFromSharedAppleDevice action</span></span>](../api/intune-devices-manageddevice-deleteuserfromsharedappledevice.md)|<span data-ttu-id="0e17c-175">なし</span><span class="sxs-lookup"><span data-stu-id="0e17c-175">None</span></span>|<span data-ttu-id="0e17c-176">共有の Apple デバイスからユーザーを削除します</span><span class="sxs-lookup"><span data-stu-id="0e17c-176">Delete user from shared Apple device</span></span>|
|[<span data-ttu-id="0e17c-177">syncDevice action</span><span class="sxs-lookup"><span data-stu-id="0e17c-177">syncDevice action</span></span>](../api/intune-devices-manageddevice-syncdevice.md)|<span data-ttu-id="0e17c-178">None</span><span class="sxs-lookup"><span data-stu-id="0e17c-178">None</span></span>|<span data-ttu-id="0e17c-179">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0e17c-179">Not yet documented</span></span>|
|[<span data-ttu-id="0e17c-180">windowsDefenderScan action</span><span class="sxs-lookup"><span data-stu-id="0e17c-180">windowsDefenderScan action</span></span>](../api/intune-devices-manageddevice-windowsdefenderscan.md)|<span data-ttu-id="0e17c-181">None</span><span class="sxs-lookup"><span data-stu-id="0e17c-181">None</span></span>|<span data-ttu-id="0e17c-182">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0e17c-182">Not yet documented</span></span>|
|[<span data-ttu-id="0e17c-183">windowsDefenderUpdateSignatures action</span><span class="sxs-lookup"><span data-stu-id="0e17c-183">windowsDefenderUpdateSignatures action</span></span>](../api/intune-devices-manageddevice-windowsdefenderupdatesignatures.md)|<span data-ttu-id="0e17c-184">None</span><span class="sxs-lookup"><span data-stu-id="0e17c-184">None</span></span>|<span data-ttu-id="0e17c-185">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0e17c-185">Not yet documented</span></span>|
|[<span data-ttu-id="0e17c-186">updateWindowsDeviceAccount action</span><span class="sxs-lookup"><span data-stu-id="0e17c-186">updateWindowsDeviceAccount action</span></span>](../api/intune-devices-manageddevice-updatewindowsdeviceaccount.md)|<span data-ttu-id="0e17c-187">なし</span><span class="sxs-lookup"><span data-stu-id="0e17c-187">None</span></span>|<span data-ttu-id="0e17c-188">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0e17c-188">Not yet documented</span></span>|
|[<span data-ttu-id="0e17c-189">revokeAppleVppLicenses アクション</span><span class="sxs-lookup"><span data-stu-id="0e17c-189">revokeAppleVppLicenses action</span></span>](../api/intune-devices-manageddevice-revokeapplevpplicenses.md)|<span data-ttu-id="0e17c-190">None</span><span class="sxs-lookup"><span data-stu-id="0e17c-190">None</span></span>|<span data-ttu-id="0e17c-191">デバイスのすべての Apple Vpp ライセンスを取り消す</span><span class="sxs-lookup"><span data-stu-id="0e17c-191">Revoke all Apple Vpp licenses for a device</span></span>|

## <a name="properties"></a><span data-ttu-id="0e17c-192">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e17c-192">Properties</span></span>
|<span data-ttu-id="0e17c-193">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e17c-193">Property</span></span>|<span data-ttu-id="0e17c-194">型</span><span class="sxs-lookup"><span data-stu-id="0e17c-194">Type</span></span>|<span data-ttu-id="0e17c-195">説明</span><span class="sxs-lookup"><span data-stu-id="0e17c-195">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e17c-196">id</span><span class="sxs-lookup"><span data-stu-id="0e17c-196">id</span></span>|<span data-ttu-id="0e17c-197">文字列</span><span class="sxs-lookup"><span data-stu-id="0e17c-197">String</span></span>|<span data-ttu-id="0e17c-198">デバイスの一意識別子</span><span class="sxs-lookup"><span data-stu-id="0e17c-198">Unique Identifier for the device</span></span>|
|<span data-ttu-id="0e17c-199">userId</span><span class="sxs-lookup"><span data-stu-id="0e17c-199">userId</span></span>|<span data-ttu-id="0e17c-200">String</span><span class="sxs-lookup"><span data-stu-id="0e17c-200">String</span></span>|<span data-ttu-id="0e17c-201">デバイスに関連付けられているユーザーの一意の識別子</span><span class="sxs-lookup"><span data-stu-id="0e17c-201">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="0e17c-202">deviceName</span><span class="sxs-lookup"><span data-stu-id="0e17c-202">deviceName</span></span>|<span data-ttu-id="0e17c-203">String</span><span class="sxs-lookup"><span data-stu-id="0e17c-203">String</span></span>|<span data-ttu-id="0e17c-204">デバイスの名前</span><span class="sxs-lookup"><span data-stu-id="0e17c-204">Name of the device</span></span>|
|<span data-ttu-id="0e17c-205">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="0e17c-205">hardwareInformation</span></span>|[<span data-ttu-id="0e17c-206">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="0e17c-206">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="0e17c-207">デバイスのハードワードの詳細。</span><span class="sxs-lookup"><span data-stu-id="0e17c-207">The hardward details for the device.</span></span>  <span data-ttu-id="0e17c-208">記憶領域、製造元、シリアル番号などの情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="0e17c-208">Includes information such as storage space, manufacturer, serial number, etc.</span></span>|
|<span data-ttu-id="0e17c-209">ownerType</span><span class="sxs-lookup"><span data-stu-id="0e17c-209">ownerType</span></span>|[<span data-ttu-id="0e17c-210">ownerType</span><span class="sxs-lookup"><span data-stu-id="0e17c-210">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="0e17c-211">デバイスの所有権。</span><span class="sxs-lookup"><span data-stu-id="0e17c-211">Ownership of the device.</span></span> <span data-ttu-id="0e17c-212">' Company ' または ' personal ' にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0e17c-212">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="0e17c-213">可能な値は、`unknown`、`company`、`personal` です。</span><span class="sxs-lookup"><span data-stu-id="0e17c-213">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="0e17c-214">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="0e17c-214">managedDeviceOwnerType</span></span>|[<span data-ttu-id="0e17c-215">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="0e17c-215">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="0e17c-216">デバイスの所有権。</span><span class="sxs-lookup"><span data-stu-id="0e17c-216">Ownership of the device.</span></span> <span data-ttu-id="0e17c-217">' Company ' または ' personal ' にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0e17c-217">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="0e17c-218">可能な値は、`unknown`、`company`、`personal` です。</span><span class="sxs-lookup"><span data-stu-id="0e17c-218">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="0e17c-219">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="0e17c-219">deviceActionResults</span></span>|<span data-ttu-id="0e17c-220">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0e17c-220">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="0e17c-221">ComplexType deviceActionResult オブジェクトのリスト。</span><span class="sxs-lookup"><span data-stu-id="0e17c-221">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="0e17c-222">managementState</span><span class="sxs-lookup"><span data-stu-id="0e17c-222">managementState</span></span>|[<span data-ttu-id="0e17c-223">managementState</span><span class="sxs-lookup"><span data-stu-id="0e17c-223">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="0e17c-224">デバイスの管理状態。</span><span class="sxs-lookup"><span data-stu-id="0e17c-224">Management state of the device.</span></span> <span data-ttu-id="0e17c-225">可能な値は、`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered` です。</span><span class="sxs-lookup"><span data-stu-id="0e17c-225">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="0e17c-226">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="0e17c-226">enrolledDateTime</span></span>|<span data-ttu-id="0e17c-227">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e17c-227">DateTimeOffset</span></span>|<span data-ttu-id="0e17c-228">デバイスの登録時刻。</span><span class="sxs-lookup"><span data-stu-id="0e17c-228">Enrollment time of the device.</span></span>|
|<span data-ttu-id="0e17c-229">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0e17c-229">lastSyncDateTime</span></span>|<span data-ttu-id="0e17c-230">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e17c-230">DateTimeOffset</span></span>|<span data-ttu-id="0e17c-231">デバイスが Intune との正常な同期を最終的に完了した日時。</span><span class="sxs-lookup"><span data-stu-id="0e17c-231">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="0e17c-232">chassisType</span><span class="sxs-lookup"><span data-stu-id="0e17c-232">chassisType</span></span>|[<span data-ttu-id="0e17c-233">chassisType</span><span class="sxs-lookup"><span data-stu-id="0e17c-233">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="0e17c-234">デバイスのシャーシの種類。</span><span class="sxs-lookup"><span data-stu-id="0e17c-234">Chassis type of the device.</span></span> <span data-ttu-id="0e17c-235">可能な値は、`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown` です。</span><span class="sxs-lookup"><span data-stu-id="0e17c-235">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="0e17c-236">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="0e17c-236">operatingSystem</span></span>|<span data-ttu-id="0e17c-237">文字列</span><span class="sxs-lookup"><span data-stu-id="0e17c-237">String</span></span>|<span data-ttu-id="0e17c-238">デバイスのオペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="0e17c-238">Operating system of the device.</span></span> <span data-ttu-id="0e17c-239">Windows、iOS など。</span><span class="sxs-lookup"><span data-stu-id="0e17c-239">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="0e17c-240">deviceType</span><span class="sxs-lookup"><span data-stu-id="0e17c-240">deviceType</span></span>|[<span data-ttu-id="0e17c-241">deviceType</span><span class="sxs-lookup"><span data-stu-id="0e17c-241">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="0e17c-242">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="0e17c-242">Platform of the device.</span></span> <span data-ttu-id="0e17c-243">可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="0e17c-243">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="0e17c-244">complianceState</span><span class="sxs-lookup"><span data-stu-id="0e17c-244">complianceState</span></span>|[<span data-ttu-id="0e17c-245">complianceState</span><span class="sxs-lookup"><span data-stu-id="0e17c-245">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="0e17c-246">デバイスのコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="0e17c-246">Compliance state of the device.</span></span> <span data-ttu-id="0e17c-247">可能な値は、`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager` です。</span><span class="sxs-lookup"><span data-stu-id="0e17c-247">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="0e17c-248">jailBroken</span><span class="sxs-lookup"><span data-stu-id="0e17c-248">jailBroken</span></span>|<span data-ttu-id="0e17c-249">String</span><span class="sxs-lookup"><span data-stu-id="0e17c-249">String</span></span>|<span data-ttu-id="0e17c-250">デバイスが脱獄またはルート化されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0e17c-250">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="0e17c-251">managementAgent</span><span class="sxs-lookup"><span data-stu-id="0e17c-251">managementAgent</span></span>|[<span data-ttu-id="0e17c-252">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="0e17c-252">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="0e17c-253">デバイスの管理チャネル。</span><span class="sxs-lookup"><span data-stu-id="0e17c-253">Management channel of the device.</span></span> <span data-ttu-id="0e17c-254">Intune、EAS など。可能な値は`eas`、 `mdm`、 `easMdm` `intuneClient` `easIntuneClient` `configurationManagerClient` `jamf` `googleCloudDevicePolicyController`、、、、、、、、、 `microsoft365ManagedMdm`、、です。 `configurationManagerClientMdm` `configurationManagerClientMdmEas` `unknown`</span><span class="sxs-lookup"><span data-stu-id="0e17c-254">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="0e17c-255">osVersion</span><span class="sxs-lookup"><span data-stu-id="0e17c-255">osVersion</span></span>|<span data-ttu-id="0e17c-256">String</span><span class="sxs-lookup"><span data-stu-id="0e17c-256">String</span></span>|<span data-ttu-id="0e17c-257">デバイスのオペレーティング システムのバージョン。</span><span class="sxs-lookup"><span data-stu-id="0e17c-257">Operating system version of the device.</span></span>|
|<span data-ttu-id="0e17c-258">easActivated</span><span class="sxs-lookup"><span data-stu-id="0e17c-258">easActivated</span></span>|<span data-ttu-id="0e17c-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e17c-259">Boolean</span></span>|<span data-ttu-id="0e17c-260">Exchange ActiveSync がアクティブになっているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0e17c-260">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="0e17c-261">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="0e17c-261">easDeviceId</span></span>|<span data-ttu-id="0e17c-262">String</span><span class="sxs-lookup"><span data-stu-id="0e17c-262">String</span></span>|<span data-ttu-id="0e17c-263">デバイスの Exchange ActiveSync の ID。</span><span class="sxs-lookup"><span data-stu-id="0e17c-263">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="0e17c-264">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="0e17c-264">easActivationDateTime</span></span>|<span data-ttu-id="0e17c-265">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e17c-265">DateTimeOffset</span></span>|<span data-ttu-id="0e17c-266">デバイスの Exchange ActivationSync のアクティブ化の時刻。</span><span class="sxs-lookup"><span data-stu-id="0e17c-266">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="0e17c-267">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="0e17c-267">aadRegistered</span></span>|<span data-ttu-id="0e17c-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e17c-268">Boolean</span></span>|<span data-ttu-id="0e17c-269">Azure Active Directory が登録されているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0e17c-269">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="0e17c-270">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="0e17c-270">azureADRegistered</span></span>|<span data-ttu-id="0e17c-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e17c-271">Boolean</span></span>|<span data-ttu-id="0e17c-272">Azure Active Directory が登録されているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0e17c-272">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="0e17c-273">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="0e17c-273">deviceEnrollmentType</span></span>|[<span data-ttu-id="0e17c-274">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="0e17c-274">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="0e17c-275">デバイスの登録の種類。</span><span class="sxs-lookup"><span data-stu-id="0e17c-275">Enrollment type of the device.</span></span> <span data-ttu-id="0e17c-276">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="0e17c-276">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="0e17c-277">lostModeState</span><span class="sxs-lookup"><span data-stu-id="0e17c-277">lostModeState</span></span>|[<span data-ttu-id="0e17c-278">lostModeState</span><span class="sxs-lookup"><span data-stu-id="0e17c-278">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="0e17c-279">失われたモードが有効か無効かを示します。</span><span class="sxs-lookup"><span data-stu-id="0e17c-279">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="0e17c-280">可能な値は、`disabled`、`enabled` です。</span><span class="sxs-lookup"><span data-stu-id="0e17c-280">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="0e17c-281">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="0e17c-281">activationLockBypassCode</span></span>|<span data-ttu-id="0e17c-282">String</span><span class="sxs-lookup"><span data-stu-id="0e17c-282">String</span></span>|<span data-ttu-id="0e17c-283">デバイスのアクティベーション ロックをバイパスするためのコード。</span><span class="sxs-lookup"><span data-stu-id="0e17c-283">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="0e17c-284">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0e17c-284">emailAddress</span></span>|<span data-ttu-id="0e17c-285">String</span><span class="sxs-lookup"><span data-stu-id="0e17c-285">String</span></span>|<span data-ttu-id="0e17c-286">デバイスに関連付けられているユーザーの電子メール</span><span class="sxs-lookup"><span data-stu-id="0e17c-286">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="0e17c-287">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="0e17c-287">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="0e17c-288">String</span><span class="sxs-lookup"><span data-stu-id="0e17c-288">String</span></span>|<span data-ttu-id="0e17c-289">Azure Active Directory デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="0e17c-289">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="0e17c-290">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0e17c-290">Read only.</span></span>|
|<span data-ttu-id="0e17c-291">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="0e17c-291">azureADDeviceId</span></span>|<span data-ttu-id="0e17c-292">String</span><span class="sxs-lookup"><span data-stu-id="0e17c-292">String</span></span>|<span data-ttu-id="0e17c-293">Azure Active Directory デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="0e17c-293">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="0e17c-294">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0e17c-294">Read only.</span></span>|
|<span data-ttu-id="0e17c-295">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="0e17c-295">deviceRegistrationState</span></span>|[<span data-ttu-id="0e17c-296">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="0e17c-296">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="0e17c-297">デバイスの登録状態。</span><span class="sxs-lookup"><span data-stu-id="0e17c-297">Device registration state.</span></span> <span data-ttu-id="0e17c-298">可能な値は、`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="0e17c-298">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="0e17c-299">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="0e17c-299">deviceCategoryDisplayName</span></span>|<span data-ttu-id="0e17c-300">String</span><span class="sxs-lookup"><span data-stu-id="0e17c-300">String</span></span>|<span data-ttu-id="0e17c-301">デバイス カテゴリの表示名</span><span class="sxs-lookup"><span data-stu-id="0e17c-301">Device category display name</span></span>|
|<span data-ttu-id="0e17c-302">isSupervised</span><span class="sxs-lookup"><span data-stu-id="0e17c-302">isSupervised</span></span>|<span data-ttu-id="0e17c-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e17c-303">Boolean</span></span>|<span data-ttu-id="0e17c-304">デバイスの管理状況</span><span class="sxs-lookup"><span data-stu-id="0e17c-304">Device supervised status</span></span>|
|<span data-ttu-id="0e17c-305">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0e17c-305">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="0e17c-306">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e17c-306">DateTimeOffset</span></span>|<span data-ttu-id="0e17c-307">最後にデバイスが Exchange に接続した時刻。</span><span class="sxs-lookup"><span data-stu-id="0e17c-307">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="0e17c-308">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="0e17c-308">exchangeAccessState</span></span>|[<span data-ttu-id="0e17c-309">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="0e17c-309">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="0e17c-310">Exchange でのデバイスのアクセスの状態。</span><span class="sxs-lookup"><span data-stu-id="0e17c-310">The Access State of the device in Exchange.</span></span> <span data-ttu-id="0e17c-311">可能な値は、`none`、`unknown`、`allowed`、`blocked`、`quarantined` です。</span><span class="sxs-lookup"><span data-stu-id="0e17c-311">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="0e17c-312">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="0e17c-312">exchangeAccessStateReason</span></span>|[<span data-ttu-id="0e17c-313">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="0e17c-313">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="0e17c-314">Exchange でのデバイスのアクセス状態の理由。
</span><span class="sxs-lookup"><span data-stu-id="0e17c-314">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="0e17c-315">可能な値は、`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp` です。</span><span class="sxs-lookup"><span data-stu-id="0e17c-315">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="0e17c-316">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="0e17c-316">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="0e17c-317">String</span><span class="sxs-lookup"><span data-stu-id="0e17c-317">String</span></span>|<span data-ttu-id="0e17c-318">デバイスとのリモート アシスタンス セッションを確立できるようにする URL。</span><span class="sxs-lookup"><span data-stu-id="0e17c-318">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="0e17c-319">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="0e17c-319">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="0e17c-320">String</span><span class="sxs-lookup"><span data-stu-id="0e17c-320">String</span></span>|<span data-ttu-id="0e17c-321">リモート アシスタンス セッション オブジェクトの作成時に問題を識別するエラー文字列。</span><span class="sxs-lookup"><span data-stu-id="0e17c-321">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="0e17c-322">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="0e17c-322">isEncrypted</span></span>|<span data-ttu-id="0e17c-323">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e17c-323">Boolean</span></span>|<span data-ttu-id="0e17c-324">デバイスの暗号化の状態</span><span class="sxs-lookup"><span data-stu-id="0e17c-324">Device encryption status</span></span>|
|<span data-ttu-id="0e17c-325">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0e17c-325">userPrincipalName</span></span>|<span data-ttu-id="0e17c-326">String</span><span class="sxs-lookup"><span data-stu-id="0e17c-326">String</span></span>|<span data-ttu-id="0e17c-327">デバイスのユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="0e17c-327">Device user principal name</span></span>|
|<span data-ttu-id="0e17c-328">model</span><span class="sxs-lookup"><span data-stu-id="0e17c-328">model</span></span>|<span data-ttu-id="0e17c-329">String</span><span class="sxs-lookup"><span data-stu-id="0e17c-329">String</span></span>|<span data-ttu-id="0e17c-330">デバイスのモデル</span><span class="sxs-lookup"><span data-stu-id="0e17c-330">Model of the device</span></span>|
|<span data-ttu-id="0e17c-331">manufacturer</span><span class="sxs-lookup"><span data-stu-id="0e17c-331">manufacturer</span></span>|<span data-ttu-id="0e17c-332">String</span><span class="sxs-lookup"><span data-stu-id="0e17c-332">String</span></span>|<span data-ttu-id="0e17c-333">デバイスのメーカー</span><span class="sxs-lookup"><span data-stu-id="0e17c-333">Manufacturer of the device</span></span>|
|<span data-ttu-id="0e17c-334">imei</span><span class="sxs-lookup"><span data-stu-id="0e17c-334">imei</span></span>|<span data-ttu-id="0e17c-335">String</span><span class="sxs-lookup"><span data-stu-id="0e17c-335">String</span></span>|<span data-ttu-id="0e17c-336">IMEI</span><span class="sxs-lookup"><span data-stu-id="0e17c-336">IMEI</span></span>|
|<span data-ttu-id="0e17c-337">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0e17c-337">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="0e17c-338">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e17c-338">DateTimeOffset</span></span>|<span data-ttu-id="0e17c-339">デバイス コンプライアンスの猶予期間が経過する DateTime</span><span class="sxs-lookup"><span data-stu-id="0e17c-339">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="0e17c-340">serialNumber</span><span class="sxs-lookup"><span data-stu-id="0e17c-340">serialNumber</span></span>|<span data-ttu-id="0e17c-341">String</span><span class="sxs-lookup"><span data-stu-id="0e17c-341">String</span></span>|<span data-ttu-id="0e17c-342">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="0e17c-342">SerialNumber</span></span>|
|<span data-ttu-id="0e17c-343">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="0e17c-343">phoneNumber</span></span>|<span data-ttu-id="0e17c-344">String</span><span class="sxs-lookup"><span data-stu-id="0e17c-344">String</span></span>|<span data-ttu-id="0e17c-345">デバイスの電話番号</span><span class="sxs-lookup"><span data-stu-id="0e17c-345">Phone number of the device</span></span>|
|<span data-ttu-id="0e17c-346">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="0e17c-346">androidSecurityPatchLevel</span></span>|<span data-ttu-id="0e17c-347">String</span><span class="sxs-lookup"><span data-stu-id="0e17c-347">String</span></span>|<span data-ttu-id="0e17c-348">Android セキュリティ パッチのレベル</span><span class="sxs-lookup"><span data-stu-id="0e17c-348">Android security patch level</span></span>|
|<span data-ttu-id="0e17c-349">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="0e17c-349">userDisplayName</span></span>|<span data-ttu-id="0e17c-350">String</span><span class="sxs-lookup"><span data-stu-id="0e17c-350">String</span></span>|<span data-ttu-id="0e17c-351">ユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="0e17c-351">User display name</span></span>|
|<span data-ttu-id="0e17c-352">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="0e17c-352">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="0e17c-353">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="0e17c-353">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="0e17c-354">ConfigrMgr クライアント対応機能
</span><span class="sxs-lookup"><span data-stu-id="0e17c-354">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="0e17c-355">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="0e17c-355">wiFiMacAddress</span></span>|<span data-ttu-id="0e17c-356">String</span><span class="sxs-lookup"><span data-stu-id="0e17c-356">String</span></span>|<span data-ttu-id="0e17c-357">Wi-Fi MAC</span><span class="sxs-lookup"><span data-stu-id="0e17c-357">Wi-Fi MAC</span></span>|
|<span data-ttu-id="0e17c-358">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="0e17c-358">deviceHealthAttestationState</span></span>|[<span data-ttu-id="0e17c-359">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="0e17c-359">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="0e17c-360">デバイスの正常性構成証明の状態。</span><span class="sxs-lookup"><span data-stu-id="0e17c-360">The device health attestation state.</span></span>|
|<span data-ttu-id="0e17c-361">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="0e17c-361">subscriberCarrier</span></span>|<span data-ttu-id="0e17c-362">String</span><span class="sxs-lookup"><span data-stu-id="0e17c-362">String</span></span>|<span data-ttu-id="0e17c-363">サブスクライバー通信事業者</span><span class="sxs-lookup"><span data-stu-id="0e17c-363">Subscriber Carrier</span></span>|
|<span data-ttu-id="0e17c-364">meid</span><span class="sxs-lookup"><span data-stu-id="0e17c-364">meid</span></span>|<span data-ttu-id="0e17c-365">String</span><span class="sxs-lookup"><span data-stu-id="0e17c-365">String</span></span>|<span data-ttu-id="0e17c-366">MEID</span><span class="sxs-lookup"><span data-stu-id="0e17c-366">MEID</span></span>|
|<span data-ttu-id="0e17c-367">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="0e17c-367">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="0e17c-368">Int64</span><span class="sxs-lookup"><span data-stu-id="0e17c-368">Int64</span></span>|<span data-ttu-id="0e17c-369">記憶域の合計 (バイト)</span><span class="sxs-lookup"><span data-stu-id="0e17c-369">Total Storage in Bytes</span></span>|
|<span data-ttu-id="0e17c-370">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="0e17c-370">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="0e17c-371">Int64</span><span class="sxs-lookup"><span data-stu-id="0e17c-371">Int64</span></span>|<span data-ttu-id="0e17c-372">空き記憶域 (バイト)</span><span class="sxs-lookup"><span data-stu-id="0e17c-372">Free Storage in Bytes</span></span>|
|<span data-ttu-id="0e17c-373">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="0e17c-373">managedDeviceName</span></span>|<span data-ttu-id="0e17c-374">String</span><span class="sxs-lookup"><span data-stu-id="0e17c-374">String</span></span>|<span data-ttu-id="0e17c-375">デバイスを識別する名前が自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="0e17c-375">Automatically generated name to identify a device.</span></span> <span data-ttu-id="0e17c-376">ユーザー フレンドリ名に上書きできます。</span><span class="sxs-lookup"><span data-stu-id="0e17c-376">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="0e17c-377">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="0e17c-377">partnerReportedThreatState</span></span>|[<span data-ttu-id="0e17c-378">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="0e17c-378">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="0e17c-379">Mobile Threat Defense パートナーがアカウントおよびデバイスで使用されている場合の、デバイスの脅威の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="0e17c-379">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="0e17c-380">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0e17c-380">Read Only.</span></span> <span data-ttu-id="0e17c-381">可能な値は、`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured` です。</span><span class="sxs-lookup"><span data-stu-id="0e17c-381">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="0e17c-382">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="0e17c-382">retireAfterDateTime</span></span>|<span data-ttu-id="0e17c-383">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e17c-383">DateTimeOffset</span></span>|<span data-ttu-id="0e17c-384">スケジュールされたアクションのためにデバイスが自動廃棄されるまでの時間を示します。</span><span class="sxs-lookup"><span data-stu-id="0e17c-384">Indicates the time after when a device will be auto retired because of scheduled action.</span></span>|
|<span data-ttu-id="0e17c-385">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="0e17c-385">usersLoggedOn</span></span>|<span data-ttu-id="0e17c-386">[loggedOnUser](../resources/intune-devices-loggedonuser.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0e17c-386">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="0e17c-387">デバイスの最後にログオンしたユーザーを示します</span><span class="sxs-lookup"><span data-stu-id="0e17c-387">Indicates the last logged on users of a device</span></span>|
|<span data-ttu-id="0e17c-388">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e17c-388">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="0e17c-389">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e17c-389">DateTimeOffset</span></span>|<span data-ttu-id="0e17c-390">PreferMdmOverGroupPolicy の設定が設定された DateTime を報告します。</span><span class="sxs-lookup"><span data-stu-id="0e17c-390">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="0e17c-391">設定すると、競合がある場合に Intune MDM 設定がグループポリシー設定を上書きします。</span><span class="sxs-lookup"><span data-stu-id="0e17c-391">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="0e17c-392">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0e17c-392">Read Only.</span></span>|
|<span data-ttu-id="0e17c-393">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="0e17c-393">autopilotEnrolled</span></span>|<span data-ttu-id="0e17c-394">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e17c-394">Boolean</span></span>|<span data-ttu-id="0e17c-395">管理対象デバイスが自動パイロットで登録されているかどうかを報告します。</span><span class="sxs-lookup"><span data-stu-id="0e17c-395">Reports if the managed device is enrolled via auto-pilot.</span></span>|
|<span data-ttu-id="0e17c-396">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="0e17c-396">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="0e17c-397">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e17c-397">Boolean</span></span>|<span data-ttu-id="0e17c-398">管理対象 iOS デバイスがユーザー承認登録であるかどうかを報告します。</span><span class="sxs-lookup"><span data-stu-id="0e17c-398">Reports if the managed iOS device is user approval enrollment.</span></span>|
|<span data-ttu-id="0e17c-399">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="0e17c-399">managementCertificateExpirationDate</span></span>|<span data-ttu-id="0e17c-400">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e17c-400">DateTimeOffset</span></span>|<span data-ttu-id="0e17c-401">デバイス管理証明書の有効期限を報告する</span><span class="sxs-lookup"><span data-stu-id="0e17c-401">Reports device management certificate expiration date</span></span>|
|<span data-ttu-id="0e17c-402">iccid</span><span class="sxs-lookup"><span data-stu-id="0e17c-402">iccid</span></span>|<span data-ttu-id="0e17c-403">String</span><span class="sxs-lookup"><span data-stu-id="0e17c-403">String</span></span>|<span data-ttu-id="0e17c-404">Ic カード識別子。 SIM カードの一意の識別番号です。</span><span class="sxs-lookup"><span data-stu-id="0e17c-404">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span>|
|<span data-ttu-id="0e17c-405">udid</span><span class="sxs-lookup"><span data-stu-id="0e17c-405">udid</span></span>|<span data-ttu-id="0e17c-406">String</span><span class="sxs-lookup"><span data-stu-id="0e17c-406">String</span></span>|<span data-ttu-id="0e17c-407">IOS および macOS デバイスの一意のデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="0e17c-407">Unique Device Identifier for iOS and macOS devices.</span></span>|
|<span data-ttu-id="0e17c-408">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0e17c-408">roleScopeTagIds</span></span>|<span data-ttu-id="0e17c-409">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="0e17c-409">String collection</span></span>|<span data-ttu-id="0e17c-410">このデバイスインスタンスの範囲タグ Id のリスト。</span><span class="sxs-lookup"><span data-stu-id="0e17c-410">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="0e17c-411">windowsActiveMalwareCount 再計算</span><span class="sxs-lookup"><span data-stu-id="0e17c-411">windowsActiveMalwareCount</span></span>|<span data-ttu-id="0e17c-412">Int32</span><span class="sxs-lookup"><span data-stu-id="0e17c-412">Int32</span></span>|<span data-ttu-id="0e17c-413">この windows デバイスのアクティブなマルウェアの数</span><span class="sxs-lookup"><span data-stu-id="0e17c-413">Count of active malware for this windows device</span></span>|
|<span data-ttu-id="0e17c-414">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="0e17c-414">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="0e17c-415">Int32</span><span class="sxs-lookup"><span data-stu-id="0e17c-415">Int32</span></span>|<span data-ttu-id="0e17c-416">この windows デバイスの修復済みマルウェアの数</span><span class="sxs-lookup"><span data-stu-id="0e17c-416">Count of remediated malware for this windows device</span></span>|
|<span data-ttu-id="0e17c-417">notes</span><span class="sxs-lookup"><span data-stu-id="0e17c-417">notes</span></span>|<span data-ttu-id="0e17c-418">String</span><span class="sxs-lookup"><span data-stu-id="0e17c-418">String</span></span>|<span data-ttu-id="0e17c-419">IT 管理者によって作成されたデバイスのメモ</span><span class="sxs-lookup"><span data-stu-id="0e17c-419">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="0e17c-420">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="0e17c-420">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="0e17c-421">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="0e17c-421">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="0e17c-422">構成マネージャークライアントの正常性状態。 MDM/ConfigMgr エージェントによって管理されるデバイスに対してのみ有効です。</span><span class="sxs-lookup"><span data-stu-id="0e17c-422">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e17c-423">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0e17c-423">Relationships</span></span>
|<span data-ttu-id="0e17c-424">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0e17c-424">Relationship</span></span>|<span data-ttu-id="0e17c-425">型</span><span class="sxs-lookup"><span data-stu-id="0e17c-425">Type</span></span>|<span data-ttu-id="0e17c-426">説明</span><span class="sxs-lookup"><span data-stu-id="0e17c-426">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e17c-427">detectedApps</span><span class="sxs-lookup"><span data-stu-id="0e17c-427">detectedApps</span></span>|<span data-ttu-id="0e17c-428">[detectedApp](../resources/intune-devices-detectedapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0e17c-428">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="0e17c-429">デバイスに現在インストールされているすべてのアプリケーション</span><span class="sxs-lookup"><span data-stu-id="0e17c-429">All applications currently installed on the device</span></span>|
|<span data-ttu-id="0e17c-430">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="0e17c-430">deviceCategory</span></span>|[<span data-ttu-id="0e17c-431">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="0e17c-431">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="0e17c-432">デバイス カテゴリ</span><span class="sxs-lookup"><span data-stu-id="0e17c-432">Device category</span></span>|
|<span data-ttu-id="0e17c-433">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="0e17c-433">windowsProtectionState</span></span>|[<span data-ttu-id="0e17c-434">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="0e17c-434">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="0e17c-435">デバイス保護の状態。</span><span class="sxs-lookup"><span data-stu-id="0e17c-435">The device protection status.</span></span>|
|<span data-ttu-id="0e17c-436">users</span><span class="sxs-lookup"><span data-stu-id="0e17c-436">users</span></span>|<span data-ttu-id="0e17c-437">[user](../resources/intune-shared-user.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0e17c-437">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="0e17c-438">管理対象デバイスに関連付けられているプライマリユーザー。</span><span class="sxs-lookup"><span data-stu-id="0e17c-438">The primary users associated with the managed device.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0e17c-439">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0e17c-439">JSON Representation</span></span>
<span data-ttu-id="0e17c-440">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0e17c-440">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "String (identifier)",
  "userId": "String",
  "deviceName": "String",
  "hardwareInformation": {
    "@odata.type": "microsoft.graph.hardwareInformation",
    "serialNumber": "String",
    "totalStorageSpace": 1024,
    "freeStorageSpace": 1024,
    "imei": "String",
    "meid": "String",
    "manufacturer": "String",
    "model": "String",
    "phoneNumber": "String",
    "subscriberCarrier": "String",
    "cellularTechnology": "String",
    "wifiMac": "String",
    "operatingSystemLanguage": "String",
    "isSupervised": true,
    "isEncrypted": true,
    "isSharedDevice": true,
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
        "userPrincipalName": "String",
        "dataToSync": true,
        "dataQuota": 1024,
        "dataUsed": 1024
      }
    ],
    "tpmSpecificationVersion": "String",
    "operatingSystemEdition": "String",
    "deviceFullQualifiedDomainName": "String",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "String",
    "deviceGuardVirtualizationBasedSecurityState": "String",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "String"
  },
  "ownerType": "String",
  "managedDeviceOwnerType": "String",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "String",
      "actionState": "String",
      "startDateTime": "String (timestamp)",
      "lastUpdatedDateTime": "String (timestamp)"
    }
  ],
  "managementState": "String",
  "enrolledDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "chassisType": "String",
  "operatingSystem": "String",
  "deviceType": "String",
  "complianceState": "String",
  "jailBroken": "String",
  "managementAgent": "String",
  "osVersion": "String",
  "easActivated": true,
  "easDeviceId": "String",
  "easActivationDateTime": "String (timestamp)",
  "aadRegistered": true,
  "azureADRegistered": true,
  "deviceEnrollmentType": "String",
  "lostModeState": "String",
  "activationLockBypassCode": "String",
  "emailAddress": "String",
  "azureActiveDirectoryDeviceId": "String",
  "azureADDeviceId": "String",
  "deviceRegistrationState": "String",
  "deviceCategoryDisplayName": "String",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "String (timestamp)",
  "exchangeAccessState": "String",
  "exchangeAccessStateReason": "String",
  "remoteAssistanceSessionUrl": "String",
  "remoteAssistanceSessionErrorDetails": "String",
  "isEncrypted": true,
  "userPrincipalName": "String",
  "model": "String",
  "manufacturer": "String",
  "imei": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "serialNumber": "String",
  "phoneNumber": "String",
  "androidSecurityPatchLevel": "String",
  "userDisplayName": "String",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true,
    "endpointProtection": true,
    "officeApps": true
  },
  "wiFiMacAddress": "String",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "String",
    "contentNamespaceUrl": "String",
    "deviceHealthAttestationStatus": "String",
    "contentVersion": "String",
    "issuedDateTime": "String (timestamp)",
    "attestationIdentityKey": "String",
    "resetCount": 1024,
    "restartCount": 1024,
    "dataExcutionPolicy": "String",
    "bitLockerStatus": "String",
    "bootManagerVersion": "String",
    "codeIntegrityCheckVersion": "String",
    "secureBoot": "String",
    "bootDebugging": "String",
    "operatingSystemKernelDebugging": "String",
    "codeIntegrity": "String",
    "testSigning": "String",
    "safeMode": "String",
    "windowsPE": "String",
    "earlyLaunchAntiMalwareDriverProtection": "String",
    "virtualSecureMode": "String",
    "pcrHashAlgorithm": "String",
    "bootAppSecurityVersion": "String",
    "bootManagerSecurityVersion": "String",
    "tpmVersion": "String",
    "pcr0": "String",
    "secureBootConfigurationPolicyFingerPrint": "String",
    "codeIntegrityPolicy": "String",
    "bootRevisionListInfo": "String",
    "operatingSystemRevListInfo": "String",
    "healthStatusMismatchInfo": "String",
    "healthAttestationSupportedStatus": "String"
  },
  "subscriberCarrier": "String",
  "meid": "String",
  "totalStorageSpaceInBytes": 1024,
  "freeStorageSpaceInBytes": 1024,
  "managedDeviceName": "String",
  "partnerReportedThreatState": "String",
  "retireAfterDateTime": "String (timestamp)",
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.graph.loggedOnUser",
      "userId": "String",
      "lastLogOnDateTime": "String (timestamp)"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "String (timestamp)",
  "autopilotEnrolled": true,
  "requireUserEnrollmentApproval": true,
  "managementCertificateExpirationDate": "String (timestamp)",
  "iccid": "String",
  "udid": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "windowsActiveMalwareCount": 1024,
  "windowsRemediatedMalwareCount": 1024,
  "notes": "String",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
    "state": "String",
    "errorCode": 1024,
    "lastSyncDateTime": "String (timestamp)"
  }
}
```





