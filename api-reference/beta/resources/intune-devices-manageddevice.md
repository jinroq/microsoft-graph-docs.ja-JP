---
title: managedDevice リソース タイプ
description: Intune 経由で管理または事前登録されるデバイス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 274c0000dbdae3b886241d628f4d03e944b61d5d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162511"
---
# <a name="manageddevice-resource-type"></a><span data-ttu-id="bc845-103">managedDevice リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="bc845-103">managedDevice resource type</span></span>

> <span data-ttu-id="bc845-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc845-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc845-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bc845-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc845-106">Intune 経由で管理または事前登録されるデバイス</span><span class="sxs-lookup"><span data-stu-id="bc845-106">Devices that are managed or pre-enrolled through Intune</span></span>

## <a name="methods"></a><span data-ttu-id="bc845-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="bc845-107">Methods</span></span>
|<span data-ttu-id="bc845-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="bc845-108">Method</span></span>|<span data-ttu-id="bc845-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bc845-109">Return Type</span></span>|<span data-ttu-id="bc845-110">説明</span><span class="sxs-lookup"><span data-stu-id="bc845-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bc845-111">Get managedDevice</span><span class="sxs-lookup"><span data-stu-id="bc845-111">Get managedDevice</span></span>](../api/intune-devices-manageddevice-get.md)|[<span data-ttu-id="bc845-112">managedDevice</span><span class="sxs-lookup"><span data-stu-id="bc845-112">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="bc845-113">[managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="bc845-113">Read properties and relationships of the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="bc845-114">Update managedDevice</span><span class="sxs-lookup"><span data-stu-id="bc845-114">Update managedDevice</span></span>](../api/intune-devices-manageddevice-update.md)|[<span data-ttu-id="bc845-115">managedDevice</span><span class="sxs-lookup"><span data-stu-id="bc845-115">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="bc845-116">[managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bc845-116">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="bc845-117">executeAction アクション</span><span class="sxs-lookup"><span data-stu-id="bc845-117">executeAction action</span></span>](../api/intune-devices-manageddevice-executeaction.md)|[<span data-ttu-id="bc845-118">bulkManagedDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="bc845-118">bulkManagedDeviceActionResult</span></span>](../resources/intune-devices-bulkmanageddeviceactionresult.md)|<span data-ttu-id="bc845-119">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="bc845-119">Not yet documented</span></span>|
|[<span data-ttu-id="bc845-120">enableLostMode アクション</span><span class="sxs-lookup"><span data-stu-id="bc845-120">enableLostMode action</span></span>](../api/intune-devices-manageddevice-enablelostmode.md)|<span data-ttu-id="bc845-121">なし</span><span class="sxs-lookup"><span data-stu-id="bc845-121">None</span></span>|<span data-ttu-id="bc845-122">削除モードを有効にする</span><span class="sxs-lookup"><span data-stu-id="bc845-122">Enable lost mode</span></span>|
|[<span data-ttu-id="bc845-123">playLostModeSound アクション</span><span class="sxs-lookup"><span data-stu-id="bc845-123">playLostModeSound action</span></span>](../api/intune-devices-manageddevice-playlostmodesound.md)|<span data-ttu-id="bc845-124">なし</span><span class="sxs-lookup"><span data-stu-id="bc845-124">None</span></span>|<span data-ttu-id="bc845-125">リモート ロック</span><span class="sxs-lookup"><span data-stu-id="bc845-125">Remote lock</span></span>|
|[<span data-ttu-id="bc845-126">setDeviceName アクション</span><span class="sxs-lookup"><span data-stu-id="bc845-126">setDeviceName action</span></span>](../api/intune-devices-manageddevice-setdevicename.md)|<span data-ttu-id="bc845-127">なし</span><span class="sxs-lookup"><span data-stu-id="bc845-127">None</span></span>|<span data-ttu-id="bc845-128">デバイスのデバイス名を設定します。</span><span class="sxs-lookup"><span data-stu-id="bc845-128">Set device name of the device.</span></span>|
|[<span data-ttu-id="bc845-129">retire action</span><span class="sxs-lookup"><span data-stu-id="bc845-129">retire action</span></span>](../api/intune-devices-manageddevice-retire.md)|<span data-ttu-id="bc845-130">なし</span><span class="sxs-lookup"><span data-stu-id="bc845-130">None</span></span>|<span data-ttu-id="bc845-131">デバイスを破棄します</span><span class="sxs-lookup"><span data-stu-id="bc845-131">Retire a device</span></span>|
|[<span data-ttu-id="bc845-132">wipe action</span><span class="sxs-lookup"><span data-stu-id="bc845-132">wipe action</span></span>](../api/intune-devices-manageddevice-wipe.md)|<span data-ttu-id="bc845-133">なし</span><span class="sxs-lookup"><span data-stu-id="bc845-133">None</span></span>|<span data-ttu-id="bc845-134">デバイスをワイプします</span><span class="sxs-lookup"><span data-stu-id="bc845-134">Wipe a device</span></span>|
|[<span data-ttu-id="bc845-135">resetPasscode action</span><span class="sxs-lookup"><span data-stu-id="bc845-135">resetPasscode action</span></span>](../api/intune-devices-manageddevice-resetpasscode.md)|<span data-ttu-id="bc845-136">なし</span><span class="sxs-lookup"><span data-stu-id="bc845-136">None</span></span>|<span data-ttu-id="bc845-137">パスコードをリセットします</span><span class="sxs-lookup"><span data-stu-id="bc845-137">Reset passcode</span></span>|
|[<span data-ttu-id="bc845-138">remoteLock action</span><span class="sxs-lookup"><span data-stu-id="bc845-138">remoteLock action</span></span>](../api/intune-devices-manageddevice-remotelock.md)|<span data-ttu-id="bc845-139">なし</span><span class="sxs-lookup"><span data-stu-id="bc845-139">None</span></span>|<span data-ttu-id="bc845-140">リモート ロック</span><span class="sxs-lookup"><span data-stu-id="bc845-140">Remote lock</span></span>|
|[<span data-ttu-id="bc845-141">requestRemoteAssistance action</span><span class="sxs-lookup"><span data-stu-id="bc845-141">requestRemoteAssistance action</span></span>](../api/intune-devices-manageddevice-requestremoteassistance.md)|<span data-ttu-id="bc845-142">なし</span><span class="sxs-lookup"><span data-stu-id="bc845-142">None</span></span>|<span data-ttu-id="bc845-143">リモート アシスタンスを要求します</span><span class="sxs-lookup"><span data-stu-id="bc845-143">Request remote assistance</span></span>|
|[<span data-ttu-id="bc845-144">disableLostMode action</span><span class="sxs-lookup"><span data-stu-id="bc845-144">disableLostMode action</span></span>](../api/intune-devices-manageddevice-disablelostmode.md)|<span data-ttu-id="bc845-145">なし</span><span class="sxs-lookup"><span data-stu-id="bc845-145">None</span></span>|<span data-ttu-id="bc845-146">紛失モードを無効化します</span><span class="sxs-lookup"><span data-stu-id="bc845-146">Disable lost mode</span></span>|
|[<span data-ttu-id="bc845-147">locateDevice action</span><span class="sxs-lookup"><span data-stu-id="bc845-147">locateDevice action</span></span>](../api/intune-devices-manageddevice-locatedevice.md)|<span data-ttu-id="bc845-148">なし</span><span class="sxs-lookup"><span data-stu-id="bc845-148">None</span></span>|<span data-ttu-id="bc845-149">デバイスを検索します</span><span class="sxs-lookup"><span data-stu-id="bc845-149">Locate a device</span></span>|
|[<span data-ttu-id="bc845-150">bypassActivationLock action</span><span class="sxs-lookup"><span data-stu-id="bc845-150">bypassActivationLock action</span></span>](../api/intune-devices-manageddevice-bypassactivationlock.md)|<span data-ttu-id="bc845-151">なし</span><span class="sxs-lookup"><span data-stu-id="bc845-151">None</span></span>|<span data-ttu-id="bc845-152">アクティベーション ロックをバイパスします</span><span class="sxs-lookup"><span data-stu-id="bc845-152">Bypass activation lock</span></span>|
|[<span data-ttu-id="bc845-153">rebootNow action</span><span class="sxs-lookup"><span data-stu-id="bc845-153">rebootNow action</span></span>](../api/intune-devices-manageddevice-rebootnow.md)|<span data-ttu-id="bc845-154">なし</span><span class="sxs-lookup"><span data-stu-id="bc845-154">None</span></span>|<span data-ttu-id="bc845-155">デバイスを再起動します</span><span class="sxs-lookup"><span data-stu-id="bc845-155">Reboot device</span></span>|
|[<span data-ttu-id="bc845-156">shutDown action</span><span class="sxs-lookup"><span data-stu-id="bc845-156">shutDown action</span></span>](../api/intune-devices-manageddevice-shutdown.md)|<span data-ttu-id="bc845-157">なし</span><span class="sxs-lookup"><span data-stu-id="bc845-157">None</span></span>|<span data-ttu-id="bc845-158">デバイスをシャットダウンします</span><span class="sxs-lookup"><span data-stu-id="bc845-158">Shut down device</span></span>|
|[<span data-ttu-id="bc845-159">recoverPasscode action</span><span class="sxs-lookup"><span data-stu-id="bc845-159">recoverPasscode action</span></span>](../api/intune-devices-manageddevice-recoverpasscode.md)|<span data-ttu-id="bc845-160">なし</span><span class="sxs-lookup"><span data-stu-id="bc845-160">None</span></span>|<span data-ttu-id="bc845-161">パスコードを回復します</span><span class="sxs-lookup"><span data-stu-id="bc845-161">Recover passcode</span></span>|
|[<span data-ttu-id="bc845-162">cleanWindowsDevice action</span><span class="sxs-lookup"><span data-stu-id="bc845-162">cleanWindowsDevice action</span></span>](../api/intune-devices-manageddevice-cleanwindowsdevice.md)|<span data-ttu-id="bc845-163">なし</span><span class="sxs-lookup"><span data-stu-id="bc845-163">None</span></span>|<span data-ttu-id="bc845-164">Windows デバイスをクリーンにします</span><span class="sxs-lookup"><span data-stu-id="bc845-164">Clean Windows device</span></span>|
|[<span data-ttu-id="bc845-165">logoutSharedAppleDeviceActiveUser action</span><span class="sxs-lookup"><span data-stu-id="bc845-165">logoutSharedAppleDeviceActiveUser action</span></span>](../api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser.md)|<span data-ttu-id="bc845-166">なし</span><span class="sxs-lookup"><span data-stu-id="bc845-166">None</span></span>|<span data-ttu-id="bc845-167">共有の Apple デバイスのアクティブなユーザーをログアウトします</span><span class="sxs-lookup"><span data-stu-id="bc845-167">Logout shared Apple device active user</span></span>|
|[<span data-ttu-id="bc845-168">deleteUserFromSharedAppleDevice action</span><span class="sxs-lookup"><span data-stu-id="bc845-168">deleteUserFromSharedAppleDevice action</span></span>](../api/intune-devices-manageddevice-deleteuserfromsharedappledevice.md)|<span data-ttu-id="bc845-169">なし</span><span class="sxs-lookup"><span data-stu-id="bc845-169">None</span></span>|<span data-ttu-id="bc845-170">共有の Apple デバイスからユーザーを削除します</span><span class="sxs-lookup"><span data-stu-id="bc845-170">Delete user from shared Apple device</span></span>|
|[<span data-ttu-id="bc845-171">syncDevice action</span><span class="sxs-lookup"><span data-stu-id="bc845-171">syncDevice action</span></span>](../api/intune-devices-manageddevice-syncdevice.md)|<span data-ttu-id="bc845-172">なし</span><span class="sxs-lookup"><span data-stu-id="bc845-172">None</span></span>|<span data-ttu-id="bc845-173">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="bc845-173">Not yet documented</span></span>|
|[<span data-ttu-id="bc845-174">windowsDefenderScan action</span><span class="sxs-lookup"><span data-stu-id="bc845-174">windowsDefenderScan action</span></span>](../api/intune-devices-manageddevice-windowsdefenderscan.md)|<span data-ttu-id="bc845-175">なし</span><span class="sxs-lookup"><span data-stu-id="bc845-175">None</span></span>|<span data-ttu-id="bc845-176">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="bc845-176">Not yet documented</span></span>|
|[<span data-ttu-id="bc845-177">windowsDefenderUpdateSignatures action</span><span class="sxs-lookup"><span data-stu-id="bc845-177">windowsDefenderUpdateSignatures action</span></span>](../api/intune-devices-manageddevice-windowsdefenderupdatesignatures.md)|<span data-ttu-id="bc845-178">なし</span><span class="sxs-lookup"><span data-stu-id="bc845-178">None</span></span>|<span data-ttu-id="bc845-179">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="bc845-179">Not yet documented</span></span>|
|[<span data-ttu-id="bc845-180">updateWindowsDeviceAccount action</span><span class="sxs-lookup"><span data-stu-id="bc845-180">updateWindowsDeviceAccount action</span></span>](../api/intune-devices-manageddevice-updatewindowsdeviceaccount.md)|<span data-ttu-id="bc845-181">なし</span><span class="sxs-lookup"><span data-stu-id="bc845-181">None</span></span>|<span data-ttu-id="bc845-182">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="bc845-182">Not yet documented</span></span>|
|[<span data-ttu-id="bc845-183">revokeAppleVppLicenses アクション</span><span class="sxs-lookup"><span data-stu-id="bc845-183">revokeAppleVppLicenses action</span></span>](../api/intune-devices-manageddevice-revokeapplevpplicenses.md)|<span data-ttu-id="bc845-184">なし</span><span class="sxs-lookup"><span data-stu-id="bc845-184">None</span></span>|<span data-ttu-id="bc845-185">デバイスのすべての Apple Vpp ライセンスを取り消す</span><span class="sxs-lookup"><span data-stu-id="bc845-185">Revoke all Apple Vpp licenses for a device</span></span>|

