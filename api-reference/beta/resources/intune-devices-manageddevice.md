---
title: managedDevice リソース タイプ
description: Intune 経由で管理または事前登録されるデバイス
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d0656bcf3f2726ee114e5e302a4e60f322d8e96
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941983"
---
# <a name="manageddevice-resource-type"></a><span data-ttu-id="97d2b-103">managedDevice リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="97d2b-103">managedDevice resource type</span></span>

> <span data-ttu-id="97d2b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="97d2b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97d2b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="97d2b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97d2b-106">Intune 経由で管理または事前登録されるデバイス</span><span class="sxs-lookup"><span data-stu-id="97d2b-106">Devices that are managed or pre-enrolled through Intune</span></span>

## <a name="methods"></a><span data-ttu-id="97d2b-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="97d2b-107">Methods</span></span>
|<span data-ttu-id="97d2b-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="97d2b-108">Method</span></span>|<span data-ttu-id="97d2b-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="97d2b-109">Return Type</span></span>|<span data-ttu-id="97d2b-110">説明</span><span class="sxs-lookup"><span data-stu-id="97d2b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="97d2b-111">Get managedDevice</span><span class="sxs-lookup"><span data-stu-id="97d2b-111">Get managedDevice</span></span>](../api/intune-devices-manageddevice-get.md)|[<span data-ttu-id="97d2b-112">managedDevice</span><span class="sxs-lookup"><span data-stu-id="97d2b-112">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="97d2b-113">[managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="97d2b-113">Read properties and relationships of the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="97d2b-114">Update managedDevice</span><span class="sxs-lookup"><span data-stu-id="97d2b-114">Update managedDevice</span></span>](../api/intune-devices-manageddevice-update.md)|[<span data-ttu-id="97d2b-115">managedDevice</span><span class="sxs-lookup"><span data-stu-id="97d2b-115">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="97d2b-116">[managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="97d2b-116">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="97d2b-117">executeAction アクション</span><span class="sxs-lookup"><span data-stu-id="97d2b-117">executeAction action</span></span>](../api/intune-devices-manageddevice-executeaction.md)|[<span data-ttu-id="97d2b-118">bulkManagedDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="97d2b-118">bulkManagedDeviceActionResult</span></span>](../resources/intune-devices-bulkmanageddeviceactionresult.md)|<span data-ttu-id="97d2b-119">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="97d2b-119">Not yet documented</span></span>|
|[<span data-ttu-id="97d2b-120">enableLostMode アクション</span><span class="sxs-lookup"><span data-stu-id="97d2b-120">enableLostMode action</span></span>](../api/intune-devices-manageddevice-enablelostmode.md)|<span data-ttu-id="97d2b-121">None</span><span class="sxs-lookup"><span data-stu-id="97d2b-121">None</span></span>|<span data-ttu-id="97d2b-122">削除モードを有効にする</span><span class="sxs-lookup"><span data-stu-id="97d2b-122">Enable lost mode</span></span>|
|[<span data-ttu-id="97d2b-123">playLostModeSound アクション</span><span class="sxs-lookup"><span data-stu-id="97d2b-123">playLostModeSound action</span></span>](../api/intune-devices-manageddevice-playlostmodesound.md)|<span data-ttu-id="97d2b-124">None</span><span class="sxs-lookup"><span data-stu-id="97d2b-124">None</span></span>|<span data-ttu-id="97d2b-125">リモート ロック</span><span class="sxs-lookup"><span data-stu-id="97d2b-125">Remote lock</span></span>|
|[<span data-ttu-id="97d2b-126">setDeviceName アクション</span><span class="sxs-lookup"><span data-stu-id="97d2b-126">setDeviceName action</span></span>](../api/intune-devices-manageddevice-setdevicename.md)|<span data-ttu-id="97d2b-127">None</span><span class="sxs-lookup"><span data-stu-id="97d2b-127">None</span></span>|<span data-ttu-id="97d2b-128">デバイスのデバイス名を設定します。</span><span class="sxs-lookup"><span data-stu-id="97d2b-128">Set device name of the device.</span></span>|
|[<span data-ttu-id="97d2b-129">rotateFileVaultKey アクション</span><span class="sxs-lookup"><span data-stu-id="97d2b-129">rotateFileVaultKey action</span></span>](../api/intune-devices-manageddevice-rotatefilevaultkey.md)|<span data-ttu-id="97d2b-130">None</span><span class="sxs-lookup"><span data-stu-id="97d2b-130">None</span></span>|<span data-ttu-id="97d2b-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="97d2b-131">Not yet documented</span></span>|
|[<span data-ttu-id="97d2b-132">getFileVaultKey 関数</span><span class="sxs-lookup"><span data-stu-id="97d2b-132">getFileVaultKey function</span></span>](../api/intune-devices-manageddevice-getfilevaultkey.md)|<span data-ttu-id="97d2b-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="97d2b-133">String</span></span>|<span data-ttu-id="97d2b-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="97d2b-134">Not yet documented</span></span>|
|[<span data-ttu-id="97d2b-135">retire action</span><span class="sxs-lookup"><span data-stu-id="97d2b-135">retire action</span></span>](../api/intune-devices-manageddevice-retire.md)|<span data-ttu-id="97d2b-136">None</span><span class="sxs-lookup"><span data-stu-id="97d2b-136">None</span></span>|<span data-ttu-id="97d2b-137">デバイスを破棄します</span><span class="sxs-lookup"><span data-stu-id="97d2b-137">Retire a device</span></span>|
|[<span data-ttu-id="97d2b-138">wipe action</span><span class="sxs-lookup"><span data-stu-id="97d2b-138">wipe action</span></span>](../api/intune-devices-manageddevice-wipe.md)|<span data-ttu-id="97d2b-139">None</span><span class="sxs-lookup"><span data-stu-id="97d2b-139">None</span></span>|<span data-ttu-id="97d2b-140">デバイスをワイプします</span><span class="sxs-lookup"><span data-stu-id="97d2b-140">Wipe a device</span></span>|
|[<span data-ttu-id="97d2b-141">resetPasscode action</span><span class="sxs-lookup"><span data-stu-id="97d2b-141">resetPasscode action</span></span>](../api/intune-devices-manageddevice-resetpasscode.md)|<span data-ttu-id="97d2b-142">None</span><span class="sxs-lookup"><span data-stu-id="97d2b-142">None</span></span>|<span data-ttu-id="97d2b-143">パスコードをリセットします</span><span class="sxs-lookup"><span data-stu-id="97d2b-143">Reset passcode</span></span>|
|[<span data-ttu-id="97d2b-144">remoteLock action</span><span class="sxs-lookup"><span data-stu-id="97d2b-144">remoteLock action</span></span>](../api/intune-devices-manageddevice-remotelock.md)|<span data-ttu-id="97d2b-145">None</span><span class="sxs-lookup"><span data-stu-id="97d2b-145">None</span></span>|<span data-ttu-id="97d2b-146">リモート ロック</span><span class="sxs-lookup"><span data-stu-id="97d2b-146">Remote lock</span></span>|
|[<span data-ttu-id="97d2b-147">requestRemoteAssistance action</span><span class="sxs-lookup"><span data-stu-id="97d2b-147">requestRemoteAssistance action</span></span>](../api/intune-devices-manageddevice-requestremoteassistance.md)|<span data-ttu-id="97d2b-148">None</span><span class="sxs-lookup"><span data-stu-id="97d2b-148">None</span></span>|<span data-ttu-id="97d2b-149">リモート アシスタンスを要求します</span><span class="sxs-lookup"><span data-stu-id="97d2b-149">Request remote assistance</span></span>|
|[<span data-ttu-id="97d2b-150">disableLostMode action</span><span class="sxs-lookup"><span data-stu-id="97d2b-150">disableLostMode action</span></span>](../api/intune-devices-manageddevice-disablelostmode.md)|<span data-ttu-id="97d2b-151">None</span><span class="sxs-lookup"><span data-stu-id="97d2b-151">None</span></span>|<span data-ttu-id="97d2b-152">紛失モードを無効化します</span><span class="sxs-lookup"><span data-stu-id="97d2b-152">Disable lost mode</span></span>|
|[<span data-ttu-id="97d2b-153">locateDevice action</span><span class="sxs-lookup"><span data-stu-id="97d2b-153">locateDevice action</span></span>](../api/intune-devices-manageddevice-locatedevice.md)|<span data-ttu-id="97d2b-154">None</span><span class="sxs-lookup"><span data-stu-id="97d2b-154">None</span></span>|<span data-ttu-id="97d2b-155">デバイスを検索します</span><span class="sxs-lookup"><span data-stu-id="97d2b-155">Locate a device</span></span>|
|[<span data-ttu-id="97d2b-156">bypassActivationLock action</span><span class="sxs-lookup"><span data-stu-id="97d2b-156">bypassActivationLock action</span></span>](../api/intune-devices-manageddevice-bypassactivationlock.md)|<span data-ttu-id="97d2b-157">None</span><span class="sxs-lookup"><span data-stu-id="97d2b-157">None</span></span>|<span data-ttu-id="97d2b-158">アクティベーション ロックをバイパスします</span><span class="sxs-lookup"><span data-stu-id="97d2b-158">Bypass activation lock</span></span>|
|[<span data-ttu-id="97d2b-159">rebootNow action</span><span class="sxs-lookup"><span data-stu-id="97d2b-159">rebootNow action</span></span>](../api/intune-devices-manageddevice-rebootnow.md)|<span data-ttu-id="97d2b-160">None</span><span class="sxs-lookup"><span data-stu-id="97d2b-160">None</span></span>|<span data-ttu-id="97d2b-161">デバイスを再起動します</span><span class="sxs-lookup"><span data-stu-id="97d2b-161">Reboot device</span></span>|
|[<span data-ttu-id="97d2b-162">shutDown action</span><span class="sxs-lookup"><span data-stu-id="97d2b-162">shutDown action</span></span>](../api/intune-devices-manageddevice-shutdown.md)|<span data-ttu-id="97d2b-163">None</span><span class="sxs-lookup"><span data-stu-id="97d2b-163">None</span></span>|<span data-ttu-id="97d2b-164">デバイスをシャットダウンします</span><span class="sxs-lookup"><span data-stu-id="97d2b-164">Shut down device</span></span>|
|[<span data-ttu-id="97d2b-165">recoverPasscode action</span><span class="sxs-lookup"><span data-stu-id="97d2b-165">recoverPasscode action</span></span>](../api/intune-devices-manageddevice-recoverpasscode.md)|<span data-ttu-id="97d2b-166">None</span><span class="sxs-lookup"><span data-stu-id="97d2b-166">None</span></span>|<span data-ttu-id="97d2b-167">パスコードを回復します</span><span class="sxs-lookup"><span data-stu-id="97d2b-167">Recover passcode</span></span>|
|[<span data-ttu-id="97d2b-168">cleanWindowsDevice action</span><span class="sxs-lookup"><span data-stu-id="97d2b-168">cleanWindowsDevice action</span></span>](../api/intune-devices-manageddevice-cleanwindowsdevice.md)|<span data-ttu-id="97d2b-169">None</span><span class="sxs-lookup"><span data-stu-id="97d2b-169">None</span></span>|<span data-ttu-id="97d2b-170">Windows デバイスをクリーンにします</span><span class="sxs-lookup"><span data-stu-id="97d2b-170">Clean Windows device</span></span>|
|[<span data-ttu-id="97d2b-171">logoutSharedAppleDeviceActiveUser action</span><span class="sxs-lookup"><span data-stu-id="97d2b-171">logoutSharedAppleDeviceActiveUser action</span></span>](../api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser.md)|<span data-ttu-id="97d2b-172">None</span><span class="sxs-lookup"><span data-stu-id="97d2b-172">None</span></span>|<span data-ttu-id="97d2b-173">共有の Apple デバイスのアクティブなユーザーをログアウトします</span><span class="sxs-lookup"><span data-stu-id="97d2b-173">Logout shared Apple device active user</span></span>|
|[<span data-ttu-id="97d2b-174">deleteUserFromSharedAppleDevice action</span><span class="sxs-lookup"><span data-stu-id="97d2b-174">deleteUserFromSharedAppleDevice action</span></span>](../api/intune-devices-manageddevice-deleteuserfromsharedappledevice.md)|<span data-ttu-id="97d2b-175">なし</span><span class="sxs-lookup"><span data-stu-id="97d2b-175">None</span></span>|<span data-ttu-id="97d2b-176">共有の Apple デバイスからユーザーを削除します</span><span class="sxs-lookup"><span data-stu-id="97d2b-176">Delete user from shared Apple device</span></span>|
|[<span data-ttu-id="97d2b-177">syncDevice action</span><span class="sxs-lookup"><span data-stu-id="97d2b-177">syncDevice action</span></span>](../api/intune-devices-manageddevice-syncdevice.md)|<span data-ttu-id="97d2b-178">None</span><span class="sxs-lookup"><span data-stu-id="97d2b-178">None</span></span>|<span data-ttu-id="97d2b-179">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="97d2b-179">Not yet documented</span></span>|
|[<span data-ttu-id="97d2b-180">windowsDefenderScan action</span><span class="sxs-lookup"><span data-stu-id="97d2b-180">windowsDefenderScan action</span></span>](../api/intune-devices-manageddevice-windowsdefenderscan.md)|<span data-ttu-id="97d2b-181">None</span><span class="sxs-lookup"><span data-stu-id="97d2b-181">None</span></span>|<span data-ttu-id="97d2b-182">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="97d2b-182">Not yet documented</span></span>|
|[<span data-ttu-id="97d2b-183">windowsDefenderUpdateSignatures action</span><span class="sxs-lookup"><span data-stu-id="97d2b-183">windowsDefenderUpdateSignatures action</span></span>](../api/intune-devices-manageddevice-windowsdefenderupdatesignatures.md)|<span data-ttu-id="97d2b-184">None</span><span class="sxs-lookup"><span data-stu-id="97d2b-184">None</span></span>|<span data-ttu-id="97d2b-185">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="97d2b-185">Not yet documented</span></span>|
|[<span data-ttu-id="97d2b-186">updateWindowsDeviceAccount action</span><span class="sxs-lookup"><span data-stu-id="97d2b-186">updateWindowsDeviceAccount action</span></span>](../api/intune-devices-manageddevice-updatewindowsdeviceaccount.md)|<span data-ttu-id="97d2b-187">なし</span><span class="sxs-lookup"><span data-stu-id="97d2b-187">None</span></span>|<span data-ttu-id="97d2b-188">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="97d2b-188">Not yet documented</span></span>|
|[<span data-ttu-id="97d2b-189">revokeAppleVppLicenses アクション</span><span class="sxs-lookup"><span data-stu-id="97d2b-189">revokeAppleVppLicenses action</span></span>](../api/intune-devices-manageddevice-revokeapplevpplicenses.md)|<span data-ttu-id="97d2b-190">None</span><span class="sxs-lookup"><span data-stu-id="97d2b-190">None</span></span>|<span data-ttu-id="97d2b-191">デバイスのすべての Apple Vpp ライセンスを取り消す</span><span class="sxs-lookup"><span data-stu-id="97d2b-191">Revoke all Apple Vpp licenses for a device</span></span>|

