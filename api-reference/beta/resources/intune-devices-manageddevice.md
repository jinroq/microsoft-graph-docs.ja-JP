---
title: managedDevice リソース タイプ
description: Intune 経由で管理または事前登録されるデバイス
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d08b0559065b3977978621004b290a87879cdc70
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869217"
---
# <a name="manageddevice-resource-type"></a><span data-ttu-id="f3bd2-103">managedDevice リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="f3bd2-103">managedDevice resource type</span></span>

> <span data-ttu-id="f3bd2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3bd2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f3bd2-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f3bd2-107">Intune 経由で管理または事前登録されるデバイス</span><span class="sxs-lookup"><span data-stu-id="f3bd2-107">Devices that are managed or pre-enrolled through Intune</span></span>
## <a name="methods"></a><span data-ttu-id="f3bd2-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="f3bd2-108">Methods</span></span>
|<span data-ttu-id="f3bd2-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="f3bd2-109">Method</span></span>|<span data-ttu-id="f3bd2-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f3bd2-110">Return Type</span></span>|<span data-ttu-id="f3bd2-111">説明</span><span class="sxs-lookup"><span data-stu-id="f3bd2-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f3bd2-112">Get managedDevice</span><span class="sxs-lookup"><span data-stu-id="f3bd2-112">Get managedDevice</span></span>](../api/intune-devices-manageddevice-get.md)|[<span data-ttu-id="f3bd2-113">managedDevice</span><span class="sxs-lookup"><span data-stu-id="f3bd2-113">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="f3bd2-114">[managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-114">Read properties and relationships of the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="f3bd2-115">Update managedDevice</span><span class="sxs-lookup"><span data-stu-id="f3bd2-115">Update managedDevice</span></span>](../api/intune-devices-manageddevice-update.md)|[<span data-ttu-id="f3bd2-116">managedDevice</span><span class="sxs-lookup"><span data-stu-id="f3bd2-116">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="f3bd2-117">[managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-117">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="f3bd2-118">executeAction アクション</span><span class="sxs-lookup"><span data-stu-id="f3bd2-118">executeAction action</span></span>](../api/intune-devices-manageddevice-executeaction.md)|[<span data-ttu-id="f3bd2-119">bulkManagedDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="f3bd2-119">bulkManagedDeviceActionResult</span></span>](../resources/intune-devices-bulkmanageddeviceactionresult.md)|<span data-ttu-id="f3bd2-120">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f3bd2-120">Not yet documented</span></span>|
|[<span data-ttu-id="f3bd2-121">enableLostMode アクション</span><span class="sxs-lookup"><span data-stu-id="f3bd2-121">enableLostMode action</span></span>](../api/intune-devices-manageddevice-enablelostmode.md)|<span data-ttu-id="f3bd2-122">なし</span><span class="sxs-lookup"><span data-stu-id="f3bd2-122">None</span></span>|<span data-ttu-id="f3bd2-123">失われるモードを有効にします。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-123">Enable lost mode</span></span>|
|[<span data-ttu-id="f3bd2-124">playLostModeSound アクション</span><span class="sxs-lookup"><span data-stu-id="f3bd2-124">playLostModeSound action</span></span>](../api/intune-devices-manageddevice-playlostmodesound.md)|<span data-ttu-id="f3bd2-125">なし</span><span class="sxs-lookup"><span data-stu-id="f3bd2-125">None</span></span>|<span data-ttu-id="f3bd2-126">リモート ロック</span><span class="sxs-lookup"><span data-stu-id="f3bd2-126">Remote lock</span></span>|
|[<span data-ttu-id="f3bd2-127">setDeviceName アクション</span><span class="sxs-lookup"><span data-stu-id="f3bd2-127">setDeviceName action</span></span>](../api/intune-devices-manageddevice-setdevicename.md)|<span data-ttu-id="f3bd2-128">なし</span><span class="sxs-lookup"><span data-stu-id="f3bd2-128">None</span></span>|<span data-ttu-id="f3bd2-129">デバイスのデバイス名を設定します。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-129">Set device name of the device.</span></span>|
|[<span data-ttu-id="f3bd2-130">retire action</span><span class="sxs-lookup"><span data-stu-id="f3bd2-130">retire action</span></span>](../api/intune-devices-manageddevice-retire.md)|<span data-ttu-id="f3bd2-131">なし</span><span class="sxs-lookup"><span data-stu-id="f3bd2-131">None</span></span>|<span data-ttu-id="f3bd2-132">デバイスを破棄します</span><span class="sxs-lookup"><span data-stu-id="f3bd2-132">Retire a device</span></span>|
|[<span data-ttu-id="f3bd2-133">wipe action</span><span class="sxs-lookup"><span data-stu-id="f3bd2-133">wipe action</span></span>](../api/intune-devices-manageddevice-wipe.md)|<span data-ttu-id="f3bd2-134">なし</span><span class="sxs-lookup"><span data-stu-id="f3bd2-134">None</span></span>|<span data-ttu-id="f3bd2-135">デバイスをワイプします</span><span class="sxs-lookup"><span data-stu-id="f3bd2-135">Wipe a device</span></span>|
|[<span data-ttu-id="f3bd2-136">resetPasscode action</span><span class="sxs-lookup"><span data-stu-id="f3bd2-136">resetPasscode action</span></span>](../api/intune-devices-manageddevice-resetpasscode.md)|<span data-ttu-id="f3bd2-137">なし</span><span class="sxs-lookup"><span data-stu-id="f3bd2-137">None</span></span>|<span data-ttu-id="f3bd2-138">パスコードをリセットします</span><span class="sxs-lookup"><span data-stu-id="f3bd2-138">Reset passcode</span></span>|
|[<span data-ttu-id="f3bd2-139">remoteLock action</span><span class="sxs-lookup"><span data-stu-id="f3bd2-139">remoteLock action</span></span>](../api/intune-devices-manageddevice-remotelock.md)|<span data-ttu-id="f3bd2-140">なし</span><span class="sxs-lookup"><span data-stu-id="f3bd2-140">None</span></span>|<span data-ttu-id="f3bd2-141">リモート ロック</span><span class="sxs-lookup"><span data-stu-id="f3bd2-141">Remote lock</span></span>|
|[<span data-ttu-id="f3bd2-142">requestRemoteAssistance action</span><span class="sxs-lookup"><span data-stu-id="f3bd2-142">requestRemoteAssistance action</span></span>](../api/intune-devices-manageddevice-requestremoteassistance.md)|<span data-ttu-id="f3bd2-143">なし</span><span class="sxs-lookup"><span data-stu-id="f3bd2-143">None</span></span>|<span data-ttu-id="f3bd2-144">リモート アシスタンスを要求します</span><span class="sxs-lookup"><span data-stu-id="f3bd2-144">Request remote assistance</span></span>|
|[<span data-ttu-id="f3bd2-145">disableLostMode action</span><span class="sxs-lookup"><span data-stu-id="f3bd2-145">disableLostMode action</span></span>](../api/intune-devices-manageddevice-disablelostmode.md)|<span data-ttu-id="f3bd2-146">なし</span><span class="sxs-lookup"><span data-stu-id="f3bd2-146">None</span></span>|<span data-ttu-id="f3bd2-147">紛失モードを無効化します</span><span class="sxs-lookup"><span data-stu-id="f3bd2-147">Disable lost mode</span></span>|
|[<span data-ttu-id="f3bd2-148">locateDevice action</span><span class="sxs-lookup"><span data-stu-id="f3bd2-148">locateDevice action</span></span>](../api/intune-devices-manageddevice-locatedevice.md)|<span data-ttu-id="f3bd2-149">なし</span><span class="sxs-lookup"><span data-stu-id="f3bd2-149">None</span></span>|<span data-ttu-id="f3bd2-150">デバイスを検索します</span><span class="sxs-lookup"><span data-stu-id="f3bd2-150">Locate a device</span></span>|
|[<span data-ttu-id="f3bd2-151">bypassActivationLock action</span><span class="sxs-lookup"><span data-stu-id="f3bd2-151">bypassActivationLock action</span></span>](../api/intune-devices-manageddevice-bypassactivationlock.md)|<span data-ttu-id="f3bd2-152">なし</span><span class="sxs-lookup"><span data-stu-id="f3bd2-152">None</span></span>|<span data-ttu-id="f3bd2-153">アクティベーション ロックをバイパスします</span><span class="sxs-lookup"><span data-stu-id="f3bd2-153">Bypass activation lock</span></span>|
|[<span data-ttu-id="f3bd2-154">rebootNow action</span><span class="sxs-lookup"><span data-stu-id="f3bd2-154">rebootNow action</span></span>](../api/intune-devices-manageddevice-rebootnow.md)|<span data-ttu-id="f3bd2-155">なし</span><span class="sxs-lookup"><span data-stu-id="f3bd2-155">None</span></span>|<span data-ttu-id="f3bd2-156">デバイスを再起動します</span><span class="sxs-lookup"><span data-stu-id="f3bd2-156">Reboot device</span></span>|
|[<span data-ttu-id="f3bd2-157">shutDown action</span><span class="sxs-lookup"><span data-stu-id="f3bd2-157">shutDown action</span></span>](../api/intune-devices-manageddevice-shutdown.md)|<span data-ttu-id="f3bd2-158">なし</span><span class="sxs-lookup"><span data-stu-id="f3bd2-158">None</span></span>|<span data-ttu-id="f3bd2-159">デバイスをシャットダウンします</span><span class="sxs-lookup"><span data-stu-id="f3bd2-159">Shut down device</span></span>|
|[<span data-ttu-id="f3bd2-160">recoverPasscode action</span><span class="sxs-lookup"><span data-stu-id="f3bd2-160">recoverPasscode action</span></span>](../api/intune-devices-manageddevice-recoverpasscode.md)|<span data-ttu-id="f3bd2-161">なし</span><span class="sxs-lookup"><span data-stu-id="f3bd2-161">None</span></span>|<span data-ttu-id="f3bd2-162">パスコードを回復します</span><span class="sxs-lookup"><span data-stu-id="f3bd2-162">Recover passcode</span></span>|
|[<span data-ttu-id="f3bd2-163">cleanWindowsDevice action</span><span class="sxs-lookup"><span data-stu-id="f3bd2-163">cleanWindowsDevice action</span></span>](../api/intune-devices-manageddevice-cleanwindowsdevice.md)|<span data-ttu-id="f3bd2-164">なし</span><span class="sxs-lookup"><span data-stu-id="f3bd2-164">None</span></span>|<span data-ttu-id="f3bd2-165">Windows デバイスをクリーンにします</span><span class="sxs-lookup"><span data-stu-id="f3bd2-165">Clean Windows device</span></span>|
|[<span data-ttu-id="f3bd2-166">logoutSharedAppleDeviceActiveUser action</span><span class="sxs-lookup"><span data-stu-id="f3bd2-166">logoutSharedAppleDeviceActiveUser action</span></span>](../api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser.md)|<span data-ttu-id="f3bd2-167">なし</span><span class="sxs-lookup"><span data-stu-id="f3bd2-167">None</span></span>|<span data-ttu-id="f3bd2-168">共有の Apple デバイスのアクティブなユーザーをログアウトします</span><span class="sxs-lookup"><span data-stu-id="f3bd2-168">Logout shared Apple device active user</span></span>|
|[<span data-ttu-id="f3bd2-169">deleteUserFromSharedAppleDevice action</span><span class="sxs-lookup"><span data-stu-id="f3bd2-169">deleteUserFromSharedAppleDevice action</span></span>](../api/intune-devices-manageddevice-deleteuserfromsharedappledevice.md)|<span data-ttu-id="f3bd2-170">なし</span><span class="sxs-lookup"><span data-stu-id="f3bd2-170">None</span></span>|<span data-ttu-id="f3bd2-171">共有の Apple デバイスからユーザーを削除します</span><span class="sxs-lookup"><span data-stu-id="f3bd2-171">Delete user from shared Apple device</span></span>|
|[<span data-ttu-id="f3bd2-172">syncDevice action</span><span class="sxs-lookup"><span data-stu-id="f3bd2-172">syncDevice action</span></span>](../api/intune-devices-manageddevice-syncdevice.md)|<span data-ttu-id="f3bd2-173">なし</span><span class="sxs-lookup"><span data-stu-id="f3bd2-173">None</span></span>|<span data-ttu-id="f3bd2-174">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f3bd2-174">Not yet documented</span></span>|
|[<span data-ttu-id="f3bd2-175">windowsDefenderScan action</span><span class="sxs-lookup"><span data-stu-id="f3bd2-175">windowsDefenderScan action</span></span>](../api/intune-devices-manageddevice-windowsdefenderscan.md)|<span data-ttu-id="f3bd2-176">なし</span><span class="sxs-lookup"><span data-stu-id="f3bd2-176">None</span></span>|<span data-ttu-id="f3bd2-177">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f3bd2-177">Not yet documented</span></span>|
|[<span data-ttu-id="f3bd2-178">windowsDefenderUpdateSignatures action</span><span class="sxs-lookup"><span data-stu-id="f3bd2-178">windowsDefenderUpdateSignatures action</span></span>](../api/intune-devices-manageddevice-windowsdefenderupdatesignatures.md)|<span data-ttu-id="f3bd2-179">なし</span><span class="sxs-lookup"><span data-stu-id="f3bd2-179">None</span></span>|<span data-ttu-id="f3bd2-180">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f3bd2-180">Not yet documented</span></span>|
|[<span data-ttu-id="f3bd2-181">updateWindowsDeviceAccount action</span><span class="sxs-lookup"><span data-stu-id="f3bd2-181">updateWindowsDeviceAccount action</span></span>](../api/intune-devices-manageddevice-updatewindowsdeviceaccount.md)|<span data-ttu-id="f3bd2-182">なし</span><span class="sxs-lookup"><span data-stu-id="f3bd2-182">None</span></span>|<span data-ttu-id="f3bd2-183">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f3bd2-183">Not yet documented</span></span>|
|[<span data-ttu-id="f3bd2-184">revokeAppleVppLicenses アクション</span><span class="sxs-lookup"><span data-stu-id="f3bd2-184">revokeAppleVppLicenses action</span></span>](../api/intune-devices-manageddevice-revokeapplevpplicenses.md)|<span data-ttu-id="f3bd2-185">なし</span><span class="sxs-lookup"><span data-stu-id="f3bd2-185">None</span></span>|<span data-ttu-id="f3bd2-186">デバイスのすべてのアップル Vpp ライセンスを失効させる</span><span class="sxs-lookup"><span data-stu-id="f3bd2-186">Revoke all Apple Vpp licenses for a device</span></span>|

## <a name="properties"></a><span data-ttu-id="f3bd2-187">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3bd2-187">Properties</span></span>
|<span data-ttu-id="f3bd2-188">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3bd2-188">Property</span></span>|<span data-ttu-id="f3bd2-189">種類</span><span class="sxs-lookup"><span data-stu-id="f3bd2-189">Type</span></span>|<span data-ttu-id="f3bd2-190">説明</span><span class="sxs-lookup"><span data-stu-id="f3bd2-190">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3bd2-191">ID</span><span class="sxs-lookup"><span data-stu-id="f3bd2-191">id</span></span>|<span data-ttu-id="f3bd2-192">String</span><span class="sxs-lookup"><span data-stu-id="f3bd2-192">String</span></span>|<span data-ttu-id="f3bd2-193">デバイスの一意識別子</span><span class="sxs-lookup"><span data-stu-id="f3bd2-193">Unique Identifier for the device</span></span>|
|<span data-ttu-id="f3bd2-194">userId</span><span class="sxs-lookup"><span data-stu-id="f3bd2-194">userId</span></span>|<span data-ttu-id="f3bd2-195">String</span><span class="sxs-lookup"><span data-stu-id="f3bd2-195">String</span></span>|<span data-ttu-id="f3bd2-196">デバイスに関連付けられているユーザーの一意の識別子</span><span class="sxs-lookup"><span data-stu-id="f3bd2-196">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="f3bd2-197">deviceName</span><span class="sxs-lookup"><span data-stu-id="f3bd2-197">deviceName</span></span>|<span data-ttu-id="f3bd2-198">String</span><span class="sxs-lookup"><span data-stu-id="f3bd2-198">String</span></span>|<span data-ttu-id="f3bd2-199">デバイスの名前</span><span class="sxs-lookup"><span data-stu-id="f3bd2-199">Name of the device</span></span>|
|<span data-ttu-id="f3bd2-200">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="f3bd2-200">hardwareInformation</span></span>|[<span data-ttu-id="f3bd2-201">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="f3bd2-201">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="f3bd2-202">デバイスのハードウェアの詳細。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-202">The hardward details for the device.</span></span>  <span data-ttu-id="f3bd2-203">記憶域の製造元、シリアル番号などの情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-203">Includes information such as storage space, manufacturer, serial number, etc.</span></span>|
|<span data-ttu-id="f3bd2-204">ownerType</span><span class="sxs-lookup"><span data-stu-id="f3bd2-204">ownerType</span></span>|[<span data-ttu-id="f3bd2-205">ownerType</span><span class="sxs-lookup"><span data-stu-id="f3bd2-205">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="f3bd2-206">デバイスの所有権。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-206">Ownership of the device.</span></span> <span data-ttu-id="f3bd2-207">'会社' または '個人' にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-207">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="f3bd2-208">可能な値は、`unknown`、`company`、`personal` です。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-208">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="f3bd2-209">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="f3bd2-209">managedDeviceOwnerType</span></span>|[<span data-ttu-id="f3bd2-210">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="f3bd2-210">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="f3bd2-211">デバイスの所有権。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-211">Ownership of the device.</span></span> <span data-ttu-id="f3bd2-212">'会社' または '個人' にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-212">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="f3bd2-213">可能な値は、`unknown`、`company`、`personal` です。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-213">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="f3bd2-214">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="f3bd2-214">deviceActionResults</span></span>|<span data-ttu-id="f3bd2-215">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f3bd2-215">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="f3bd2-216">ComplexType deviceActionResult オブジェクトのリスト。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-216">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="f3bd2-217">managementState</span><span class="sxs-lookup"><span data-stu-id="f3bd2-217">managementState</span></span>|[<span data-ttu-id="f3bd2-218">managementState</span><span class="sxs-lookup"><span data-stu-id="f3bd2-218">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="f3bd2-219">デバイスの状態を管理します。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-219">Management state of the device.</span></span> <span data-ttu-id="f3bd2-220">可能な値は、`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered` です。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-220">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="f3bd2-221">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="f3bd2-221">enrolledDateTime</span></span>|<span data-ttu-id="f3bd2-222">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3bd2-222">DateTimeOffset</span></span>|<span data-ttu-id="f3bd2-223">デバイスの登録時刻。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-223">Enrollment time of the device.</span></span>|
|<span data-ttu-id="f3bd2-224">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f3bd2-224">lastSyncDateTime</span></span>|<span data-ttu-id="f3bd2-225">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3bd2-225">DateTimeOffset</span></span>|<span data-ttu-id="f3bd2-226">デバイスが Intune との正常な同期を最終的に完了した日時。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-226">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="f3bd2-227">chassisType</span><span class="sxs-lookup"><span data-stu-id="f3bd2-227">chassisType</span></span>|[<span data-ttu-id="f3bd2-228">chassisType</span><span class="sxs-lookup"><span data-stu-id="f3bd2-228">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="f3bd2-229">デバイスのシャーシの種類です。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-229">Chassis type of the device.</span></span> <span data-ttu-id="f3bd2-230">可能な値は、`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown` です。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-230">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="f3bd2-231">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="f3bd2-231">operatingSystem</span></span>|<span data-ttu-id="f3bd2-232">String</span><span class="sxs-lookup"><span data-stu-id="f3bd2-232">String</span></span>|<span data-ttu-id="f3bd2-233">デバイスのオペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-233">Operating system of the device.</span></span> <span data-ttu-id="f3bd2-234">Windows、iOS など。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-234">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="f3bd2-235">deviceType</span><span class="sxs-lookup"><span data-stu-id="f3bd2-235">deviceType</span></span>|[<span data-ttu-id="f3bd2-236">deviceType</span><span class="sxs-lookup"><span data-stu-id="f3bd2-236">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="f3bd2-237">デバイスのプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-237">Platform of the device.</span></span> <span data-ttu-id="f3bd2-238">使用可能な値: `desktop`、 `windowsRT`、 `winMO6`、 `nokia`、 `windowsPhone`、 `mac`、 `winCE`、 `winEmbedded`、 `iPhone`、 `iPad`、 `iPod`、 `android`、 `iSocConsumer`、 `unix`、 `macMDM`、 `holoLens`、 `surfaceHub`、 `androidForWork`、 `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="f3bd2-238">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="f3bd2-239">complianceState</span><span class="sxs-lookup"><span data-stu-id="f3bd2-239">complianceState</span></span>|[<span data-ttu-id="f3bd2-240">complianceState</span><span class="sxs-lookup"><span data-stu-id="f3bd2-240">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="f3bd2-241">デバイスのコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-241">Compliance state of the device.</span></span> <span data-ttu-id="f3bd2-242">可能な値は、`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager` です。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-242">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="f3bd2-243">jailBroken</span><span class="sxs-lookup"><span data-stu-id="f3bd2-243">jailBroken</span></span>|<span data-ttu-id="f3bd2-244">String</span><span class="sxs-lookup"><span data-stu-id="f3bd2-244">String</span></span>|<span data-ttu-id="f3bd2-245">デバイスが脱獄またはルート化されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-245">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="f3bd2-246">managementAgent</span><span class="sxs-lookup"><span data-stu-id="f3bd2-246">managementAgent</span></span>|[<span data-ttu-id="f3bd2-247">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="f3bd2-247">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="f3bd2-248">デバイスの管理チャネル。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-248">Management channel of the device.</span></span> <span data-ttu-id="f3bd2-249">Intune、EA などです。使用可能な値: `eas`、 `mdm`、 `easMdm`、 `intuneClient`、 `easIntuneClient`、 `configurationManagerClient`、 `configurationManagerClientMdm`、 `configurationManagerClientMdmEas`、 `unknown`、 `jamf`、 `googleCloudDevicePolicyController`、 `microsoft365ManagedMdm`。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-249">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="f3bd2-250">osVersion</span><span class="sxs-lookup"><span data-stu-id="f3bd2-250">osVersion</span></span>|<span data-ttu-id="f3bd2-251">String</span><span class="sxs-lookup"><span data-stu-id="f3bd2-251">String</span></span>|<span data-ttu-id="f3bd2-252">デバイスのオペレーティング システムのバージョン。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-252">Operating system version of the device.</span></span>|
|<span data-ttu-id="f3bd2-253">easActivated</span><span class="sxs-lookup"><span data-stu-id="f3bd2-253">easActivated</span></span>|<span data-ttu-id="f3bd2-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3bd2-254">Boolean</span></span>|<span data-ttu-id="f3bd2-255">Exchange ActiveSync がアクティブになっているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-255">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="f3bd2-256">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="f3bd2-256">easDeviceId</span></span>|<span data-ttu-id="f3bd2-257">String</span><span class="sxs-lookup"><span data-stu-id="f3bd2-257">String</span></span>|<span data-ttu-id="f3bd2-258">デバイスの Exchange ActiveSync の ID。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-258">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="f3bd2-259">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="f3bd2-259">easActivationDateTime</span></span>|<span data-ttu-id="f3bd2-260">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3bd2-260">DateTimeOffset</span></span>|<span data-ttu-id="f3bd2-261">デバイスの Exchange ActivationSync のアクティブ化の時刻。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-261">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="f3bd2-262">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="f3bd2-262">aadRegistered</span></span>|<span data-ttu-id="f3bd2-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3bd2-263">Boolean</span></span>|<span data-ttu-id="f3bd2-264">Azure Active Directory が登録されているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-264">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="f3bd2-265">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="f3bd2-265">azureADRegistered</span></span>|<span data-ttu-id="f3bd2-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3bd2-266">Boolean</span></span>|<span data-ttu-id="f3bd2-267">Azure Active Directory が登録されているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-267">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="f3bd2-268">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="f3bd2-268">deviceEnrollmentType</span></span>|[<span data-ttu-id="f3bd2-269">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="f3bd2-269">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="f3bd2-270">デバイスの登録の種類。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-270">Enrollment type of the device.</span></span> <span data-ttu-id="f3bd2-271">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-271">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="f3bd2-272">lostModeState</span><span class="sxs-lookup"><span data-stu-id="f3bd2-272">lostModeState</span></span>|[<span data-ttu-id="f3bd2-273">lostModeState</span><span class="sxs-lookup"><span data-stu-id="f3bd2-273">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="f3bd2-274">失われたモードが有効か無効を示します。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-274">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="f3bd2-275">使用可能な値は、`disabled`、`enabled` です。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-275">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="f3bd2-276">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="f3bd2-276">activationLockBypassCode</span></span>|<span data-ttu-id="f3bd2-277">String</span><span class="sxs-lookup"><span data-stu-id="f3bd2-277">String</span></span>|<span data-ttu-id="f3bd2-278">デバイスのアクティベーション ロックをバイパスするためのコード。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-278">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="f3bd2-279">emailAddress</span><span class="sxs-lookup"><span data-stu-id="f3bd2-279">emailAddress</span></span>|<span data-ttu-id="f3bd2-280">String</span><span class="sxs-lookup"><span data-stu-id="f3bd2-280">String</span></span>|<span data-ttu-id="f3bd2-281">デバイスに関連付けられているユーザーの電子メール</span><span class="sxs-lookup"><span data-stu-id="f3bd2-281">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="f3bd2-282">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="f3bd2-282">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="f3bd2-283">String</span><span class="sxs-lookup"><span data-stu-id="f3bd2-283">String</span></span>|<span data-ttu-id="f3bd2-284">Azure Active Directory デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-284">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="f3bd2-285">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-285">Read only.</span></span>|
|<span data-ttu-id="f3bd2-286">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="f3bd2-286">azureADDeviceId</span></span>|<span data-ttu-id="f3bd2-287">String</span><span class="sxs-lookup"><span data-stu-id="f3bd2-287">String</span></span>|<span data-ttu-id="f3bd2-288">Azure Active Directory デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-288">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="f3bd2-289">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-289">Read only.</span></span>|
|<span data-ttu-id="f3bd2-290">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="f3bd2-290">deviceRegistrationState</span></span>|[<span data-ttu-id="f3bd2-291">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="f3bd2-291">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="f3bd2-292">デバイスの登録状態。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-292">Device registration state.</span></span> <span data-ttu-id="f3bd2-293">可能な値は、`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-293">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="f3bd2-294">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="f3bd2-294">deviceCategoryDisplayName</span></span>|<span data-ttu-id="f3bd2-295">String</span><span class="sxs-lookup"><span data-stu-id="f3bd2-295">String</span></span>|<span data-ttu-id="f3bd2-296">デバイス カテゴリの表示名</span><span class="sxs-lookup"><span data-stu-id="f3bd2-296">Device category display name</span></span>|
|<span data-ttu-id="f3bd2-297">isSupervised</span><span class="sxs-lookup"><span data-stu-id="f3bd2-297">isSupervised</span></span>|<span data-ttu-id="f3bd2-298">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3bd2-298">Boolean</span></span>|<span data-ttu-id="f3bd2-299">デバイスの管理状況</span><span class="sxs-lookup"><span data-stu-id="f3bd2-299">Device supervised status</span></span>|
|<span data-ttu-id="f3bd2-300">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f3bd2-300">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="f3bd2-301">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3bd2-301">DateTimeOffset</span></span>|<span data-ttu-id="f3bd2-302">最後にデバイスが Exchange に接続した時刻。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-302">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="f3bd2-303">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="f3bd2-303">exchangeAccessState</span></span>|[<span data-ttu-id="f3bd2-304">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="f3bd2-304">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="f3bd2-305">Exchange でのデバイスのアクセスの状態。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-305">The Access State of the device in Exchange.</span></span> <span data-ttu-id="f3bd2-306">可能な値は、`none`、`unknown`、`allowed`、`blocked`、`quarantined` です。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-306">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="f3bd2-307">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="f3bd2-307">exchangeAccessStateReason</span></span>|[<span data-ttu-id="f3bd2-308">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="f3bd2-308">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="f3bd2-309">Exchange でのデバイスのアクセス状態の理由。
</span><span class="sxs-lookup"><span data-stu-id="f3bd2-309">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="f3bd2-310">可能な値は、`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp` です。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-310">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="f3bd2-311">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="f3bd2-311">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="f3bd2-312">String</span><span class="sxs-lookup"><span data-stu-id="f3bd2-312">String</span></span>|<span data-ttu-id="f3bd2-313">デバイスとのリモート アシスタンス セッションを確立できるようにする URL。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-313">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="f3bd2-314">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="f3bd2-314">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="f3bd2-315">String</span><span class="sxs-lookup"><span data-stu-id="f3bd2-315">String</span></span>|<span data-ttu-id="f3bd2-316">リモート アシスタンス セッション オブジェクトの作成時に問題を識別するエラー文字列。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-316">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="f3bd2-317">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="f3bd2-317">isEncrypted</span></span>|<span data-ttu-id="f3bd2-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3bd2-318">Boolean</span></span>|<span data-ttu-id="f3bd2-319">デバイスの暗号化の状態</span><span class="sxs-lookup"><span data-stu-id="f3bd2-319">Device encryption status</span></span>|
|<span data-ttu-id="f3bd2-320">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f3bd2-320">userPrincipalName</span></span>|<span data-ttu-id="f3bd2-321">String</span><span class="sxs-lookup"><span data-stu-id="f3bd2-321">String</span></span>|<span data-ttu-id="f3bd2-322">デバイスのユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-322">Device user principal name</span></span>|
|<span data-ttu-id="f3bd2-323">model</span><span class="sxs-lookup"><span data-stu-id="f3bd2-323">model</span></span>|<span data-ttu-id="f3bd2-324">String</span><span class="sxs-lookup"><span data-stu-id="f3bd2-324">String</span></span>|<span data-ttu-id="f3bd2-325">デバイスのモデル</span><span class="sxs-lookup"><span data-stu-id="f3bd2-325">Model of the device</span></span>|
|<span data-ttu-id="f3bd2-326">manufacturer</span><span class="sxs-lookup"><span data-stu-id="f3bd2-326">manufacturer</span></span>|<span data-ttu-id="f3bd2-327">String</span><span class="sxs-lookup"><span data-stu-id="f3bd2-327">String</span></span>|<span data-ttu-id="f3bd2-328">デバイスのメーカー</span><span class="sxs-lookup"><span data-stu-id="f3bd2-328">Manufacturer of the device</span></span>|
|<span data-ttu-id="f3bd2-329">imei</span><span class="sxs-lookup"><span data-stu-id="f3bd2-329">imei</span></span>|<span data-ttu-id="f3bd2-330">String</span><span class="sxs-lookup"><span data-stu-id="f3bd2-330">String</span></span>|<span data-ttu-id="f3bd2-331">IMEI</span><span class="sxs-lookup"><span data-stu-id="f3bd2-331">IMEI</span></span>|
|<span data-ttu-id="f3bd2-332">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f3bd2-332">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="f3bd2-333">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3bd2-333">DateTimeOffset</span></span>|<span data-ttu-id="f3bd2-334">デバイス コンプライアンスの猶予期間が経過する DateTime</span><span class="sxs-lookup"><span data-stu-id="f3bd2-334">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="f3bd2-335">serialNumber</span><span class="sxs-lookup"><span data-stu-id="f3bd2-335">serialNumber</span></span>|<span data-ttu-id="f3bd2-336">String</span><span class="sxs-lookup"><span data-stu-id="f3bd2-336">String</span></span>|<span data-ttu-id="f3bd2-337">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="f3bd2-337">SerialNumber</span></span>|
|<span data-ttu-id="f3bd2-338">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="f3bd2-338">phoneNumber</span></span>|<span data-ttu-id="f3bd2-339">String</span><span class="sxs-lookup"><span data-stu-id="f3bd2-339">String</span></span>|<span data-ttu-id="f3bd2-340">デバイスの電話番号</span><span class="sxs-lookup"><span data-stu-id="f3bd2-340">Phone number of the device</span></span>|
|<span data-ttu-id="f3bd2-341">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="f3bd2-341">androidSecurityPatchLevel</span></span>|<span data-ttu-id="f3bd2-342">String</span><span class="sxs-lookup"><span data-stu-id="f3bd2-342">String</span></span>|<span data-ttu-id="f3bd2-343">Android セキュリティ パッチのレベル</span><span class="sxs-lookup"><span data-stu-id="f3bd2-343">Android security patch level</span></span>|
|<span data-ttu-id="f3bd2-344">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="f3bd2-344">userDisplayName</span></span>|<span data-ttu-id="f3bd2-345">String</span><span class="sxs-lookup"><span data-stu-id="f3bd2-345">String</span></span>|<span data-ttu-id="f3bd2-346">ユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="f3bd2-346">User display name</span></span>|
|<span data-ttu-id="f3bd2-347">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="f3bd2-347">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="f3bd2-348">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="f3bd2-348">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="f3bd2-349">ConfigrMgr クライアント対応機能
</span><span class="sxs-lookup"><span data-stu-id="f3bd2-349">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="f3bd2-350">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="f3bd2-350">wiFiMacAddress</span></span>|<span data-ttu-id="f3bd2-351">String</span><span class="sxs-lookup"><span data-stu-id="f3bd2-351">String</span></span>|<span data-ttu-id="f3bd2-352">Wi-Fi MAC</span><span class="sxs-lookup"><span data-stu-id="f3bd2-352">Wi-Fi MAC</span></span>|
|<span data-ttu-id="f3bd2-353">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="f3bd2-353">deviceHealthAttestationState</span></span>|[<span data-ttu-id="f3bd2-354">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="f3bd2-354">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="f3bd2-355">デバイスの正常性構成証明の状態。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-355">The device health attestation state.</span></span>|
|<span data-ttu-id="f3bd2-356">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="f3bd2-356">subscriberCarrier</span></span>|<span data-ttu-id="f3bd2-357">String</span><span class="sxs-lookup"><span data-stu-id="f3bd2-357">String</span></span>|<span data-ttu-id="f3bd2-358">サブスクライバー通信事業者</span><span class="sxs-lookup"><span data-stu-id="f3bd2-358">Subscriber Carrier</span></span>|
|<span data-ttu-id="f3bd2-359">meid</span><span class="sxs-lookup"><span data-stu-id="f3bd2-359">meid</span></span>|<span data-ttu-id="f3bd2-360">String</span><span class="sxs-lookup"><span data-stu-id="f3bd2-360">String</span></span>|<span data-ttu-id="f3bd2-361">MEID</span><span class="sxs-lookup"><span data-stu-id="f3bd2-361">MEID</span></span>|
|<span data-ttu-id="f3bd2-362">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="f3bd2-362">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="f3bd2-363">Int64</span><span class="sxs-lookup"><span data-stu-id="f3bd2-363">Int64</span></span>|<span data-ttu-id="f3bd2-364">記憶域の合計 (バイト)</span><span class="sxs-lookup"><span data-stu-id="f3bd2-364">Total Storage in Bytes</span></span>|
|<span data-ttu-id="f3bd2-365">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="f3bd2-365">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="f3bd2-366">Int64</span><span class="sxs-lookup"><span data-stu-id="f3bd2-366">Int64</span></span>|<span data-ttu-id="f3bd2-367">空き記憶域 (バイト)</span><span class="sxs-lookup"><span data-stu-id="f3bd2-367">Free Storage in Bytes</span></span>|
|<span data-ttu-id="f3bd2-368">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="f3bd2-368">managedDeviceName</span></span>|<span data-ttu-id="f3bd2-369">String</span><span class="sxs-lookup"><span data-stu-id="f3bd2-369">String</span></span>|<span data-ttu-id="f3bd2-370">デバイスを識別する名前が自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-370">Automatically generated name to identify a device.</span></span> <span data-ttu-id="f3bd2-371">ユーザー フレンドリ名に上書きできます。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-371">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="f3bd2-372">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="f3bd2-372">partnerReportedThreatState</span></span>|[<span data-ttu-id="f3bd2-373">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="f3bd2-373">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="f3bd2-374">Mobile Threat Defense パートナーがアカウントおよびデバイスで使用されている場合の、デバイスの脅威の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-374">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="f3bd2-375">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-375">Read Only.</span></span> <span data-ttu-id="f3bd2-376">可能な値は、`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured` です。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-376">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="f3bd2-377">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="f3bd2-377">usersLoggedOn</span></span>|<span data-ttu-id="f3bd2-378">[loggedOnUser](../resources/intune-devices-loggedonuser.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f3bd2-378">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="f3bd2-379">最後のデバイスのユーザーにログオンしていることを示します</span><span class="sxs-lookup"><span data-stu-id="f3bd2-379">Indicates the last logged on users of a device</span></span>|
|<span data-ttu-id="f3bd2-380">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3bd2-380">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="f3bd2-381">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3bd2-381">DateTimeOffset</span></span>|<span data-ttu-id="f3bd2-382">レポート preferMdmOverGroupPolicy 設定日付と時刻が設定されています。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-382">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="f3bd2-383">設定すると、Intune MDM 設定が優先されますグループ ポリシー設定の競合がある場合。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-383">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="f3bd2-384">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-384">Read Only.</span></span>|
|<span data-ttu-id="f3bd2-385">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="f3bd2-385">autopilotEnrolled</span></span>|<span data-ttu-id="f3bd2-386">ブール型</span><span class="sxs-lookup"><span data-stu-id="f3bd2-386">Boolean</span></span>|<span data-ttu-id="f3bd2-387">自動操縦を使用して管理対象のデバイスが登録されている場合にレポートします。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-387">Reports if the managed device is enrolled via auto-pilot.</span></span>|
|<span data-ttu-id="f3bd2-388">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="f3bd2-388">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="f3bd2-389">ブール型</span><span class="sxs-lookup"><span data-stu-id="f3bd2-389">Boolean</span></span>|<span data-ttu-id="f3bd2-390">マネージ iOS デバイスがユーザーの承認登録の場合にレポートします。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-390">Reports if the managed iOS device is user approval enrollment.</span></span>|
|<span data-ttu-id="f3bd2-391">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="f3bd2-391">managementCertificateExpirationDate</span></span>|<span data-ttu-id="f3bd2-392">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3bd2-392">DateTimeOffset</span></span>|<span data-ttu-id="f3bd2-393">デバイスの管理の証明書の有効期限の日付をレポート</span><span class="sxs-lookup"><span data-stu-id="f3bd2-393">Reports device management certificate expiration date</span></span>|
|<span data-ttu-id="f3bd2-394">iccid</span><span class="sxs-lookup"><span data-stu-id="f3bd2-394">iccid</span></span>|<span data-ttu-id="f3bd2-395">String</span><span class="sxs-lookup"><span data-stu-id="f3bd2-395">String</span></span>|<span data-ttu-id="f3bd2-396">A SIM カードの一意の識別番号は集積回路カードの識別子です。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-396">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span>|
|<span data-ttu-id="f3bd2-397">udid</span><span class="sxs-lookup"><span data-stu-id="f3bd2-397">udid</span></span>|<span data-ttu-id="f3bd2-398">String</span><span class="sxs-lookup"><span data-stu-id="f3bd2-398">String</span></span>|<span data-ttu-id="f3bd2-399">IOS と macOS デバイスに一意のデバイス識別子です。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-399">Unique Device Identifier for iOS and macOS devices.</span></span>|
|<span data-ttu-id="f3bd2-400">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f3bd2-400">roleScopeTagIds</span></span>|<span data-ttu-id="f3bd2-401">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f3bd2-401">String collection</span></span>|<span data-ttu-id="f3bd2-402">このデバイス インスタンスのスコープのタグ Id のリストです。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-402">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="f3bd2-403">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="f3bd2-403">windowsActiveMalwareCount</span></span>|<span data-ttu-id="f3bd2-404">Int32</span><span class="sxs-lookup"><span data-stu-id="f3bd2-404">Int32</span></span>|<span data-ttu-id="f3bd2-405">この windows デバイスのアクティブなマルウェアの数</span><span class="sxs-lookup"><span data-stu-id="f3bd2-405">Count of active malware for this windows device</span></span>|
|<span data-ttu-id="f3bd2-406">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="f3bd2-406">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="f3bd2-407">Int32</span><span class="sxs-lookup"><span data-stu-id="f3bd2-407">Int32</span></span>|<span data-ttu-id="f3bd2-408">この windows デバイス用の修正されたマルウェアの数</span><span class="sxs-lookup"><span data-stu-id="f3bd2-408">Count of remediated malware for this windows device</span></span>|
|<span data-ttu-id="f3bd2-409">notes</span><span class="sxs-lookup"><span data-stu-id="f3bd2-409">notes</span></span>|<span data-ttu-id="f3bd2-410">String</span><span class="sxs-lookup"><span data-stu-id="f3bd2-410">String</span></span>|<span data-ttu-id="f3bd2-411">IT 管理者によって作成されたデバイスに関する注意事項</span><span class="sxs-lookup"><span data-stu-id="f3bd2-411">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="f3bd2-412">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="f3bd2-412">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="f3bd2-413">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="f3bd2-413">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="f3bd2-414">構成マネージャー クライアント正常性の状態、または構成マネージャーの MDM エージェントによって管理されるデバイスに対してのみ有効です。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-414">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3bd2-415">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f3bd2-415">Relationships</span></span>
|<span data-ttu-id="f3bd2-416">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f3bd2-416">Relationship</span></span>|<span data-ttu-id="f3bd2-417">型</span><span class="sxs-lookup"><span data-stu-id="f3bd2-417">Type</span></span>|<span data-ttu-id="f3bd2-418">説明</span><span class="sxs-lookup"><span data-stu-id="f3bd2-418">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3bd2-419">detectedApps</span><span class="sxs-lookup"><span data-stu-id="f3bd2-419">detectedApps</span></span>|<span data-ttu-id="f3bd2-420">[detectedApp](../resources/intune-devices-detectedapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f3bd2-420">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="f3bd2-421">デバイス上に現在インストールされているすべてのアプリケーション</span><span class="sxs-lookup"><span data-stu-id="f3bd2-421">All applications currently installed on the device</span></span>|
|<span data-ttu-id="f3bd2-422">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="f3bd2-422">deviceCategory</span></span>|[<span data-ttu-id="f3bd2-423">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="f3bd2-423">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="f3bd2-424">デバイス カテゴリ</span><span class="sxs-lookup"><span data-stu-id="f3bd2-424">Device category</span></span>|
|<span data-ttu-id="f3bd2-425">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="f3bd2-425">windowsProtectionState</span></span>|[<span data-ttu-id="f3bd2-426">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="f3bd2-426">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="f3bd2-427">デバイス保護の状態です。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-427">The device protection status.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f3bd2-428">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f3bd2-428">JSON Representation</span></span>
<span data-ttu-id="f3bd2-429">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f3bd2-429">Here is a JSON representation of the resource.</span></span>
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
    "windowsUpdateForBusiness": true
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