## <a name="properties"></a><span data-ttu-id="bc845-186">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc845-186">Properties</span></span>
|<span data-ttu-id="bc845-187">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc845-187">Property</span></span>|<span data-ttu-id="bc845-188">型</span><span class="sxs-lookup"><span data-stu-id="bc845-188">Type</span></span>|<span data-ttu-id="bc845-189">説明</span><span class="sxs-lookup"><span data-stu-id="bc845-189">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc845-190">id</span><span class="sxs-lookup"><span data-stu-id="bc845-190">id</span></span>|<span data-ttu-id="bc845-191">文字列</span><span class="sxs-lookup"><span data-stu-id="bc845-191">String</span></span>|<span data-ttu-id="bc845-192">デバイスの一意識別子</span><span class="sxs-lookup"><span data-stu-id="bc845-192">Unique Identifier for the device</span></span>|
|<span data-ttu-id="bc845-193">userId</span><span class="sxs-lookup"><span data-stu-id="bc845-193">userId</span></span>|<span data-ttu-id="bc845-194">String</span><span class="sxs-lookup"><span data-stu-id="bc845-194">String</span></span>|<span data-ttu-id="bc845-195">デバイスに関連付けられているユーザーの一意の識別子</span><span class="sxs-lookup"><span data-stu-id="bc845-195">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="bc845-196">deviceName</span><span class="sxs-lookup"><span data-stu-id="bc845-196">deviceName</span></span>|<span data-ttu-id="bc845-197">String</span><span class="sxs-lookup"><span data-stu-id="bc845-197">String</span></span>|<span data-ttu-id="bc845-198">デバイスの名前</span><span class="sxs-lookup"><span data-stu-id="bc845-198">Name of the device</span></span>|
|<span data-ttu-id="bc845-199">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="bc845-199">hardwareInformation</span></span>|[<span data-ttu-id="bc845-200">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="bc845-200">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="bc845-201">デバイスのハードワードの詳細。</span><span class="sxs-lookup"><span data-stu-id="bc845-201">The hardward details for the device.</span></span>  <span data-ttu-id="bc845-202">記憶領域、製造元、シリアル番号などの情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="bc845-202">Includes information such as storage space, manufacturer, serial number, etc.</span></span>|
|<span data-ttu-id="bc845-203">ownerType</span><span class="sxs-lookup"><span data-stu-id="bc845-203">ownerType</span></span>|[<span data-ttu-id="bc845-204">ownerType</span><span class="sxs-lookup"><span data-stu-id="bc845-204">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="bc845-205">デバイスの所有権。</span><span class="sxs-lookup"><span data-stu-id="bc845-205">Ownership of the device.</span></span> <span data-ttu-id="bc845-206">' company ' または ' personal ' にすることができます。</span><span class="sxs-lookup"><span data-stu-id="bc845-206">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="bc845-207">可能な値は `unknown`、`company`、`personal` です。</span><span class="sxs-lookup"><span data-stu-id="bc845-207">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="bc845-208">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="bc845-208">managedDeviceOwnerType</span></span>|[<span data-ttu-id="bc845-209">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="bc845-209">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="bc845-210">デバイスの所有権。</span><span class="sxs-lookup"><span data-stu-id="bc845-210">Ownership of the device.</span></span> <span data-ttu-id="bc845-211">' company ' または ' personal ' にすることができます。</span><span class="sxs-lookup"><span data-stu-id="bc845-211">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="bc845-212">可能な値は `unknown`、`company`、`personal` です。</span><span class="sxs-lookup"><span data-stu-id="bc845-212">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="bc845-213">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="bc845-213">deviceActionResults</span></span>|<span data-ttu-id="bc845-214">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bc845-214">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="bc845-215">ComplexType deviceActionResult オブジェクトのリスト。</span><span class="sxs-lookup"><span data-stu-id="bc845-215">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="bc845-216">managementstate</span><span class="sxs-lookup"><span data-stu-id="bc845-216">managementState</span></span>|[<span data-ttu-id="bc845-217">managementstate</span><span class="sxs-lookup"><span data-stu-id="bc845-217">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="bc845-218">デバイスの管理状態。</span><span class="sxs-lookup"><span data-stu-id="bc845-218">Management state of the device.</span></span> <span data-ttu-id="bc845-219">可能な値は、`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered` です。</span><span class="sxs-lookup"><span data-stu-id="bc845-219">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="bc845-220">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="bc845-220">enrolledDateTime</span></span>|<span data-ttu-id="bc845-221">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc845-221">DateTimeOffset</span></span>|<span data-ttu-id="bc845-222">デバイスの登録時刻。</span><span class="sxs-lookup"><span data-stu-id="bc845-222">Enrollment time of the device.</span></span>|
|<span data-ttu-id="bc845-223">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="bc845-223">lastSyncDateTime</span></span>|<span data-ttu-id="bc845-224">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc845-224">DateTimeOffset</span></span>|<span data-ttu-id="bc845-225">デバイスが Intune との正常な同期を最終的に完了した日時。</span><span class="sxs-lookup"><span data-stu-id="bc845-225">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="bc845-226">chassisType</span><span class="sxs-lookup"><span data-stu-id="bc845-226">chassisType</span></span>|[<span data-ttu-id="bc845-227">chassisType</span><span class="sxs-lookup"><span data-stu-id="bc845-227">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="bc845-228">デバイスのシャーシの種類。</span><span class="sxs-lookup"><span data-stu-id="bc845-228">Chassis type of the device.</span></span> <span data-ttu-id="bc845-229">可能な値は、`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown` です。</span><span class="sxs-lookup"><span data-stu-id="bc845-229">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="bc845-230">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="bc845-230">operatingSystem</span></span>|<span data-ttu-id="bc845-231">文字列</span><span class="sxs-lookup"><span data-stu-id="bc845-231">String</span></span>|<span data-ttu-id="bc845-232">デバイスのオペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="bc845-232">Operating system of the device.</span></span> <span data-ttu-id="bc845-233">Windows、iOS など。</span><span class="sxs-lookup"><span data-stu-id="bc845-233">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="bc845-234">deviceType</span><span class="sxs-lookup"><span data-stu-id="bc845-234">deviceType</span></span>|[<span data-ttu-id="bc845-235">deviceType</span><span class="sxs-lookup"><span data-stu-id="bc845-235">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="bc845-236">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="bc845-236">Platform of the device.</span></span> <span data-ttu-id="bc845-237">可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="bc845-237">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="bc845-238">complianceState</span><span class="sxs-lookup"><span data-stu-id="bc845-238">complianceState</span></span>|[<span data-ttu-id="bc845-239">complianceState</span><span class="sxs-lookup"><span data-stu-id="bc845-239">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="bc845-240">デバイスのコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="bc845-240">Compliance state of the device.</span></span> <span data-ttu-id="bc845-241">可能な値は、`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager` です。</span><span class="sxs-lookup"><span data-stu-id="bc845-241">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="bc845-242">jailBroken</span><span class="sxs-lookup"><span data-stu-id="bc845-242">jailBroken</span></span>|<span data-ttu-id="bc845-243">String</span><span class="sxs-lookup"><span data-stu-id="bc845-243">String</span></span>|<span data-ttu-id="bc845-244">デバイスが脱獄またはルート化されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bc845-244">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="bc845-245">managementAgent</span><span class="sxs-lookup"><span data-stu-id="bc845-245">managementAgent</span></span>|[<span data-ttu-id="bc845-246">managementagenttype</span><span class="sxs-lookup"><span data-stu-id="bc845-246">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="bc845-247">デバイスの管理チャネル。</span><span class="sxs-lookup"><span data-stu-id="bc845-247">Management channel of the device.</span></span> <span data-ttu-id="bc845-248">Intune、EAS など。可能な値は`eas`、 `mdm`、 `easMdm` `intuneClient` `easIntuneClient` `configurationManagerClient` `jamf` `googleCloudDevicePolicyController`、、、、、、、、、 `microsoft365ManagedMdm`、、です。 `configurationManagerClientMdm` `configurationManagerClientMdmEas` `unknown`</span><span class="sxs-lookup"><span data-stu-id="bc845-248">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="bc845-249">osVersion</span><span class="sxs-lookup"><span data-stu-id="bc845-249">osVersion</span></span>|<span data-ttu-id="bc845-250">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="bc845-250">String</span></span>|<span data-ttu-id="bc845-251">デバイスのオペレーティング システムのバージョン。</span><span class="sxs-lookup"><span data-stu-id="bc845-251">Operating system version of the device.</span></span>|
|<span data-ttu-id="bc845-252">easActivated</span><span class="sxs-lookup"><span data-stu-id="bc845-252">easActivated</span></span>|<span data-ttu-id="bc845-253">ブール値</span><span class="sxs-lookup"><span data-stu-id="bc845-253">Boolean</span></span>|<span data-ttu-id="bc845-254">Exchange ActiveSync がアクティブになっているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bc845-254">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="bc845-255">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="bc845-255">easDeviceId</span></span>|<span data-ttu-id="bc845-256">String</span><span class="sxs-lookup"><span data-stu-id="bc845-256">String</span></span>|<span data-ttu-id="bc845-257">デバイスの Exchange ActiveSync の ID。</span><span class="sxs-lookup"><span data-stu-id="bc845-257">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="bc845-258">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="bc845-258">easActivationDateTime</span></span>|<span data-ttu-id="bc845-259">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc845-259">DateTimeOffset</span></span>|<span data-ttu-id="bc845-260">デバイスの Exchange ActivationSync のアクティブ化の時刻。</span><span class="sxs-lookup"><span data-stu-id="bc845-260">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="bc845-261">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="bc845-261">aadRegistered</span></span>|<span data-ttu-id="bc845-262">ブール値</span><span class="sxs-lookup"><span data-stu-id="bc845-262">Boolean</span></span>|<span data-ttu-id="bc845-263">Azure Active Directory が登録されているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bc845-263">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="bc845-264">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="bc845-264">azureADRegistered</span></span>|<span data-ttu-id="bc845-265">ブール値</span><span class="sxs-lookup"><span data-stu-id="bc845-265">Boolean</span></span>|<span data-ttu-id="bc845-266">Azure Active Directory が登録されているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bc845-266">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="bc845-267">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="bc845-267">deviceEnrollmentType</span></span>|[<span data-ttu-id="bc845-268">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="bc845-268">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="bc845-269">デバイスの登録の種類。</span><span class="sxs-lookup"><span data-stu-id="bc845-269">Enrollment type of the device.</span></span> <span data-ttu-id="bc845-270">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="bc845-270">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="bc845-271">lostModeState</span><span class="sxs-lookup"><span data-stu-id="bc845-271">lostModeState</span></span>|[<span data-ttu-id="bc845-272">lostModeState</span><span class="sxs-lookup"><span data-stu-id="bc845-272">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="bc845-273">失われたモードが有効か無効かを示します。</span><span class="sxs-lookup"><span data-stu-id="bc845-273">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="bc845-274">使用可能な値は、`disabled`、`enabled` です。</span><span class="sxs-lookup"><span data-stu-id="bc845-274">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="bc845-275">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="bc845-275">activationLockBypassCode</span></span>|<span data-ttu-id="bc845-276">String</span><span class="sxs-lookup"><span data-stu-id="bc845-276">String</span></span>|<span data-ttu-id="bc845-277">デバイスのアクティベーション ロックをバイパスするためのコード。</span><span class="sxs-lookup"><span data-stu-id="bc845-277">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="bc845-278">emailAddress</span><span class="sxs-lookup"><span data-stu-id="bc845-278">emailAddress</span></span>|<span data-ttu-id="bc845-279">String</span><span class="sxs-lookup"><span data-stu-id="bc845-279">String</span></span>|<span data-ttu-id="bc845-280">デバイスに関連付けられているユーザーの電子メール</span><span class="sxs-lookup"><span data-stu-id="bc845-280">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="bc845-281">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="bc845-281">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="bc845-282">String</span><span class="sxs-lookup"><span data-stu-id="bc845-282">String</span></span>|<span data-ttu-id="bc845-283">Azure Active Directory デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="bc845-283">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="bc845-284">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bc845-284">Read only.</span></span>|
|<span data-ttu-id="bc845-285">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="bc845-285">azureADDeviceId</span></span>|<span data-ttu-id="bc845-286">String</span><span class="sxs-lookup"><span data-stu-id="bc845-286">String</span></span>|<span data-ttu-id="bc845-287">Azure Active Directory デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="bc845-287">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="bc845-288">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bc845-288">Read only.</span></span>|
|<span data-ttu-id="bc845-289">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="bc845-289">deviceRegistrationState</span></span>|[<span data-ttu-id="bc845-290">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="bc845-290">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="bc845-291">デバイスの登録状態。</span><span class="sxs-lookup"><span data-stu-id="bc845-291">Device registration state.</span></span> <span data-ttu-id="bc845-292">可能な値は、`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="bc845-292">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="bc845-293">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="bc845-293">deviceCategoryDisplayName</span></span>|<span data-ttu-id="bc845-294">String</span><span class="sxs-lookup"><span data-stu-id="bc845-294">String</span></span>|<span data-ttu-id="bc845-295">デバイス カテゴリの表示名</span><span class="sxs-lookup"><span data-stu-id="bc845-295">Device category display name</span></span>|
|<span data-ttu-id="bc845-296">isSupervised</span><span class="sxs-lookup"><span data-stu-id="bc845-296">isSupervised</span></span>|<span data-ttu-id="bc845-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc845-297">Boolean</span></span>|<span data-ttu-id="bc845-298">デバイスの管理状況</span><span class="sxs-lookup"><span data-stu-id="bc845-298">Device supervised status</span></span>|
|<span data-ttu-id="bc845-299">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="bc845-299">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="bc845-300">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc845-300">DateTimeOffset</span></span>|<span data-ttu-id="bc845-301">最後にデバイスが Exchange に接続した時刻。</span><span class="sxs-lookup"><span data-stu-id="bc845-301">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="bc845-302">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="bc845-302">exchangeAccessState</span></span>|[<span data-ttu-id="bc845-303">devicemanagementexchangeaccessstate</span><span class="sxs-lookup"><span data-stu-id="bc845-303">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="bc845-304">Exchange でのデバイスのアクセスの状態。</span><span class="sxs-lookup"><span data-stu-id="bc845-304">The Access State of the device in Exchange.</span></span> <span data-ttu-id="bc845-305">可能な値は、`none`、`unknown`、`allowed`、`blocked`、`quarantined` です。</span><span class="sxs-lookup"><span data-stu-id="bc845-305">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="bc845-306">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="bc845-306">exchangeAccessStateReason</span></span>|[<span data-ttu-id="bc845-307">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="bc845-307">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="bc845-308">Exchange でのデバイスのアクセス状態の理由。
</span><span class="sxs-lookup"><span data-stu-id="bc845-308">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="bc845-309">可能な値は、`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp` です。</span><span class="sxs-lookup"><span data-stu-id="bc845-309">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="bc845-310">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="bc845-310">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="bc845-311">String</span><span class="sxs-lookup"><span data-stu-id="bc845-311">String</span></span>|<span data-ttu-id="bc845-312">デバイスとのリモート アシスタンス セッションを確立できるようにする URL。</span><span class="sxs-lookup"><span data-stu-id="bc845-312">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="bc845-313">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="bc845-313">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="bc845-314">String</span><span class="sxs-lookup"><span data-stu-id="bc845-314">String</span></span>|<span data-ttu-id="bc845-315">リモート アシスタンス セッション オブジェクトの作成時に問題を識別するエラー文字列。</span><span class="sxs-lookup"><span data-stu-id="bc845-315">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="bc845-316">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="bc845-316">isEncrypted</span></span>|<span data-ttu-id="bc845-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc845-317">Boolean</span></span>|<span data-ttu-id="bc845-318">デバイスの暗号化の状態</span><span class="sxs-lookup"><span data-stu-id="bc845-318">Device encryption status</span></span>|
|<span data-ttu-id="bc845-319">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bc845-319">userPrincipalName</span></span>|<span data-ttu-id="bc845-320">文字列</span><span class="sxs-lookup"><span data-stu-id="bc845-320">String</span></span>|<span data-ttu-id="bc845-321">デバイスのユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="bc845-321">Device user principal name</span></span>|
|<span data-ttu-id="bc845-322">model</span><span class="sxs-lookup"><span data-stu-id="bc845-322">model</span></span>|<span data-ttu-id="bc845-323">String</span><span class="sxs-lookup"><span data-stu-id="bc845-323">String</span></span>|<span data-ttu-id="bc845-324">デバイスのモデル</span><span class="sxs-lookup"><span data-stu-id="bc845-324">Model of the device</span></span>|
|<span data-ttu-id="bc845-325">manufacturer</span><span class="sxs-lookup"><span data-stu-id="bc845-325">manufacturer</span></span>|<span data-ttu-id="bc845-326">String</span><span class="sxs-lookup"><span data-stu-id="bc845-326">String</span></span>|<span data-ttu-id="bc845-327">デバイスのメーカー</span><span class="sxs-lookup"><span data-stu-id="bc845-327">Manufacturer of the device</span></span>|
|<span data-ttu-id="bc845-328">imei</span><span class="sxs-lookup"><span data-stu-id="bc845-328">imei</span></span>|<span data-ttu-id="bc845-329">String</span><span class="sxs-lookup"><span data-stu-id="bc845-329">String</span></span>|<span data-ttu-id="bc845-330">IMEI</span><span class="sxs-lookup"><span data-stu-id="bc845-330">IMEI</span></span>|
|<span data-ttu-id="bc845-331">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bc845-331">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="bc845-332">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc845-332">DateTimeOffset</span></span>|<span data-ttu-id="bc845-333">デバイス コンプライアンスの猶予期間が経過する DateTime</span><span class="sxs-lookup"><span data-stu-id="bc845-333">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="bc845-334">serialNumber</span><span class="sxs-lookup"><span data-stu-id="bc845-334">serialNumber</span></span>|<span data-ttu-id="bc845-335">String</span><span class="sxs-lookup"><span data-stu-id="bc845-335">String</span></span>|<span data-ttu-id="bc845-336">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="bc845-336">SerialNumber</span></span>|
|<span data-ttu-id="bc845-337">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="bc845-337">phoneNumber</span></span>|<span data-ttu-id="bc845-338">String</span><span class="sxs-lookup"><span data-stu-id="bc845-338">String</span></span>|<span data-ttu-id="bc845-339">デバイスの電話番号</span><span class="sxs-lookup"><span data-stu-id="bc845-339">Phone number of the device</span></span>|
|<span data-ttu-id="bc845-340">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="bc845-340">androidSecurityPatchLevel</span></span>|<span data-ttu-id="bc845-341">String</span><span class="sxs-lookup"><span data-stu-id="bc845-341">String</span></span>|<span data-ttu-id="bc845-342">Android セキュリティ パッチのレベル</span><span class="sxs-lookup"><span data-stu-id="bc845-342">Android security patch level</span></span>|
|<span data-ttu-id="bc845-343">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="bc845-343">userDisplayName</span></span>|<span data-ttu-id="bc845-344">String</span><span class="sxs-lookup"><span data-stu-id="bc845-344">String</span></span>|<span data-ttu-id="bc845-345">ユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="bc845-345">User display name</span></span>|
|<span data-ttu-id="bc845-346">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="bc845-346">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="bc845-347">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="bc845-347">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="bc845-348">ConfigrMgr クライアント対応機能
</span><span class="sxs-lookup"><span data-stu-id="bc845-348">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="bc845-349">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="bc845-349">wiFiMacAddress</span></span>|<span data-ttu-id="bc845-350">String</span><span class="sxs-lookup"><span data-stu-id="bc845-350">String</span></span>|<span data-ttu-id="bc845-351">Wi-Fi MAC</span><span class="sxs-lookup"><span data-stu-id="bc845-351">Wi-Fi MAC</span></span>|
|<span data-ttu-id="bc845-352">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="bc845-352">deviceHealthAttestationState</span></span>|[<span data-ttu-id="bc845-353">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="bc845-353">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="bc845-354">デバイスの正常性構成証明の状態。</span><span class="sxs-lookup"><span data-stu-id="bc845-354">The device health attestation state.</span></span>|
|<span data-ttu-id="bc845-355">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="bc845-355">subscriberCarrier</span></span>|<span data-ttu-id="bc845-356">String</span><span class="sxs-lookup"><span data-stu-id="bc845-356">String</span></span>|<span data-ttu-id="bc845-357">サブスクライバー通信事業者</span><span class="sxs-lookup"><span data-stu-id="bc845-357">Subscriber Carrier</span></span>|
|<span data-ttu-id="bc845-358">meid</span><span class="sxs-lookup"><span data-stu-id="bc845-358">meid</span></span>|<span data-ttu-id="bc845-359">String</span><span class="sxs-lookup"><span data-stu-id="bc845-359">String</span></span>|<span data-ttu-id="bc845-360">MEID</span><span class="sxs-lookup"><span data-stu-id="bc845-360">MEID</span></span>|
|<span data-ttu-id="bc845-361">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="bc845-361">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="bc845-362">Int64</span><span class="sxs-lookup"><span data-stu-id="bc845-362">Int64</span></span>|<span data-ttu-id="bc845-363">記憶域の合計 (バイト)</span><span class="sxs-lookup"><span data-stu-id="bc845-363">Total Storage in Bytes</span></span>|
|<span data-ttu-id="bc845-364">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="bc845-364">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="bc845-365">Int64</span><span class="sxs-lookup"><span data-stu-id="bc845-365">Int64</span></span>|<span data-ttu-id="bc845-366">空き記憶域 (バイト)</span><span class="sxs-lookup"><span data-stu-id="bc845-366">Free Storage in Bytes</span></span>|
|<span data-ttu-id="bc845-367">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="bc845-367">managedDeviceName</span></span>|<span data-ttu-id="bc845-368">String</span><span class="sxs-lookup"><span data-stu-id="bc845-368">String</span></span>|<span data-ttu-id="bc845-369">デバイスを識別する名前が自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="bc845-369">Automatically generated name to identify a device.</span></span> <span data-ttu-id="bc845-370">ユーザー フレンドリ名に上書きできます。</span><span class="sxs-lookup"><span data-stu-id="bc845-370">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="bc845-371">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="bc845-371">partnerReportedThreatState</span></span>|[<span data-ttu-id="bc845-372">manageddevicepartnerreportedhealthstate</span><span class="sxs-lookup"><span data-stu-id="bc845-372">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="bc845-373">Mobile Threat Defense パートナーがアカウントおよびデバイスで使用されている場合の、デバイスの脅威の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="bc845-373">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="bc845-374">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bc845-374">Read Only.</span></span> <span data-ttu-id="bc845-375">可能な値は、`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured` です。</span><span class="sxs-lookup"><span data-stu-id="bc845-375">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="bc845-376">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="bc845-376">usersLoggedOn</span></span>|<span data-ttu-id="bc845-377">[loggedOnUser](../resources/intune-devices-loggedonuser.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bc845-377">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="bc845-378">デバイスの最後にログオンしたユーザーを示します</span><span class="sxs-lookup"><span data-stu-id="bc845-378">Indicates the last logged on users of a device</span></span>|
|<span data-ttu-id="bc845-379">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc845-379">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="bc845-380">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc845-380">DateTimeOffset</span></span>|<span data-ttu-id="bc845-381">preferMdmOverGroupPolicy の設定が設定された DateTime を報告します。</span><span class="sxs-lookup"><span data-stu-id="bc845-381">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="bc845-382">設定すると、競合がある場合に Intune MDM 設定がグループポリシー設定を上書きします。</span><span class="sxs-lookup"><span data-stu-id="bc845-382">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="bc845-383">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bc845-383">Read Only.</span></span>|
|<span data-ttu-id="bc845-384">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="bc845-384">autopilotEnrolled</span></span>|<span data-ttu-id="bc845-385">ブール値</span><span class="sxs-lookup"><span data-stu-id="bc845-385">Boolean</span></span>|<span data-ttu-id="bc845-386">管理対象デバイスが自動パイロットで登録されているかどうかを報告します。</span><span class="sxs-lookup"><span data-stu-id="bc845-386">Reports if the managed device is enrolled via auto-pilot.</span></span>|
|<span data-ttu-id="bc845-387">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="bc845-387">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="bc845-388">ブール値</span><span class="sxs-lookup"><span data-stu-id="bc845-388">Boolean</span></span>|<span data-ttu-id="bc845-389">管理対象 iOS デバイスがユーザー承認登録であるかどうかを報告します。</span><span class="sxs-lookup"><span data-stu-id="bc845-389">Reports if the managed iOS device is user approval enrollment.</span></span>|
|<span data-ttu-id="bc845-390">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="bc845-390">managementCertificateExpirationDate</span></span>|<span data-ttu-id="bc845-391">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc845-391">DateTimeOffset</span></span>|<span data-ttu-id="bc845-392">デバイス管理証明書の有効期限を報告する</span><span class="sxs-lookup"><span data-stu-id="bc845-392">Reports device management certificate expiration date</span></span>|
|<span data-ttu-id="bc845-393">iccid</span><span class="sxs-lookup"><span data-stu-id="bc845-393">iccid</span></span>|<span data-ttu-id="bc845-394">String</span><span class="sxs-lookup"><span data-stu-id="bc845-394">String</span></span>|<span data-ttu-id="bc845-395">ic カード識別子。 SIM カードの一意の識別番号です。</span><span class="sxs-lookup"><span data-stu-id="bc845-395">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span>|
|<span data-ttu-id="bc845-396">udid</span><span class="sxs-lookup"><span data-stu-id="bc845-396">udid</span></span>|<span data-ttu-id="bc845-397">String</span><span class="sxs-lookup"><span data-stu-id="bc845-397">String</span></span>|<span data-ttu-id="bc845-398">iOS および macOS デバイスの一意のデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="bc845-398">Unique Device Identifier for iOS and macOS devices.</span></span>|
|<span data-ttu-id="bc845-399">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bc845-399">roleScopeTagIds</span></span>|<span data-ttu-id="bc845-400">String collection</span><span class="sxs-lookup"><span data-stu-id="bc845-400">String collection</span></span>|<span data-ttu-id="bc845-401">このデバイスインスタンスの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="bc845-401">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="bc845-402">windowsactivemalwarecount 再計算</span><span class="sxs-lookup"><span data-stu-id="bc845-402">windowsActiveMalwareCount</span></span>|<span data-ttu-id="bc845-403">Int32</span><span class="sxs-lookup"><span data-stu-id="bc845-403">Int32</span></span>|<span data-ttu-id="bc845-404">この windows デバイスのアクティブなマルウェアの数</span><span class="sxs-lookup"><span data-stu-id="bc845-404">Count of active malware for this windows device</span></span>|
|<span data-ttu-id="bc845-405">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="bc845-405">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="bc845-406">Int32</span><span class="sxs-lookup"><span data-stu-id="bc845-406">Int32</span></span>|<span data-ttu-id="bc845-407">この windows デバイスの修復済みマルウェアの数</span><span class="sxs-lookup"><span data-stu-id="bc845-407">Count of remediated malware for this windows device</span></span>|
|<span data-ttu-id="bc845-408">notes</span><span class="sxs-lookup"><span data-stu-id="bc845-408">notes</span></span>|<span data-ttu-id="bc845-409">String</span><span class="sxs-lookup"><span data-stu-id="bc845-409">String</span></span>|<span data-ttu-id="bc845-410">IT 管理者によって作成されたデバイスのメモ</span><span class="sxs-lookup"><span data-stu-id="bc845-410">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="bc845-411">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="bc845-411">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="bc845-412">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="bc845-412">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="bc845-413">構成マネージャークライアントの正常性状態。 MDM/ConfigMgr エージェントによって管理されるデバイスに対してのみ有効です。</span><span class="sxs-lookup"><span data-stu-id="bc845-413">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc845-414">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bc845-414">Relationships</span></span>
|<span data-ttu-id="bc845-415">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bc845-415">Relationship</span></span>|<span data-ttu-id="bc845-416">型</span><span class="sxs-lookup"><span data-stu-id="bc845-416">Type</span></span>|<span data-ttu-id="bc845-417">説明</span><span class="sxs-lookup"><span data-stu-id="bc845-417">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc845-418">detectedApps</span><span class="sxs-lookup"><span data-stu-id="bc845-418">detectedApps</span></span>|<span data-ttu-id="bc845-419">[detectedApp](../resources/intune-devices-detectedapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bc845-419">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="bc845-420">デバイスに現在インストールされているすべてのアプリケーション</span><span class="sxs-lookup"><span data-stu-id="bc845-420">All applications currently installed on the device</span></span>|
|<span data-ttu-id="bc845-421">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="bc845-421">deviceCategory</span></span>|[<span data-ttu-id="bc845-422">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="bc845-422">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="bc845-423">デバイス カテゴリ</span><span class="sxs-lookup"><span data-stu-id="bc845-423">Device category</span></span>|
|<span data-ttu-id="bc845-424">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="bc845-424">windowsProtectionState</span></span>|[<span data-ttu-id="bc845-425">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="bc845-425">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="bc845-426">デバイス保護の状態。</span><span class="sxs-lookup"><span data-stu-id="bc845-426">The device protection status.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bc845-427">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bc845-427">JSON Representation</span></span>
<span data-ttu-id="bc845-428">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bc845-428">Here is a JSON representation of the resource.</span></span>
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