## <a name="properties"></a><span data-ttu-id="97d2b-192">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97d2b-192">Properties</span></span>
|<span data-ttu-id="97d2b-193">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97d2b-193">Property</span></span>|<span data-ttu-id="97d2b-194">型</span><span class="sxs-lookup"><span data-stu-id="97d2b-194">Type</span></span>|<span data-ttu-id="97d2b-195">説明</span><span class="sxs-lookup"><span data-stu-id="97d2b-195">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97d2b-196">id</span><span class="sxs-lookup"><span data-stu-id="97d2b-196">id</span></span>|<span data-ttu-id="97d2b-197">文字列</span><span class="sxs-lookup"><span data-stu-id="97d2b-197">String</span></span>|<span data-ttu-id="97d2b-198">デバイスの一意識別子</span><span class="sxs-lookup"><span data-stu-id="97d2b-198">Unique Identifier for the device</span></span>|
|<span data-ttu-id="97d2b-199">userId</span><span class="sxs-lookup"><span data-stu-id="97d2b-199">userId</span></span>|<span data-ttu-id="97d2b-200">String</span><span class="sxs-lookup"><span data-stu-id="97d2b-200">String</span></span>|<span data-ttu-id="97d2b-201">デバイスに関連付けられているユーザーの一意の識別子</span><span class="sxs-lookup"><span data-stu-id="97d2b-201">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="97d2b-202">deviceName</span><span class="sxs-lookup"><span data-stu-id="97d2b-202">deviceName</span></span>|<span data-ttu-id="97d2b-203">String</span><span class="sxs-lookup"><span data-stu-id="97d2b-203">String</span></span>|<span data-ttu-id="97d2b-204">デバイスの名前</span><span class="sxs-lookup"><span data-stu-id="97d2b-204">Name of the device</span></span>|
|<span data-ttu-id="97d2b-205">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="97d2b-205">hardwareInformation</span></span>|[<span data-ttu-id="97d2b-206">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="97d2b-206">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="97d2b-207">デバイスのハードワードの詳細。</span><span class="sxs-lookup"><span data-stu-id="97d2b-207">The hardward details for the device.</span></span>  <span data-ttu-id="97d2b-208">記憶領域、製造元、シリアル番号などの情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="97d2b-208">Includes information such as storage space, manufacturer, serial number, etc.</span></span>|
|<span data-ttu-id="97d2b-209">ownerType</span><span class="sxs-lookup"><span data-stu-id="97d2b-209">ownerType</span></span>|[<span data-ttu-id="97d2b-210">ownerType</span><span class="sxs-lookup"><span data-stu-id="97d2b-210">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="97d2b-211">デバイスの所有権。</span><span class="sxs-lookup"><span data-stu-id="97d2b-211">Ownership of the device.</span></span> <span data-ttu-id="97d2b-212">' Company ' または ' personal ' にすることができます。</span><span class="sxs-lookup"><span data-stu-id="97d2b-212">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="97d2b-213">可能な値は、`unknown`、`company`、`personal` です。</span><span class="sxs-lookup"><span data-stu-id="97d2b-213">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="97d2b-214">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="97d2b-214">managedDeviceOwnerType</span></span>|[<span data-ttu-id="97d2b-215">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="97d2b-215">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="97d2b-216">デバイスの所有権。</span><span class="sxs-lookup"><span data-stu-id="97d2b-216">Ownership of the device.</span></span> <span data-ttu-id="97d2b-217">' Company ' または ' personal ' にすることができます。</span><span class="sxs-lookup"><span data-stu-id="97d2b-217">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="97d2b-218">可能な値は、`unknown`、`company`、`personal` です。</span><span class="sxs-lookup"><span data-stu-id="97d2b-218">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="97d2b-219">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="97d2b-219">deviceActionResults</span></span>|<span data-ttu-id="97d2b-220">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="97d2b-220">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="97d2b-221">ComplexType deviceActionResult オブジェクトのリスト。</span><span class="sxs-lookup"><span data-stu-id="97d2b-221">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="97d2b-222">managementState</span><span class="sxs-lookup"><span data-stu-id="97d2b-222">managementState</span></span>|[<span data-ttu-id="97d2b-223">managementState</span><span class="sxs-lookup"><span data-stu-id="97d2b-223">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="97d2b-224">デバイスの管理状態。</span><span class="sxs-lookup"><span data-stu-id="97d2b-224">Management state of the device.</span></span> <span data-ttu-id="97d2b-225">可能な値は、`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered` です。</span><span class="sxs-lookup"><span data-stu-id="97d2b-225">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="97d2b-226">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="97d2b-226">enrolledDateTime</span></span>|<span data-ttu-id="97d2b-227">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97d2b-227">DateTimeOffset</span></span>|<span data-ttu-id="97d2b-228">デバイスの登録時刻。</span><span class="sxs-lookup"><span data-stu-id="97d2b-228">Enrollment time of the device.</span></span>|
|<span data-ttu-id="97d2b-229">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="97d2b-229">lastSyncDateTime</span></span>|<span data-ttu-id="97d2b-230">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97d2b-230">DateTimeOffset</span></span>|<span data-ttu-id="97d2b-231">デバイスが Intune との正常な同期を最終的に完了した日時。</span><span class="sxs-lookup"><span data-stu-id="97d2b-231">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="97d2b-232">chassisType</span><span class="sxs-lookup"><span data-stu-id="97d2b-232">chassisType</span></span>|[<span data-ttu-id="97d2b-233">chassisType</span><span class="sxs-lookup"><span data-stu-id="97d2b-233">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="97d2b-234">デバイスのシャーシの種類。</span><span class="sxs-lookup"><span data-stu-id="97d2b-234">Chassis type of the device.</span></span> <span data-ttu-id="97d2b-235">可能な値は、`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown` です。</span><span class="sxs-lookup"><span data-stu-id="97d2b-235">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="97d2b-236">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="97d2b-236">operatingSystem</span></span>|<span data-ttu-id="97d2b-237">文字列</span><span class="sxs-lookup"><span data-stu-id="97d2b-237">String</span></span>|<span data-ttu-id="97d2b-238">デバイスのオペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="97d2b-238">Operating system of the device.</span></span> <span data-ttu-id="97d2b-239">Windows、iOS など。</span><span class="sxs-lookup"><span data-stu-id="97d2b-239">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="97d2b-240">deviceType</span><span class="sxs-lookup"><span data-stu-id="97d2b-240">deviceType</span></span>|[<span data-ttu-id="97d2b-241">deviceType</span><span class="sxs-lookup"><span data-stu-id="97d2b-241">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="97d2b-242">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="97d2b-242">Platform of the device.</span></span> <span data-ttu-id="97d2b-243">可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="97d2b-243">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="97d2b-244">complianceState</span><span class="sxs-lookup"><span data-stu-id="97d2b-244">complianceState</span></span>|[<span data-ttu-id="97d2b-245">complianceState</span><span class="sxs-lookup"><span data-stu-id="97d2b-245">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="97d2b-246">デバイスのコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="97d2b-246">Compliance state of the device.</span></span> <span data-ttu-id="97d2b-247">可能な値は、`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager` です。</span><span class="sxs-lookup"><span data-stu-id="97d2b-247">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="97d2b-248">jailBroken</span><span class="sxs-lookup"><span data-stu-id="97d2b-248">jailBroken</span></span>|<span data-ttu-id="97d2b-249">String</span><span class="sxs-lookup"><span data-stu-id="97d2b-249">String</span></span>|<span data-ttu-id="97d2b-250">デバイスが脱獄またはルート化されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="97d2b-250">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="97d2b-251">managementAgent</span><span class="sxs-lookup"><span data-stu-id="97d2b-251">managementAgent</span></span>|[<span data-ttu-id="97d2b-252">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="97d2b-252">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="97d2b-253">デバイスの管理チャネル。</span><span class="sxs-lookup"><span data-stu-id="97d2b-253">Management channel of the device.</span></span> <span data-ttu-id="97d2b-254">Intune、EAS など。可能な値は`eas`、 `mdm`、 `easMdm` `intuneClient` `easIntuneClient` `configurationManagerClient` `jamf` `googleCloudDevicePolicyController`、、、、、、、、、 `microsoft365ManagedMdm`、、です。 `configurationManagerClientMdm` `configurationManagerClientMdmEas` `unknown`</span><span class="sxs-lookup"><span data-stu-id="97d2b-254">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="97d2b-255">osVersion</span><span class="sxs-lookup"><span data-stu-id="97d2b-255">osVersion</span></span>|<span data-ttu-id="97d2b-256">String</span><span class="sxs-lookup"><span data-stu-id="97d2b-256">String</span></span>|<span data-ttu-id="97d2b-257">デバイスのオペレーティング システムのバージョン。</span><span class="sxs-lookup"><span data-stu-id="97d2b-257">Operating system version of the device.</span></span>|
|<span data-ttu-id="97d2b-258">easActivated</span><span class="sxs-lookup"><span data-stu-id="97d2b-258">easActivated</span></span>|<span data-ttu-id="97d2b-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="97d2b-259">Boolean</span></span>|<span data-ttu-id="97d2b-260">Exchange ActiveSync がアクティブになっているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="97d2b-260">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="97d2b-261">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="97d2b-261">easDeviceId</span></span>|<span data-ttu-id="97d2b-262">String</span><span class="sxs-lookup"><span data-stu-id="97d2b-262">String</span></span>|<span data-ttu-id="97d2b-263">デバイスの Exchange ActiveSync の ID。</span><span class="sxs-lookup"><span data-stu-id="97d2b-263">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="97d2b-264">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="97d2b-264">easActivationDateTime</span></span>|<span data-ttu-id="97d2b-265">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97d2b-265">DateTimeOffset</span></span>|<span data-ttu-id="97d2b-266">デバイスの Exchange ActivationSync のアクティブ化の時刻。</span><span class="sxs-lookup"><span data-stu-id="97d2b-266">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="97d2b-267">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="97d2b-267">aadRegistered</span></span>|<span data-ttu-id="97d2b-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="97d2b-268">Boolean</span></span>|<span data-ttu-id="97d2b-269">Azure Active Directory が登録されているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="97d2b-269">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="97d2b-270">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="97d2b-270">azureADRegistered</span></span>|<span data-ttu-id="97d2b-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="97d2b-271">Boolean</span></span>|<span data-ttu-id="97d2b-272">Azure Active Directory が登録されているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="97d2b-272">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="97d2b-273">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="97d2b-273">deviceEnrollmentType</span></span>|[<span data-ttu-id="97d2b-274">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="97d2b-274">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="97d2b-275">デバイスの登録の種類。</span><span class="sxs-lookup"><span data-stu-id="97d2b-275">Enrollment type of the device.</span></span> <span data-ttu-id="97d2b-276">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="97d2b-276">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="97d2b-277">lostModeState</span><span class="sxs-lookup"><span data-stu-id="97d2b-277">lostModeState</span></span>|[<span data-ttu-id="97d2b-278">lostModeState</span><span class="sxs-lookup"><span data-stu-id="97d2b-278">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="97d2b-279">失われたモードが有効か無効かを示します。</span><span class="sxs-lookup"><span data-stu-id="97d2b-279">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="97d2b-280">可能な値は、`disabled`、`enabled` です。</span><span class="sxs-lookup"><span data-stu-id="97d2b-280">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="97d2b-281">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="97d2b-281">activationLockBypassCode</span></span>|<span data-ttu-id="97d2b-282">String</span><span class="sxs-lookup"><span data-stu-id="97d2b-282">String</span></span>|<span data-ttu-id="97d2b-283">デバイスのアクティベーション ロックをバイパスするためのコード。</span><span class="sxs-lookup"><span data-stu-id="97d2b-283">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="97d2b-284">emailAddress</span><span class="sxs-lookup"><span data-stu-id="97d2b-284">emailAddress</span></span>|<span data-ttu-id="97d2b-285">String</span><span class="sxs-lookup"><span data-stu-id="97d2b-285">String</span></span>|<span data-ttu-id="97d2b-286">デバイスに関連付けられているユーザーの電子メール</span><span class="sxs-lookup"><span data-stu-id="97d2b-286">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="97d2b-287">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="97d2b-287">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="97d2b-288">String</span><span class="sxs-lookup"><span data-stu-id="97d2b-288">String</span></span>|<span data-ttu-id="97d2b-289">Azure Active Directory デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="97d2b-289">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="97d2b-290">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="97d2b-290">Read only.</span></span>|
|<span data-ttu-id="97d2b-291">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="97d2b-291">azureADDeviceId</span></span>|<span data-ttu-id="97d2b-292">String</span><span class="sxs-lookup"><span data-stu-id="97d2b-292">String</span></span>|<span data-ttu-id="97d2b-293">Azure Active Directory デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="97d2b-293">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="97d2b-294">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="97d2b-294">Read only.</span></span>|
|<span data-ttu-id="97d2b-295">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="97d2b-295">deviceRegistrationState</span></span>|[<span data-ttu-id="97d2b-296">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="97d2b-296">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="97d2b-297">デバイスの登録状態。</span><span class="sxs-lookup"><span data-stu-id="97d2b-297">Device registration state.</span></span> <span data-ttu-id="97d2b-298">可能な値は、`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="97d2b-298">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="97d2b-299">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="97d2b-299">deviceCategoryDisplayName</span></span>|<span data-ttu-id="97d2b-300">String</span><span class="sxs-lookup"><span data-stu-id="97d2b-300">String</span></span>|<span data-ttu-id="97d2b-301">デバイス カテゴリの表示名</span><span class="sxs-lookup"><span data-stu-id="97d2b-301">Device category display name</span></span>|
|<span data-ttu-id="97d2b-302">isSupervised</span><span class="sxs-lookup"><span data-stu-id="97d2b-302">isSupervised</span></span>|<span data-ttu-id="97d2b-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="97d2b-303">Boolean</span></span>|<span data-ttu-id="97d2b-304">デバイスの管理状況</span><span class="sxs-lookup"><span data-stu-id="97d2b-304">Device supervised status</span></span>|
|<span data-ttu-id="97d2b-305">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="97d2b-305">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="97d2b-306">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97d2b-306">DateTimeOffset</span></span>|<span data-ttu-id="97d2b-307">最後にデバイスが Exchange に接続した時刻。</span><span class="sxs-lookup"><span data-stu-id="97d2b-307">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="97d2b-308">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="97d2b-308">exchangeAccessState</span></span>|[<span data-ttu-id="97d2b-309">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="97d2b-309">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="97d2b-310">Exchange でのデバイスのアクセスの状態。</span><span class="sxs-lookup"><span data-stu-id="97d2b-310">The Access State of the device in Exchange.</span></span> <span data-ttu-id="97d2b-311">可能な値は、`none`、`unknown`、`allowed`、`blocked`、`quarantined` です。</span><span class="sxs-lookup"><span data-stu-id="97d2b-311">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="97d2b-312">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="97d2b-312">exchangeAccessStateReason</span></span>|[<span data-ttu-id="97d2b-313">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="97d2b-313">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="97d2b-314">Exchange でのデバイスのアクセス状態の理由。
</span><span class="sxs-lookup"><span data-stu-id="97d2b-314">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="97d2b-315">可能な値は、`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp` です。</span><span class="sxs-lookup"><span data-stu-id="97d2b-315">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="97d2b-316">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="97d2b-316">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="97d2b-317">String</span><span class="sxs-lookup"><span data-stu-id="97d2b-317">String</span></span>|<span data-ttu-id="97d2b-318">デバイスとのリモート アシスタンス セッションを確立できるようにする URL。</span><span class="sxs-lookup"><span data-stu-id="97d2b-318">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="97d2b-319">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="97d2b-319">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="97d2b-320">String</span><span class="sxs-lookup"><span data-stu-id="97d2b-320">String</span></span>|<span data-ttu-id="97d2b-321">リモート アシスタンス セッション オブジェクトの作成時に問題を識別するエラー文字列。</span><span class="sxs-lookup"><span data-stu-id="97d2b-321">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="97d2b-322">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="97d2b-322">isEncrypted</span></span>|<span data-ttu-id="97d2b-323">Boolean</span><span class="sxs-lookup"><span data-stu-id="97d2b-323">Boolean</span></span>|<span data-ttu-id="97d2b-324">デバイスの暗号化の状態</span><span class="sxs-lookup"><span data-stu-id="97d2b-324">Device encryption status</span></span>|
|<span data-ttu-id="97d2b-325">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="97d2b-325">userPrincipalName</span></span>|<span data-ttu-id="97d2b-326">String</span><span class="sxs-lookup"><span data-stu-id="97d2b-326">String</span></span>|<span data-ttu-id="97d2b-327">デバイスのユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="97d2b-327">Device user principal name</span></span>|
|<span data-ttu-id="97d2b-328">model</span><span class="sxs-lookup"><span data-stu-id="97d2b-328">model</span></span>|<span data-ttu-id="97d2b-329">String</span><span class="sxs-lookup"><span data-stu-id="97d2b-329">String</span></span>|<span data-ttu-id="97d2b-330">デバイスのモデル</span><span class="sxs-lookup"><span data-stu-id="97d2b-330">Model of the device</span></span>|
|<span data-ttu-id="97d2b-331">manufacturer</span><span class="sxs-lookup"><span data-stu-id="97d2b-331">manufacturer</span></span>|<span data-ttu-id="97d2b-332">String</span><span class="sxs-lookup"><span data-stu-id="97d2b-332">String</span></span>|<span data-ttu-id="97d2b-333">デバイスのメーカー</span><span class="sxs-lookup"><span data-stu-id="97d2b-333">Manufacturer of the device</span></span>|
|<span data-ttu-id="97d2b-334">imei</span><span class="sxs-lookup"><span data-stu-id="97d2b-334">imei</span></span>|<span data-ttu-id="97d2b-335">String</span><span class="sxs-lookup"><span data-stu-id="97d2b-335">String</span></span>|<span data-ttu-id="97d2b-336">IMEI</span><span class="sxs-lookup"><span data-stu-id="97d2b-336">IMEI</span></span>|
|<span data-ttu-id="97d2b-337">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="97d2b-337">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="97d2b-338">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97d2b-338">DateTimeOffset</span></span>|<span data-ttu-id="97d2b-339">デバイス コンプライアンスの猶予期間が経過する DateTime</span><span class="sxs-lookup"><span data-stu-id="97d2b-339">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="97d2b-340">serialNumber</span><span class="sxs-lookup"><span data-stu-id="97d2b-340">serialNumber</span></span>|<span data-ttu-id="97d2b-341">String</span><span class="sxs-lookup"><span data-stu-id="97d2b-341">String</span></span>|<span data-ttu-id="97d2b-342">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="97d2b-342">SerialNumber</span></span>|
|<span data-ttu-id="97d2b-343">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="97d2b-343">phoneNumber</span></span>|<span data-ttu-id="97d2b-344">String</span><span class="sxs-lookup"><span data-stu-id="97d2b-344">String</span></span>|<span data-ttu-id="97d2b-345">デバイスの電話番号</span><span class="sxs-lookup"><span data-stu-id="97d2b-345">Phone number of the device</span></span>|
|<span data-ttu-id="97d2b-346">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="97d2b-346">androidSecurityPatchLevel</span></span>|<span data-ttu-id="97d2b-347">String</span><span class="sxs-lookup"><span data-stu-id="97d2b-347">String</span></span>|<span data-ttu-id="97d2b-348">Android セキュリティ パッチのレベル</span><span class="sxs-lookup"><span data-stu-id="97d2b-348">Android security patch level</span></span>|
|<span data-ttu-id="97d2b-349">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="97d2b-349">userDisplayName</span></span>|<span data-ttu-id="97d2b-350">String</span><span class="sxs-lookup"><span data-stu-id="97d2b-350">String</span></span>|<span data-ttu-id="97d2b-351">ユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="97d2b-351">User display name</span></span>|
|<span data-ttu-id="97d2b-352">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="97d2b-352">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="97d2b-353">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="97d2b-353">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="97d2b-354">ConfigrMgr クライアント対応機能
</span><span class="sxs-lookup"><span data-stu-id="97d2b-354">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="97d2b-355">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="97d2b-355">wiFiMacAddress</span></span>|<span data-ttu-id="97d2b-356">String</span><span class="sxs-lookup"><span data-stu-id="97d2b-356">String</span></span>|<span data-ttu-id="97d2b-357">Wi-Fi MAC</span><span class="sxs-lookup"><span data-stu-id="97d2b-357">Wi-Fi MAC</span></span>|
|<span data-ttu-id="97d2b-358">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="97d2b-358">deviceHealthAttestationState</span></span>|[<span data-ttu-id="97d2b-359">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="97d2b-359">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="97d2b-360">デバイスの正常性構成証明の状態。</span><span class="sxs-lookup"><span data-stu-id="97d2b-360">The device health attestation state.</span></span>|
|<span data-ttu-id="97d2b-361">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="97d2b-361">subscriberCarrier</span></span>|<span data-ttu-id="97d2b-362">String</span><span class="sxs-lookup"><span data-stu-id="97d2b-362">String</span></span>|<span data-ttu-id="97d2b-363">サブスクライバー通信事業者</span><span class="sxs-lookup"><span data-stu-id="97d2b-363">Subscriber Carrier</span></span>|
|<span data-ttu-id="97d2b-364">meid</span><span class="sxs-lookup"><span data-stu-id="97d2b-364">meid</span></span>|<span data-ttu-id="97d2b-365">String</span><span class="sxs-lookup"><span data-stu-id="97d2b-365">String</span></span>|<span data-ttu-id="97d2b-366">MEID</span><span class="sxs-lookup"><span data-stu-id="97d2b-366">MEID</span></span>|
|<span data-ttu-id="97d2b-367">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="97d2b-367">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="97d2b-368">Int64</span><span class="sxs-lookup"><span data-stu-id="97d2b-368">Int64</span></span>|<span data-ttu-id="97d2b-369">記憶域の合計 (バイト)</span><span class="sxs-lookup"><span data-stu-id="97d2b-369">Total Storage in Bytes</span></span>|
|<span data-ttu-id="97d2b-370">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="97d2b-370">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="97d2b-371">Int64</span><span class="sxs-lookup"><span data-stu-id="97d2b-371">Int64</span></span>|<span data-ttu-id="97d2b-372">空き記憶域 (バイト)</span><span class="sxs-lookup"><span data-stu-id="97d2b-372">Free Storage in Bytes</span></span>|
|<span data-ttu-id="97d2b-373">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="97d2b-373">managedDeviceName</span></span>|<span data-ttu-id="97d2b-374">String</span><span class="sxs-lookup"><span data-stu-id="97d2b-374">String</span></span>|<span data-ttu-id="97d2b-375">デバイスを識別する名前が自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="97d2b-375">Automatically generated name to identify a device.</span></span> <span data-ttu-id="97d2b-376">ユーザー フレンドリ名に上書きできます。</span><span class="sxs-lookup"><span data-stu-id="97d2b-376">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="97d2b-377">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="97d2b-377">partnerReportedThreatState</span></span>|[<span data-ttu-id="97d2b-378">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="97d2b-378">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="97d2b-379">Mobile Threat Defense パートナーがアカウントおよびデバイスで使用されている場合の、デバイスの脅威の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="97d2b-379">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="97d2b-380">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="97d2b-380">Read Only.</span></span> <span data-ttu-id="97d2b-381">可能な値は、`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured` です。</span><span class="sxs-lookup"><span data-stu-id="97d2b-381">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="97d2b-382">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="97d2b-382">retireAfterDateTime</span></span>|<span data-ttu-id="97d2b-383">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97d2b-383">DateTimeOffset</span></span>|<span data-ttu-id="97d2b-384">スケジュールされたアクションのためにデバイスが自動廃棄されるまでの時間を示します。</span><span class="sxs-lookup"><span data-stu-id="97d2b-384">Indicates the time after when a device will be auto retired because of scheduled action.</span></span>|
|<span data-ttu-id="97d2b-385">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="97d2b-385">usersLoggedOn</span></span>|<span data-ttu-id="97d2b-386">[loggedOnUser](../resources/intune-devices-loggedonuser.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="97d2b-386">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="97d2b-387">デバイスの最後にログオンしたユーザーを示します</span><span class="sxs-lookup"><span data-stu-id="97d2b-387">Indicates the last logged on users of a device</span></span>|
|<span data-ttu-id="97d2b-388">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="97d2b-388">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="97d2b-389">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97d2b-389">DateTimeOffset</span></span>|<span data-ttu-id="97d2b-390">PreferMdmOverGroupPolicy の設定が設定された DateTime を報告します。</span><span class="sxs-lookup"><span data-stu-id="97d2b-390">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="97d2b-391">設定すると、競合がある場合に Intune MDM 設定がグループポリシー設定を上書きします。</span><span class="sxs-lookup"><span data-stu-id="97d2b-391">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="97d2b-392">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="97d2b-392">Read Only.</span></span>|
|<span data-ttu-id="97d2b-393">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="97d2b-393">autopilotEnrolled</span></span>|<span data-ttu-id="97d2b-394">Boolean</span><span class="sxs-lookup"><span data-stu-id="97d2b-394">Boolean</span></span>|<span data-ttu-id="97d2b-395">管理対象デバイスが自動パイロットで登録されているかどうかを報告します。</span><span class="sxs-lookup"><span data-stu-id="97d2b-395">Reports if the managed device is enrolled via auto-pilot.</span></span>|
|<span data-ttu-id="97d2b-396">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="97d2b-396">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="97d2b-397">Boolean</span><span class="sxs-lookup"><span data-stu-id="97d2b-397">Boolean</span></span>|<span data-ttu-id="97d2b-398">管理対象 iOS デバイスがユーザー承認登録であるかどうかを報告します。</span><span class="sxs-lookup"><span data-stu-id="97d2b-398">Reports if the managed iOS device is user approval enrollment.</span></span>|
|<span data-ttu-id="97d2b-399">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="97d2b-399">managementCertificateExpirationDate</span></span>|<span data-ttu-id="97d2b-400">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97d2b-400">DateTimeOffset</span></span>|<span data-ttu-id="97d2b-401">デバイス管理証明書の有効期限を報告する</span><span class="sxs-lookup"><span data-stu-id="97d2b-401">Reports device management certificate expiration date</span></span>|
|<span data-ttu-id="97d2b-402">iccid</span><span class="sxs-lookup"><span data-stu-id="97d2b-402">iccid</span></span>|<span data-ttu-id="97d2b-403">String</span><span class="sxs-lookup"><span data-stu-id="97d2b-403">String</span></span>|<span data-ttu-id="97d2b-404">Ic カード識別子。 SIM カードの一意の識別番号です。</span><span class="sxs-lookup"><span data-stu-id="97d2b-404">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span>|
|<span data-ttu-id="97d2b-405">udid</span><span class="sxs-lookup"><span data-stu-id="97d2b-405">udid</span></span>|<span data-ttu-id="97d2b-406">String</span><span class="sxs-lookup"><span data-stu-id="97d2b-406">String</span></span>|<span data-ttu-id="97d2b-407">IOS および macOS デバイスの一意のデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="97d2b-407">Unique Device Identifier for iOS and macOS devices.</span></span>|
|<span data-ttu-id="97d2b-408">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="97d2b-408">roleScopeTagIds</span></span>|<span data-ttu-id="97d2b-409">String collection</span><span class="sxs-lookup"><span data-stu-id="97d2b-409">String collection</span></span>|<span data-ttu-id="97d2b-410">このデバイスインスタンスの範囲タグ Id のリスト。</span><span class="sxs-lookup"><span data-stu-id="97d2b-410">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="97d2b-411">windowsActiveMalwareCount 再計算</span><span class="sxs-lookup"><span data-stu-id="97d2b-411">windowsActiveMalwareCount</span></span>|<span data-ttu-id="97d2b-412">Int32</span><span class="sxs-lookup"><span data-stu-id="97d2b-412">Int32</span></span>|<span data-ttu-id="97d2b-413">この windows デバイスのアクティブなマルウェアの数</span><span class="sxs-lookup"><span data-stu-id="97d2b-413">Count of active malware for this windows device</span></span>|
|<span data-ttu-id="97d2b-414">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="97d2b-414">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="97d2b-415">Int32</span><span class="sxs-lookup"><span data-stu-id="97d2b-415">Int32</span></span>|<span data-ttu-id="97d2b-416">この windows デバイスの修復済みマルウェアの数</span><span class="sxs-lookup"><span data-stu-id="97d2b-416">Count of remediated malware for this windows device</span></span>|
|<span data-ttu-id="97d2b-417">notes</span><span class="sxs-lookup"><span data-stu-id="97d2b-417">notes</span></span>|<span data-ttu-id="97d2b-418">String</span><span class="sxs-lookup"><span data-stu-id="97d2b-418">String</span></span>|<span data-ttu-id="97d2b-419">IT 管理者によって作成されたデバイスのメモ</span><span class="sxs-lookup"><span data-stu-id="97d2b-419">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="97d2b-420">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="97d2b-420">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="97d2b-421">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="97d2b-421">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="97d2b-422">構成マネージャークライアントの正常性状態。 MDM/ConfigMgr エージェントによって管理されるデバイスに対してのみ有効です。</span><span class="sxs-lookup"><span data-stu-id="97d2b-422">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|

## <a name="relationships"></a><span data-ttu-id="97d2b-423">関係</span><span class="sxs-lookup"><span data-stu-id="97d2b-423">Relationships</span></span>
|<span data-ttu-id="97d2b-424">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="97d2b-424">Relationship</span></span>|<span data-ttu-id="97d2b-425">型</span><span class="sxs-lookup"><span data-stu-id="97d2b-425">Type</span></span>|<span data-ttu-id="97d2b-426">説明</span><span class="sxs-lookup"><span data-stu-id="97d2b-426">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97d2b-427">detectedApps</span><span class="sxs-lookup"><span data-stu-id="97d2b-427">detectedApps</span></span>|<span data-ttu-id="97d2b-428">[detectedApp](../resources/intune-devices-detectedapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="97d2b-428">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="97d2b-429">デバイスに現在インストールされているすべてのアプリケーション</span><span class="sxs-lookup"><span data-stu-id="97d2b-429">All applications currently installed on the device</span></span>|
|<span data-ttu-id="97d2b-430">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="97d2b-430">deviceCategory</span></span>|[<span data-ttu-id="97d2b-431">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="97d2b-431">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="97d2b-432">デバイス カテゴリ</span><span class="sxs-lookup"><span data-stu-id="97d2b-432">Device category</span></span>|
|<span data-ttu-id="97d2b-433">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="97d2b-433">windowsProtectionState</span></span>|[<span data-ttu-id="97d2b-434">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="97d2b-434">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="97d2b-435">デバイス保護の状態。</span><span class="sxs-lookup"><span data-stu-id="97d2b-435">The device protection status.</span></span>|
|<span data-ttu-id="97d2b-436">users</span><span class="sxs-lookup"><span data-stu-id="97d2b-436">users</span></span>|<span data-ttu-id="97d2b-437">[user](../resources/intune-shared-user.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="97d2b-437">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="97d2b-438">管理対象デバイスに関連付けられているプライマリユーザー。</span><span class="sxs-lookup"><span data-stu-id="97d2b-438">The primary users associated with the managed device.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="97d2b-439">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="97d2b-439">JSON Representation</span></span>
<span data-ttu-id="97d2b-440">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="97d2b-440">Here is a JSON representation of the resource.</span></span>
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




