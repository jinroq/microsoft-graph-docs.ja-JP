---
title: managedDevice リソース タイプ
description: Intune 経由で管理または事前登録されるデバイス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a2233c1dea3dfc8992becf1a12c8e99f1938020a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522077"
---
# <a name="manageddevice-resource-type"></a><span data-ttu-id="0e6f7-103">managedDevice リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="0e6f7-103">managedDevice resource type</span></span>

> <span data-ttu-id="0e6f7-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e6f7-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e6f7-106">Intune 経由で管理または事前登録されるデバイス</span><span class="sxs-lookup"><span data-stu-id="0e6f7-106">Devices that are managed or pre-enrolled through Intune</span></span>

## <a name="methods"></a><span data-ttu-id="0e6f7-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="0e6f7-107">Methods</span></span>
|<span data-ttu-id="0e6f7-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0e6f7-108">Method</span></span>|<span data-ttu-id="0e6f7-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0e6f7-109">Return Type</span></span>|<span data-ttu-id="0e6f7-110">説明</span><span class="sxs-lookup"><span data-stu-id="0e6f7-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0e6f7-111">Get managedDevice</span><span class="sxs-lookup"><span data-stu-id="0e6f7-111">Get managedDevice</span></span>](../api/intune-devices-manageddevice-get.md)|[<span data-ttu-id="0e6f7-112">managedDevice</span><span class="sxs-lookup"><span data-stu-id="0e6f7-112">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="0e6f7-113">[managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-113">Read properties and relationships of the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="0e6f7-114">Update managedDevice</span><span class="sxs-lookup"><span data-stu-id="0e6f7-114">Update managedDevice</span></span>](../api/intune-devices-manageddevice-update.md)|[<span data-ttu-id="0e6f7-115">managedDevice</span><span class="sxs-lookup"><span data-stu-id="0e6f7-115">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="0e6f7-116">[managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-116">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="0e6f7-117">executeAction アクション</span><span class="sxs-lookup"><span data-stu-id="0e6f7-117">executeAction action</span></span>](../api/intune-devices-manageddevice-executeaction.md)|[<span data-ttu-id="0e6f7-118">bulkManagedDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="0e6f7-118">bulkManagedDeviceActionResult</span></span>](../resources/intune-devices-bulkmanageddeviceactionresult.md)|<span data-ttu-id="0e6f7-119">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0e6f7-119">Not yet documented</span></span>|
|[<span data-ttu-id="0e6f7-120">enableLostMode アクション</span><span class="sxs-lookup"><span data-stu-id="0e6f7-120">enableLostMode action</span></span>](../api/intune-devices-manageddevice-enablelostmode.md)|<span data-ttu-id="0e6f7-121">なし</span><span class="sxs-lookup"><span data-stu-id="0e6f7-121">None</span></span>|<span data-ttu-id="0e6f7-122">削除モードを有効にする</span><span class="sxs-lookup"><span data-stu-id="0e6f7-122">Enable lost mode</span></span>|
|[<span data-ttu-id="0e6f7-123">playLostModeSound アクション</span><span class="sxs-lookup"><span data-stu-id="0e6f7-123">playLostModeSound action</span></span>](../api/intune-devices-manageddevice-playlostmodesound.md)|<span data-ttu-id="0e6f7-124">なし</span><span class="sxs-lookup"><span data-stu-id="0e6f7-124">None</span></span>|<span data-ttu-id="0e6f7-125">リモート ロック</span><span class="sxs-lookup"><span data-stu-id="0e6f7-125">Remote lock</span></span>|
|[<span data-ttu-id="0e6f7-126">setDeviceName アクション</span><span class="sxs-lookup"><span data-stu-id="0e6f7-126">setDeviceName action</span></span>](../api/intune-devices-manageddevice-setdevicename.md)|<span data-ttu-id="0e6f7-127">なし</span><span class="sxs-lookup"><span data-stu-id="0e6f7-127">None</span></span>|<span data-ttu-id="0e6f7-128">デバイスのデバイス名を設定します。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-128">Set device name of the device.</span></span>|
|[<span data-ttu-id="0e6f7-129">retire action</span><span class="sxs-lookup"><span data-stu-id="0e6f7-129">retire action</span></span>](../api/intune-devices-manageddevice-retire.md)|<span data-ttu-id="0e6f7-130">なし</span><span class="sxs-lookup"><span data-stu-id="0e6f7-130">None</span></span>|<span data-ttu-id="0e6f7-131">デバイスを破棄します</span><span class="sxs-lookup"><span data-stu-id="0e6f7-131">Retire a device</span></span>|
|[<span data-ttu-id="0e6f7-132">wipe action</span><span class="sxs-lookup"><span data-stu-id="0e6f7-132">wipe action</span></span>](../api/intune-devices-manageddevice-wipe.md)|<span data-ttu-id="0e6f7-133">なし</span><span class="sxs-lookup"><span data-stu-id="0e6f7-133">None</span></span>|<span data-ttu-id="0e6f7-134">デバイスをワイプします</span><span class="sxs-lookup"><span data-stu-id="0e6f7-134">Wipe a device</span></span>|
|[<span data-ttu-id="0e6f7-135">resetPasscode action</span><span class="sxs-lookup"><span data-stu-id="0e6f7-135">resetPasscode action</span></span>](../api/intune-devices-manageddevice-resetpasscode.md)|<span data-ttu-id="0e6f7-136">なし</span><span class="sxs-lookup"><span data-stu-id="0e6f7-136">None</span></span>|<span data-ttu-id="0e6f7-137">パスコードをリセットします</span><span class="sxs-lookup"><span data-stu-id="0e6f7-137">Reset passcode</span></span>|
|[<span data-ttu-id="0e6f7-138">remoteLock action</span><span class="sxs-lookup"><span data-stu-id="0e6f7-138">remoteLock action</span></span>](../api/intune-devices-manageddevice-remotelock.md)|<span data-ttu-id="0e6f7-139">なし</span><span class="sxs-lookup"><span data-stu-id="0e6f7-139">None</span></span>|<span data-ttu-id="0e6f7-140">リモート ロック</span><span class="sxs-lookup"><span data-stu-id="0e6f7-140">Remote lock</span></span>|
|[<span data-ttu-id="0e6f7-141">requestRemoteAssistance action</span><span class="sxs-lookup"><span data-stu-id="0e6f7-141">requestRemoteAssistance action</span></span>](../api/intune-devices-manageddevice-requestremoteassistance.md)|<span data-ttu-id="0e6f7-142">なし</span><span class="sxs-lookup"><span data-stu-id="0e6f7-142">None</span></span>|<span data-ttu-id="0e6f7-143">リモート アシスタンスを要求します</span><span class="sxs-lookup"><span data-stu-id="0e6f7-143">Request remote assistance</span></span>|
|[<span data-ttu-id="0e6f7-144">disableLostMode action</span><span class="sxs-lookup"><span data-stu-id="0e6f7-144">disableLostMode action</span></span>](../api/intune-devices-manageddevice-disablelostmode.md)|<span data-ttu-id="0e6f7-145">なし</span><span class="sxs-lookup"><span data-stu-id="0e6f7-145">None</span></span>|<span data-ttu-id="0e6f7-146">紛失モードを無効化します</span><span class="sxs-lookup"><span data-stu-id="0e6f7-146">Disable lost mode</span></span>|
|[<span data-ttu-id="0e6f7-147">locateDevice action</span><span class="sxs-lookup"><span data-stu-id="0e6f7-147">locateDevice action</span></span>](../api/intune-devices-manageddevice-locatedevice.md)|<span data-ttu-id="0e6f7-148">なし</span><span class="sxs-lookup"><span data-stu-id="0e6f7-148">None</span></span>|<span data-ttu-id="0e6f7-149">デバイスを検索します</span><span class="sxs-lookup"><span data-stu-id="0e6f7-149">Locate a device</span></span>|
|[<span data-ttu-id="0e6f7-150">bypassActivationLock action</span><span class="sxs-lookup"><span data-stu-id="0e6f7-150">bypassActivationLock action</span></span>](../api/intune-devices-manageddevice-bypassactivationlock.md)|<span data-ttu-id="0e6f7-151">なし</span><span class="sxs-lookup"><span data-stu-id="0e6f7-151">None</span></span>|<span data-ttu-id="0e6f7-152">アクティベーション ロックをバイパスします</span><span class="sxs-lookup"><span data-stu-id="0e6f7-152">Bypass activation lock</span></span>|
|[<span data-ttu-id="0e6f7-153">rebootNow action</span><span class="sxs-lookup"><span data-stu-id="0e6f7-153">rebootNow action</span></span>](../api/intune-devices-manageddevice-rebootnow.md)|<span data-ttu-id="0e6f7-154">なし</span><span class="sxs-lookup"><span data-stu-id="0e6f7-154">None</span></span>|<span data-ttu-id="0e6f7-155">デバイスを再起動します</span><span class="sxs-lookup"><span data-stu-id="0e6f7-155">Reboot device</span></span>|
|[<span data-ttu-id="0e6f7-156">shutDown action</span><span class="sxs-lookup"><span data-stu-id="0e6f7-156">shutDown action</span></span>](../api/intune-devices-manageddevice-shutdown.md)|<span data-ttu-id="0e6f7-157">なし</span><span class="sxs-lookup"><span data-stu-id="0e6f7-157">None</span></span>|<span data-ttu-id="0e6f7-158">デバイスをシャットダウンします</span><span class="sxs-lookup"><span data-stu-id="0e6f7-158">Shut down device</span></span>|
|[<span data-ttu-id="0e6f7-159">recoverPasscode action</span><span class="sxs-lookup"><span data-stu-id="0e6f7-159">recoverPasscode action</span></span>](../api/intune-devices-manageddevice-recoverpasscode.md)|<span data-ttu-id="0e6f7-160">なし</span><span class="sxs-lookup"><span data-stu-id="0e6f7-160">None</span></span>|<span data-ttu-id="0e6f7-161">パスコードを回復します</span><span class="sxs-lookup"><span data-stu-id="0e6f7-161">Recover passcode</span></span>|
|[<span data-ttu-id="0e6f7-162">cleanWindowsDevice action</span><span class="sxs-lookup"><span data-stu-id="0e6f7-162">cleanWindowsDevice action</span></span>](../api/intune-devices-manageddevice-cleanwindowsdevice.md)|<span data-ttu-id="0e6f7-163">なし</span><span class="sxs-lookup"><span data-stu-id="0e6f7-163">None</span></span>|<span data-ttu-id="0e6f7-164">Windows デバイスをクリーンにします</span><span class="sxs-lookup"><span data-stu-id="0e6f7-164">Clean Windows device</span></span>|
|[<span data-ttu-id="0e6f7-165">logoutSharedAppleDeviceActiveUser action</span><span class="sxs-lookup"><span data-stu-id="0e6f7-165">logoutSharedAppleDeviceActiveUser action</span></span>](../api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser.md)|<span data-ttu-id="0e6f7-166">なし</span><span class="sxs-lookup"><span data-stu-id="0e6f7-166">None</span></span>|<span data-ttu-id="0e6f7-167">共有の Apple デバイスのアクティブなユーザーをログアウトします</span><span class="sxs-lookup"><span data-stu-id="0e6f7-167">Logout shared Apple device active user</span></span>|
|[<span data-ttu-id="0e6f7-168">deleteUserFromSharedAppleDevice action</span><span class="sxs-lookup"><span data-stu-id="0e6f7-168">deleteUserFromSharedAppleDevice action</span></span>](../api/intune-devices-manageddevice-deleteuserfromsharedappledevice.md)|<span data-ttu-id="0e6f7-169">なし</span><span class="sxs-lookup"><span data-stu-id="0e6f7-169">None</span></span>|<span data-ttu-id="0e6f7-170">共有の Apple デバイスからユーザーを削除します</span><span class="sxs-lookup"><span data-stu-id="0e6f7-170">Delete user from shared Apple device</span></span>|
|[<span data-ttu-id="0e6f7-171">syncDevice action</span><span class="sxs-lookup"><span data-stu-id="0e6f7-171">syncDevice action</span></span>](../api/intune-devices-manageddevice-syncdevice.md)|<span data-ttu-id="0e6f7-172">なし</span><span class="sxs-lookup"><span data-stu-id="0e6f7-172">None</span></span>|<span data-ttu-id="0e6f7-173">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0e6f7-173">Not yet documented</span></span>|
|[<span data-ttu-id="0e6f7-174">windowsDefenderScan action</span><span class="sxs-lookup"><span data-stu-id="0e6f7-174">windowsDefenderScan action</span></span>](../api/intune-devices-manageddevice-windowsdefenderscan.md)|<span data-ttu-id="0e6f7-175">なし</span><span class="sxs-lookup"><span data-stu-id="0e6f7-175">None</span></span>|<span data-ttu-id="0e6f7-176">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0e6f7-176">Not yet documented</span></span>|
|[<span data-ttu-id="0e6f7-177">windowsDefenderUpdateSignatures action</span><span class="sxs-lookup"><span data-stu-id="0e6f7-177">windowsDefenderUpdateSignatures action</span></span>](../api/intune-devices-manageddevice-windowsdefenderupdatesignatures.md)|<span data-ttu-id="0e6f7-178">なし</span><span class="sxs-lookup"><span data-stu-id="0e6f7-178">None</span></span>|<span data-ttu-id="0e6f7-179">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0e6f7-179">Not yet documented</span></span>|
|[<span data-ttu-id="0e6f7-180">updateWindowsDeviceAccount action</span><span class="sxs-lookup"><span data-stu-id="0e6f7-180">updateWindowsDeviceAccount action</span></span>](../api/intune-devices-manageddevice-updatewindowsdeviceaccount.md)|<span data-ttu-id="0e6f7-181">なし</span><span class="sxs-lookup"><span data-stu-id="0e6f7-181">None</span></span>|<span data-ttu-id="0e6f7-182">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0e6f7-182">Not yet documented</span></span>|
|[<span data-ttu-id="0e6f7-183">revokeAppleVppLicenses アクション</span><span class="sxs-lookup"><span data-stu-id="0e6f7-183">revokeAppleVppLicenses action</span></span>](../api/intune-devices-manageddevice-revokeapplevpplicenses.md)|<span data-ttu-id="0e6f7-184">なし</span><span class="sxs-lookup"><span data-stu-id="0e6f7-184">None</span></span>|<span data-ttu-id="0e6f7-185">デバイスのすべての Apple Vpp ライセンスを取り消す</span><span class="sxs-lookup"><span data-stu-id="0e6f7-185">Revoke all Apple Vpp licenses for a device</span></span>|

## <a name="properties"></a><span data-ttu-id="0e6f7-186">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e6f7-186">Properties</span></span>
|<span data-ttu-id="0e6f7-187">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e6f7-187">Property</span></span>|<span data-ttu-id="0e6f7-188">型</span><span class="sxs-lookup"><span data-stu-id="0e6f7-188">Type</span></span>|<span data-ttu-id="0e6f7-189">説明</span><span class="sxs-lookup"><span data-stu-id="0e6f7-189">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e6f7-190">id</span><span class="sxs-lookup"><span data-stu-id="0e6f7-190">id</span></span>|<span data-ttu-id="0e6f7-191">String</span><span class="sxs-lookup"><span data-stu-id="0e6f7-191">String</span></span>|<span data-ttu-id="0e6f7-192">デバイスの一意識別子</span><span class="sxs-lookup"><span data-stu-id="0e6f7-192">Unique Identifier for the device</span></span>|
|<span data-ttu-id="0e6f7-193">userId</span><span class="sxs-lookup"><span data-stu-id="0e6f7-193">userId</span></span>|<span data-ttu-id="0e6f7-194">String</span><span class="sxs-lookup"><span data-stu-id="0e6f7-194">String</span></span>|<span data-ttu-id="0e6f7-195">デバイスに関連付けられているユーザーの一意の識別子</span><span class="sxs-lookup"><span data-stu-id="0e6f7-195">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="0e6f7-196">deviceName</span><span class="sxs-lookup"><span data-stu-id="0e6f7-196">deviceName</span></span>|<span data-ttu-id="0e6f7-197">String</span><span class="sxs-lookup"><span data-stu-id="0e6f7-197">String</span></span>|<span data-ttu-id="0e6f7-198">デバイスの名前</span><span class="sxs-lookup"><span data-stu-id="0e6f7-198">Name of the device</span></span>|
|<span data-ttu-id="0e6f7-199">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="0e6f7-199">hardwareInformation</span></span>|[<span data-ttu-id="0e6f7-200">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="0e6f7-200">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="0e6f7-201">デバイスのハードワードの詳細。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-201">The hardward details for the device.</span></span>  <span data-ttu-id="0e6f7-202">記憶領域、製造元、シリアル番号などの情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-202">Includes information such as storage space, manufacturer, serial number, etc.</span></span>|
|<span data-ttu-id="0e6f7-203">ownerType</span><span class="sxs-lookup"><span data-stu-id="0e6f7-203">ownerType</span></span>|[<span data-ttu-id="0e6f7-204">ownerType</span><span class="sxs-lookup"><span data-stu-id="0e6f7-204">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="0e6f7-205">デバイスの所有権。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-205">Ownership of the device.</span></span> <span data-ttu-id="0e6f7-206">' company ' または ' personal ' にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-206">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="0e6f7-207">使用可能な値は、`unknown`、`company`、`personal` です。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-207">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="0e6f7-208">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="0e6f7-208">managedDeviceOwnerType</span></span>|[<span data-ttu-id="0e6f7-209">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="0e6f7-209">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="0e6f7-210">デバイスの所有権。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-210">Ownership of the device.</span></span> <span data-ttu-id="0e6f7-211">' company ' または ' personal ' にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-211">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="0e6f7-212">使用可能な値は、`unknown`、`company`、`personal` です。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-212">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="0e6f7-213">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="0e6f7-213">deviceActionResults</span></span>|<span data-ttu-id="0e6f7-214">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0e6f7-214">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="0e6f7-215">ComplexType deviceActionResult オブジェクトのリスト。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-215">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="0e6f7-216">managementstate</span><span class="sxs-lookup"><span data-stu-id="0e6f7-216">managementState</span></span>|[<span data-ttu-id="0e6f7-217">managementstate</span><span class="sxs-lookup"><span data-stu-id="0e6f7-217">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="0e6f7-218">デバイスの管理状態。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-218">Management state of the device.</span></span> <span data-ttu-id="0e6f7-219">可能な値は、`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered` です。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-219">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="0e6f7-220">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="0e6f7-220">enrolledDateTime</span></span>|<span data-ttu-id="0e6f7-221">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e6f7-221">DateTimeOffset</span></span>|<span data-ttu-id="0e6f7-222">デバイスの登録時刻。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-222">Enrollment time of the device.</span></span>|
|<span data-ttu-id="0e6f7-223">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0e6f7-223">lastSyncDateTime</span></span>|<span data-ttu-id="0e6f7-224">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e6f7-224">DateTimeOffset</span></span>|<span data-ttu-id="0e6f7-225">デバイスが Intune との正常な同期を最終的に完了した日時。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-225">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="0e6f7-226">chassisType</span><span class="sxs-lookup"><span data-stu-id="0e6f7-226">chassisType</span></span>|[<span data-ttu-id="0e6f7-227">chassisType</span><span class="sxs-lookup"><span data-stu-id="0e6f7-227">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="0e6f7-228">デバイスのシャーシの種類。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-228">Chassis type of the device.</span></span> <span data-ttu-id="0e6f7-229">可能な値は、`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown` です。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-229">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="0e6f7-230">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="0e6f7-230">operatingSystem</span></span>|<span data-ttu-id="0e6f7-231">文字列</span><span class="sxs-lookup"><span data-stu-id="0e6f7-231">String</span></span>|<span data-ttu-id="0e6f7-232">デバイスのオペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-232">Operating system of the device.</span></span> <span data-ttu-id="0e6f7-233">Windows、iOS など。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-233">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="0e6f7-234">deviceType</span><span class="sxs-lookup"><span data-stu-id="0e6f7-234">deviceType</span></span>|[<span data-ttu-id="0e6f7-235">deviceType</span><span class="sxs-lookup"><span data-stu-id="0e6f7-235">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="0e6f7-236">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-236">Platform of the device.</span></span> <span data-ttu-id="0e6f7-237">可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="0e6f7-237">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="0e6f7-238">complianceState</span><span class="sxs-lookup"><span data-stu-id="0e6f7-238">complianceState</span></span>|[<span data-ttu-id="0e6f7-239">complianceState</span><span class="sxs-lookup"><span data-stu-id="0e6f7-239">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="0e6f7-240">デバイスのコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-240">Compliance state of the device.</span></span> <span data-ttu-id="0e6f7-241">可能な値は、`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager` です。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-241">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="0e6f7-242">jailBroken</span><span class="sxs-lookup"><span data-stu-id="0e6f7-242">jailBroken</span></span>|<span data-ttu-id="0e6f7-243">String</span><span class="sxs-lookup"><span data-stu-id="0e6f7-243">String</span></span>|<span data-ttu-id="0e6f7-244">デバイスが脱獄またはルート化されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-244">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="0e6f7-245">managementAgent</span><span class="sxs-lookup"><span data-stu-id="0e6f7-245">managementAgent</span></span>|[<span data-ttu-id="0e6f7-246">managementagenttype</span><span class="sxs-lookup"><span data-stu-id="0e6f7-246">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="0e6f7-247">デバイスの管理チャネル。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-247">Management channel of the device.</span></span> <span data-ttu-id="0e6f7-248">Intune、EAS など。可能な値は`eas`、 `mdm`、 `easMdm` `intuneClient` `easIntuneClient` `configurationManagerClient` `jamf` `googleCloudDevicePolicyController`、、、、、、、、、 `microsoft365ManagedMdm`、、です。 `configurationManagerClientMdm` `configurationManagerClientMdmEas` `unknown`</span><span class="sxs-lookup"><span data-stu-id="0e6f7-248">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="0e6f7-249">osVersion</span><span class="sxs-lookup"><span data-stu-id="0e6f7-249">osVersion</span></span>|<span data-ttu-id="0e6f7-250">String</span><span class="sxs-lookup"><span data-stu-id="0e6f7-250">String</span></span>|<span data-ttu-id="0e6f7-251">デバイスのオペレーティング システムのバージョン。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-251">Operating system version of the device.</span></span>|
|<span data-ttu-id="0e6f7-252">easActivated</span><span class="sxs-lookup"><span data-stu-id="0e6f7-252">easActivated</span></span>|<span data-ttu-id="0e6f7-253">ブール型</span><span class="sxs-lookup"><span data-stu-id="0e6f7-253">Boolean</span></span>|<span data-ttu-id="0e6f7-254">Exchange ActiveSync がアクティブになっているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-254">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="0e6f7-255">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="0e6f7-255">easDeviceId</span></span>|<span data-ttu-id="0e6f7-256">String</span><span class="sxs-lookup"><span data-stu-id="0e6f7-256">String</span></span>|<span data-ttu-id="0e6f7-257">デバイスの Exchange ActiveSync の ID。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-257">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="0e6f7-258">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="0e6f7-258">easActivationDateTime</span></span>|<span data-ttu-id="0e6f7-259">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e6f7-259">DateTimeOffset</span></span>|<span data-ttu-id="0e6f7-260">デバイスの Exchange ActivationSync のアクティブ化の時刻。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-260">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="0e6f7-261">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="0e6f7-261">aadRegistered</span></span>|<span data-ttu-id="0e6f7-262">ブール型</span><span class="sxs-lookup"><span data-stu-id="0e6f7-262">Boolean</span></span>|<span data-ttu-id="0e6f7-263">Azure Active Directory が登録されているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-263">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="0e6f7-264">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="0e6f7-264">azureADRegistered</span></span>|<span data-ttu-id="0e6f7-265">ブール型</span><span class="sxs-lookup"><span data-stu-id="0e6f7-265">Boolean</span></span>|<span data-ttu-id="0e6f7-266">Azure Active Directory が登録されているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-266">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="0e6f7-267">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="0e6f7-267">deviceEnrollmentType</span></span>|[<span data-ttu-id="0e6f7-268">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="0e6f7-268">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="0e6f7-269">デバイスの登録の種類。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-269">Enrollment type of the device.</span></span> <span data-ttu-id="0e6f7-270">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-270">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="0e6f7-271">lostModeState</span><span class="sxs-lookup"><span data-stu-id="0e6f7-271">lostModeState</span></span>|[<span data-ttu-id="0e6f7-272">lostModeState</span><span class="sxs-lookup"><span data-stu-id="0e6f7-272">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="0e6f7-273">失われたモードが有効か無効かを示します。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-273">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="0e6f7-274">可能な値は、`disabled`、`enabled` です。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-274">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="0e6f7-275">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="0e6f7-275">activationLockBypassCode</span></span>|<span data-ttu-id="0e6f7-276">String</span><span class="sxs-lookup"><span data-stu-id="0e6f7-276">String</span></span>|<span data-ttu-id="0e6f7-277">デバイスのアクティベーション ロックをバイパスするためのコード。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-277">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="0e6f7-278">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0e6f7-278">emailAddress</span></span>|<span data-ttu-id="0e6f7-279">String</span><span class="sxs-lookup"><span data-stu-id="0e6f7-279">String</span></span>|<span data-ttu-id="0e6f7-280">デバイスに関連付けられているユーザーの電子メール</span><span class="sxs-lookup"><span data-stu-id="0e6f7-280">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="0e6f7-281">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="0e6f7-281">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="0e6f7-282">String</span><span class="sxs-lookup"><span data-stu-id="0e6f7-282">String</span></span>|<span data-ttu-id="0e6f7-283">Azure Active Directory デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-283">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="0e6f7-284">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-284">Read only.</span></span>|
|<span data-ttu-id="0e6f7-285">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="0e6f7-285">azureADDeviceId</span></span>|<span data-ttu-id="0e6f7-286">String</span><span class="sxs-lookup"><span data-stu-id="0e6f7-286">String</span></span>|<span data-ttu-id="0e6f7-287">Azure Active Directory デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-287">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="0e6f7-288">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-288">Read only.</span></span>|
|<span data-ttu-id="0e6f7-289">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="0e6f7-289">deviceRegistrationState</span></span>|[<span data-ttu-id="0e6f7-290">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="0e6f7-290">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="0e6f7-291">デバイスの登録状態。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-291">Device registration state.</span></span> <span data-ttu-id="0e6f7-292">可能な値は、`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-292">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="0e6f7-293">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="0e6f7-293">deviceCategoryDisplayName</span></span>|<span data-ttu-id="0e6f7-294">String</span><span class="sxs-lookup"><span data-stu-id="0e6f7-294">String</span></span>|<span data-ttu-id="0e6f7-295">デバイス カテゴリの表示名</span><span class="sxs-lookup"><span data-stu-id="0e6f7-295">Device category display name</span></span>|
|<span data-ttu-id="0e6f7-296">isSupervised</span><span class="sxs-lookup"><span data-stu-id="0e6f7-296">isSupervised</span></span>|<span data-ttu-id="0e6f7-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e6f7-297">Boolean</span></span>|<span data-ttu-id="0e6f7-298">デバイスの管理状況</span><span class="sxs-lookup"><span data-stu-id="0e6f7-298">Device supervised status</span></span>|
|<span data-ttu-id="0e6f7-299">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0e6f7-299">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="0e6f7-300">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e6f7-300">DateTimeOffset</span></span>|<span data-ttu-id="0e6f7-301">最後にデバイスが Exchange に接続した時刻。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-301">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="0e6f7-302">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="0e6f7-302">exchangeAccessState</span></span>|[<span data-ttu-id="0e6f7-303">devicemanagementexchangeaccessstate</span><span class="sxs-lookup"><span data-stu-id="0e6f7-303">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="0e6f7-304">Exchange でのデバイスのアクセスの状態。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-304">The Access State of the device in Exchange.</span></span> <span data-ttu-id="0e6f7-305">可能な値は、`none`、`unknown`、`allowed`、`blocked`、`quarantined` です。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-305">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="0e6f7-306">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="0e6f7-306">exchangeAccessStateReason</span></span>|[<span data-ttu-id="0e6f7-307">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="0e6f7-307">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="0e6f7-308">Exchange でのデバイスのアクセス状態の理由。
</span><span class="sxs-lookup"><span data-stu-id="0e6f7-308">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="0e6f7-309">可能な値は、`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp` です。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-309">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="0e6f7-310">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="0e6f7-310">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="0e6f7-311">String</span><span class="sxs-lookup"><span data-stu-id="0e6f7-311">String</span></span>|<span data-ttu-id="0e6f7-312">デバイスとのリモート アシスタンス セッションを確立できるようにする URL。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-312">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="0e6f7-313">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="0e6f7-313">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="0e6f7-314">String</span><span class="sxs-lookup"><span data-stu-id="0e6f7-314">String</span></span>|<span data-ttu-id="0e6f7-315">リモート アシスタンス セッション オブジェクトの作成時に問題を識別するエラー文字列。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-315">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="0e6f7-316">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="0e6f7-316">isEncrypted</span></span>|<span data-ttu-id="0e6f7-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e6f7-317">Boolean</span></span>|<span data-ttu-id="0e6f7-318">デバイスの暗号化の状態</span><span class="sxs-lookup"><span data-stu-id="0e6f7-318">Device encryption status</span></span>|
|<span data-ttu-id="0e6f7-319">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0e6f7-319">userPrincipalName</span></span>|<span data-ttu-id="0e6f7-320">String</span><span class="sxs-lookup"><span data-stu-id="0e6f7-320">String</span></span>|<span data-ttu-id="0e6f7-321">デバイスのユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-321">Device user principal name</span></span>|
|<span data-ttu-id="0e6f7-322">model</span><span class="sxs-lookup"><span data-stu-id="0e6f7-322">model</span></span>|<span data-ttu-id="0e6f7-323">String</span><span class="sxs-lookup"><span data-stu-id="0e6f7-323">String</span></span>|<span data-ttu-id="0e6f7-324">デバイスのモデル</span><span class="sxs-lookup"><span data-stu-id="0e6f7-324">Model of the device</span></span>|
|<span data-ttu-id="0e6f7-325">manufacturer</span><span class="sxs-lookup"><span data-stu-id="0e6f7-325">manufacturer</span></span>|<span data-ttu-id="0e6f7-326">String</span><span class="sxs-lookup"><span data-stu-id="0e6f7-326">String</span></span>|<span data-ttu-id="0e6f7-327">デバイスのメーカー</span><span class="sxs-lookup"><span data-stu-id="0e6f7-327">Manufacturer of the device</span></span>|
|<span data-ttu-id="0e6f7-328">imei</span><span class="sxs-lookup"><span data-stu-id="0e6f7-328">imei</span></span>|<span data-ttu-id="0e6f7-329">String</span><span class="sxs-lookup"><span data-stu-id="0e6f7-329">String</span></span>|<span data-ttu-id="0e6f7-330">IMEI</span><span class="sxs-lookup"><span data-stu-id="0e6f7-330">IMEI</span></span>|
|<span data-ttu-id="0e6f7-331">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0e6f7-331">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="0e6f7-332">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e6f7-332">DateTimeOffset</span></span>|<span data-ttu-id="0e6f7-333">デバイス コンプライアンスの猶予期間が経過する DateTime</span><span class="sxs-lookup"><span data-stu-id="0e6f7-333">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="0e6f7-334">serialNumber</span><span class="sxs-lookup"><span data-stu-id="0e6f7-334">serialNumber</span></span>|<span data-ttu-id="0e6f7-335">String</span><span class="sxs-lookup"><span data-stu-id="0e6f7-335">String</span></span>|<span data-ttu-id="0e6f7-336">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="0e6f7-336">SerialNumber</span></span>|
|<span data-ttu-id="0e6f7-337">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="0e6f7-337">phoneNumber</span></span>|<span data-ttu-id="0e6f7-338">String</span><span class="sxs-lookup"><span data-stu-id="0e6f7-338">String</span></span>|<span data-ttu-id="0e6f7-339">デバイスの電話番号</span><span class="sxs-lookup"><span data-stu-id="0e6f7-339">Phone number of the device</span></span>|
|<span data-ttu-id="0e6f7-340">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="0e6f7-340">androidSecurityPatchLevel</span></span>|<span data-ttu-id="0e6f7-341">String</span><span class="sxs-lookup"><span data-stu-id="0e6f7-341">String</span></span>|<span data-ttu-id="0e6f7-342">Android セキュリティ パッチのレベル</span><span class="sxs-lookup"><span data-stu-id="0e6f7-342">Android security patch level</span></span>|
|<span data-ttu-id="0e6f7-343">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="0e6f7-343">userDisplayName</span></span>|<span data-ttu-id="0e6f7-344">String</span><span class="sxs-lookup"><span data-stu-id="0e6f7-344">String</span></span>|<span data-ttu-id="0e6f7-345">ユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="0e6f7-345">User display name</span></span>|
|<span data-ttu-id="0e6f7-346">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="0e6f7-346">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="0e6f7-347">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="0e6f7-347">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="0e6f7-348">ConfigrMgr クライアント対応機能
</span><span class="sxs-lookup"><span data-stu-id="0e6f7-348">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="0e6f7-349">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="0e6f7-349">wiFiMacAddress</span></span>|<span data-ttu-id="0e6f7-350">String</span><span class="sxs-lookup"><span data-stu-id="0e6f7-350">String</span></span>|<span data-ttu-id="0e6f7-351">Wi-Fi MAC</span><span class="sxs-lookup"><span data-stu-id="0e6f7-351">Wi-Fi MAC</span></span>|
|<span data-ttu-id="0e6f7-352">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="0e6f7-352">deviceHealthAttestationState</span></span>|[<span data-ttu-id="0e6f7-353">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="0e6f7-353">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="0e6f7-354">デバイスの正常性構成証明の状態。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-354">The device health attestation state.</span></span>|
|<span data-ttu-id="0e6f7-355">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="0e6f7-355">subscriberCarrier</span></span>|<span data-ttu-id="0e6f7-356">String</span><span class="sxs-lookup"><span data-stu-id="0e6f7-356">String</span></span>|<span data-ttu-id="0e6f7-357">サブスクライバー通信事業者</span><span class="sxs-lookup"><span data-stu-id="0e6f7-357">Subscriber Carrier</span></span>|
|<span data-ttu-id="0e6f7-358">meid</span><span class="sxs-lookup"><span data-stu-id="0e6f7-358">meid</span></span>|<span data-ttu-id="0e6f7-359">String</span><span class="sxs-lookup"><span data-stu-id="0e6f7-359">String</span></span>|<span data-ttu-id="0e6f7-360">MEID</span><span class="sxs-lookup"><span data-stu-id="0e6f7-360">MEID</span></span>|
|<span data-ttu-id="0e6f7-361">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="0e6f7-361">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="0e6f7-362">Int64</span><span class="sxs-lookup"><span data-stu-id="0e6f7-362">Int64</span></span>|<span data-ttu-id="0e6f7-363">記憶域の合計 (バイト)</span><span class="sxs-lookup"><span data-stu-id="0e6f7-363">Total Storage in Bytes</span></span>|
|<span data-ttu-id="0e6f7-364">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="0e6f7-364">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="0e6f7-365">Int64</span><span class="sxs-lookup"><span data-stu-id="0e6f7-365">Int64</span></span>|<span data-ttu-id="0e6f7-366">空き記憶域 (バイト)</span><span class="sxs-lookup"><span data-stu-id="0e6f7-366">Free Storage in Bytes</span></span>|
|<span data-ttu-id="0e6f7-367">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="0e6f7-367">managedDeviceName</span></span>|<span data-ttu-id="0e6f7-368">String</span><span class="sxs-lookup"><span data-stu-id="0e6f7-368">String</span></span>|<span data-ttu-id="0e6f7-369">デバイスを識別する名前が自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-369">Automatically generated name to identify a device.</span></span> <span data-ttu-id="0e6f7-370">ユーザー フレンドリ名に上書きできます。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-370">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="0e6f7-371">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="0e6f7-371">partnerReportedThreatState</span></span>|[<span data-ttu-id="0e6f7-372">manageddevicepartnerreportedhealthstate</span><span class="sxs-lookup"><span data-stu-id="0e6f7-372">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="0e6f7-373">Mobile Threat Defense パートナーがアカウントおよびデバイスで使用されている場合の、デバイスの脅威の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-373">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="0e6f7-374">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-374">Read Only.</span></span> <span data-ttu-id="0e6f7-375">可能な値は、`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured` です。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-375">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="0e6f7-376">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="0e6f7-376">usersLoggedOn</span></span>|<span data-ttu-id="0e6f7-377">[loggedOnUser](../resources/intune-devices-loggedonuser.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0e6f7-377">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="0e6f7-378">デバイスの最後にログオンしたユーザーを示します</span><span class="sxs-lookup"><span data-stu-id="0e6f7-378">Indicates the last logged on users of a device</span></span>|
|<span data-ttu-id="0e6f7-379">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e6f7-379">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="0e6f7-380">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e6f7-380">DateTimeOffset</span></span>|<span data-ttu-id="0e6f7-381">preferMdmOverGroupPolicy の設定が設定された DateTime を報告します。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-381">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="0e6f7-382">設定すると、競合がある場合に Intune MDM 設定がグループポリシー設定を上書きします。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-382">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="0e6f7-383">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-383">Read Only.</span></span>|
|<span data-ttu-id="0e6f7-384">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="0e6f7-384">autopilotEnrolled</span></span>|<span data-ttu-id="0e6f7-385">ブール型</span><span class="sxs-lookup"><span data-stu-id="0e6f7-385">Boolean</span></span>|<span data-ttu-id="0e6f7-386">管理対象デバイスが自動パイロットで登録されているかどうかを報告します。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-386">Reports if the managed device is enrolled via auto-pilot.</span></span>|
|<span data-ttu-id="0e6f7-387">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="0e6f7-387">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="0e6f7-388">ブール型</span><span class="sxs-lookup"><span data-stu-id="0e6f7-388">Boolean</span></span>|<span data-ttu-id="0e6f7-389">管理対象 iOS デバイスがユーザー承認登録であるかどうかを報告します。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-389">Reports if the managed iOS device is user approval enrollment.</span></span>|
|<span data-ttu-id="0e6f7-390">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="0e6f7-390">managementCertificateExpirationDate</span></span>|<span data-ttu-id="0e6f7-391">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e6f7-391">DateTimeOffset</span></span>|<span data-ttu-id="0e6f7-392">デバイス管理証明書の有効期限を報告する</span><span class="sxs-lookup"><span data-stu-id="0e6f7-392">Reports device management certificate expiration date</span></span>|
|<span data-ttu-id="0e6f7-393">iccid</span><span class="sxs-lookup"><span data-stu-id="0e6f7-393">iccid</span></span>|<span data-ttu-id="0e6f7-394">String</span><span class="sxs-lookup"><span data-stu-id="0e6f7-394">String</span></span>|<span data-ttu-id="0e6f7-395">ic カード識別子。 SIM カードの一意の識別番号です。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-395">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span>|
|<span data-ttu-id="0e6f7-396">udid</span><span class="sxs-lookup"><span data-stu-id="0e6f7-396">udid</span></span>|<span data-ttu-id="0e6f7-397">String</span><span class="sxs-lookup"><span data-stu-id="0e6f7-397">String</span></span>|<span data-ttu-id="0e6f7-398">iOS および macOS デバイスの一意のデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-398">Unique Device Identifier for iOS and macOS devices.</span></span>|
|<span data-ttu-id="0e6f7-399">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0e6f7-399">roleScopeTagIds</span></span>|<span data-ttu-id="0e6f7-400">String collection</span><span class="sxs-lookup"><span data-stu-id="0e6f7-400">String collection</span></span>|<span data-ttu-id="0e6f7-401">このデバイスインスタンスの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-401">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="0e6f7-402">windowsactivemalwarecount 再計算</span><span class="sxs-lookup"><span data-stu-id="0e6f7-402">windowsActiveMalwareCount</span></span>|<span data-ttu-id="0e6f7-403">Int32</span><span class="sxs-lookup"><span data-stu-id="0e6f7-403">Int32</span></span>|<span data-ttu-id="0e6f7-404">この windows デバイスのアクティブなマルウェアの数</span><span class="sxs-lookup"><span data-stu-id="0e6f7-404">Count of active malware for this windows device</span></span>|
|<span data-ttu-id="0e6f7-405">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="0e6f7-405">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="0e6f7-406">Int32</span><span class="sxs-lookup"><span data-stu-id="0e6f7-406">Int32</span></span>|<span data-ttu-id="0e6f7-407">この windows デバイスの修復済みマルウェアの数</span><span class="sxs-lookup"><span data-stu-id="0e6f7-407">Count of remediated malware for this windows device</span></span>|
|<span data-ttu-id="0e6f7-408">notes</span><span class="sxs-lookup"><span data-stu-id="0e6f7-408">notes</span></span>|<span data-ttu-id="0e6f7-409">String</span><span class="sxs-lookup"><span data-stu-id="0e6f7-409">String</span></span>|<span data-ttu-id="0e6f7-410">IT 管理者によって作成されたデバイスのメモ</span><span class="sxs-lookup"><span data-stu-id="0e6f7-410">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="0e6f7-411">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="0e6f7-411">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="0e6f7-412">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="0e6f7-412">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="0e6f7-413">構成マネージャークライアントの正常性状態。 MDM/ConfigMgr エージェントによって管理されるデバイスに対してのみ有効です。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-413">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e6f7-414">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0e6f7-414">Relationships</span></span>
|<span data-ttu-id="0e6f7-415">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0e6f7-415">Relationship</span></span>|<span data-ttu-id="0e6f7-416">型</span><span class="sxs-lookup"><span data-stu-id="0e6f7-416">Type</span></span>|<span data-ttu-id="0e6f7-417">説明</span><span class="sxs-lookup"><span data-stu-id="0e6f7-417">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e6f7-418">detectedApps</span><span class="sxs-lookup"><span data-stu-id="0e6f7-418">detectedApps</span></span>|<span data-ttu-id="0e6f7-419">[detectedApp](../resources/intune-devices-detectedapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0e6f7-419">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="0e6f7-420">デバイスに現在インストールされているすべてのアプリケーション</span><span class="sxs-lookup"><span data-stu-id="0e6f7-420">All applications currently installed on the device</span></span>|
|<span data-ttu-id="0e6f7-421">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="0e6f7-421">deviceCategory</span></span>|[<span data-ttu-id="0e6f7-422">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="0e6f7-422">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="0e6f7-423">デバイス カテゴリ</span><span class="sxs-lookup"><span data-stu-id="0e6f7-423">Device category</span></span>|
|<span data-ttu-id="0e6f7-424">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="0e6f7-424">windowsProtectionState</span></span>|[<span data-ttu-id="0e6f7-425">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="0e6f7-425">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="0e6f7-426">デバイス保護の状態。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-426">The device protection status.</span></span>|
|<span data-ttu-id="0e6f7-427">users</span><span class="sxs-lookup"><span data-stu-id="0e6f7-427">users</span></span>|<span data-ttu-id="0e6f7-428">[user](../resources/intune-shared-user.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0e6f7-428">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="0e6f7-429">管理対象デバイスに関連付けられているプライマリユーザー。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-429">The primary users associated with the managed device.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0e6f7-430">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0e6f7-430">JSON Representation</span></span>
<span data-ttu-id="0e6f7-431">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0e6f7-431">Here is a JSON representation of the resource.</span></span>
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





