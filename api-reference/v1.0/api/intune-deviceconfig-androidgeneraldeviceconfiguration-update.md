---
title: Update androidGeneralDeviceConfiguration
description: androidGeneralDeviceConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c68c13fa95221bca7c284dcc58a2bd1d69f3ff55
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553233"
---
# <a name="update-androidgeneraldeviceconfiguration"></a><span data-ttu-id="cb4c3-103">Update androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="cb4c3-103">Update androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="cb4c3-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb4c3-105">[androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-105">Update the properties of a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb4c3-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="cb4c3-106">Prerequisites</span></span>
<span data-ttu-id="cb4c3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb4c3-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cb4c3-109">Permission type</span></span>|<span data-ttu-id="cb4c3-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cb4c3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb4c3-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cb4c3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cb4c3-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb4c3-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cb4c3-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cb4c3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb4c3-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-114">Not supported.</span></span>|
|<span data-ttu-id="cb4c3-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cb4c3-115">Application</span></span>|<span data-ttu-id="cb4c3-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb4c3-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cb4c3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="cb4c3-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cb4c3-118">Request headers</span></span>
|<span data-ttu-id="cb4c3-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cb4c3-119">Header</span></span>|<span data-ttu-id="cb4c3-120">値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb4c3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb4c3-121">Authorization</span></span>|<span data-ttu-id="cb4c3-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb4c3-123">承諾</span><span class="sxs-lookup"><span data-stu-id="cb4c3-123">Accept</span></span>|<span data-ttu-id="cb4c3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cb4c3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb4c3-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="cb4c3-125">Request body</span></span>
<span data-ttu-id="cb4c3-126">要求本文で、[androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-126">In the request body, supply a JSON representation for the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="cb4c3-127">次の表に、[androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-127">The following table shows the properties that are required when you create the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="cb4c3-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb4c3-128">Property</span></span>|<span data-ttu-id="cb4c3-129">型</span><span class="sxs-lookup"><span data-stu-id="cb4c3-129">Type</span></span>|<span data-ttu-id="cb4c3-130">説明</span><span class="sxs-lookup"><span data-stu-id="cb4c3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb4c3-131">id</span><span class="sxs-lookup"><span data-stu-id="cb4c3-131">id</span></span>|<span data-ttu-id="cb4c3-132">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="cb4c3-132">String</span></span>|<span data-ttu-id="cb4c3-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-133">Key of the entity.</span></span> <span data-ttu-id="cb4c3-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cb4c3-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb4c3-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb4c3-135">lastModifiedDateTime</span></span>|<span data-ttu-id="cb4c3-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb4c3-136">DateTimeOffset</span></span>|<span data-ttu-id="cb4c3-137">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-137">DateTime the object was last modified.</span></span> <span data-ttu-id="cb4c3-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cb4c3-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb4c3-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cb4c3-139">createdDateTime</span></span>|<span data-ttu-id="cb4c3-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb4c3-140">DateTimeOffset</span></span>|<span data-ttu-id="cb4c3-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-141">DateTime the object was created.</span></span> <span data-ttu-id="cb4c3-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cb4c3-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb4c3-143">description</span><span class="sxs-lookup"><span data-stu-id="cb4c3-143">description</span></span>|<span data-ttu-id="cb4c3-144">String</span><span class="sxs-lookup"><span data-stu-id="cb4c3-144">String</span></span>|<span data-ttu-id="cb4c3-145">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cb4c3-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cb4c3-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb4c3-147">displayName</span><span class="sxs-lookup"><span data-stu-id="cb4c3-147">displayName</span></span>|<span data-ttu-id="cb4c3-148">String</span><span class="sxs-lookup"><span data-stu-id="cb4c3-148">String</span></span>|<span data-ttu-id="cb4c3-149">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cb4c3-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cb4c3-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb4c3-151">version</span><span class="sxs-lookup"><span data-stu-id="cb4c3-151">version</span></span>|<span data-ttu-id="cb4c3-152">Int32</span><span class="sxs-lookup"><span data-stu-id="cb4c3-152">Int32</span></span>|<span data-ttu-id="cb4c3-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-153">Version of the device configuration.</span></span> <span data-ttu-id="cb4c3-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cb4c3-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb4c3-155">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="cb4c3-155">appsBlockClipboardSharing</span></span>|<span data-ttu-id="cb4c3-156">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-156">Boolean</span></span>|<span data-ttu-id="cb4c3-157">アプリケーション間でコピー/貼り付けを行うためのクリップボードの共有をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-157">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="cb4c3-158">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="cb4c3-158">appsBlockCopyPaste</span></span>|<span data-ttu-id="cb4c3-159">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-159">Boolean</span></span>|<span data-ttu-id="cb4c3-160">アプリケーション内でのコピー/貼り付けをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-160">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="cb4c3-161">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="cb4c3-161">appsBlockYouTube</span></span>|<span data-ttu-id="cb4c3-162">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-162">Boolean</span></span>|<span data-ttu-id="cb4c3-163">YouTube アプリをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-163">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="cb4c3-164">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="cb4c3-164">bluetoothBlocked</span></span>|<span data-ttu-id="cb4c3-165">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-165">Boolean</span></span>|<span data-ttu-id="cb4c3-166">Bluetooth をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-166">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="cb4c3-167">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="cb4c3-167">cameraBlocked</span></span>|<span data-ttu-id="cb4c3-168">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-168">Boolean</span></span>|<span data-ttu-id="cb4c3-169">カメラの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-169">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="cb4c3-170">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="cb4c3-170">cellularBlockDataRoaming</span></span>|<span data-ttu-id="cb4c3-171">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-171">Boolean</span></span>|<span data-ttu-id="cb4c3-172">データ ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-172">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="cb4c3-173">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="cb4c3-173">cellularBlockMessaging</span></span>|<span data-ttu-id="cb4c3-174">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-174">Boolean</span></span>|<span data-ttu-id="cb4c3-175">SMS/MMS メッセージングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-175">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="cb4c3-176">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="cb4c3-176">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="cb4c3-177">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-177">Boolean</span></span>|<span data-ttu-id="cb4c3-178">音声通話ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-178">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="cb4c3-179">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="cb4c3-179">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="cb4c3-180">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-180">Boolean</span></span>|<span data-ttu-id="cb4c3-181">Wi-Fi テザリングの同期をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-181">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="cb4c3-182">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="cb4c3-182">compliantAppsList</span></span>|<span data-ttu-id="cb4c3-183">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cb4c3-183">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="cb4c3-184">コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-184">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="cb4c3-185">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-185">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="cb4c3-186">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="cb4c3-186">compliantAppListType</span></span>|[<span data-ttu-id="cb4c3-187">アプライアンスの種類</span><span class="sxs-lookup"><span data-stu-id="cb4c3-187">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="cb4c3-188">CompliantAppsList 内にあるリストの種類。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-188">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="cb4c3-189">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-189">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="cb4c3-190">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="cb4c3-190">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="cb4c3-191">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-191">Boolean</span></span>|<span data-ttu-id="cb4c3-192">診断データの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-192">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="cb4c3-193">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="cb4c3-193">locationServicesBlocked</span></span>|<span data-ttu-id="cb4c3-194">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-194">Boolean</span></span>|<span data-ttu-id="cb4c3-195">位置情報サービスをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-195">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="cb4c3-196">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="cb4c3-196">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="cb4c3-197">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-197">Boolean</span></span>|<span data-ttu-id="cb4c3-198">Google アカウントの自動同期をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-198">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="cb4c3-199">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="cb4c3-199">googlePlayStoreBlocked</span></span>|<span data-ttu-id="cb4c3-200">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-200">Boolean</span></span>|<span data-ttu-id="cb4c3-201">Google Play ストアをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-201">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="cb4c3-202">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="cb4c3-202">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="cb4c3-203">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-203">Boolean</span></span>|<span data-ttu-id="cb4c3-204">キオスク モード中に画面スリープ ボタンをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-204">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="cb4c3-205">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="cb4c3-205">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="cb4c3-206">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-206">Boolean</span></span>|<span data-ttu-id="cb4c3-207">キオスク モード中にボリューム ボタンをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-207">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="cb4c3-208">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="cb4c3-208">kioskModeApps</span></span>|<span data-ttu-id="cb4c3-209">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cb4c3-209">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="cb4c3-210">デバイスがキオスク モードのときに実行できるアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-210">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="cb4c3-211">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-211">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="cb4c3-212">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="cb4c3-212">nfcBlocked</span></span>|<span data-ttu-id="cb4c3-213">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-213">Boolean</span></span>|<span data-ttu-id="cb4c3-214">近距離無線通信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-214">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="cb4c3-215">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="cb4c3-215">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="cb4c3-216">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-216">Boolean</span></span>|<span data-ttu-id="cb4c3-217">指紋によるロック解除を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-217">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="cb4c3-218">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="cb4c3-218">passwordBlockTrustAgents</span></span>|<span data-ttu-id="cb4c3-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb4c3-219">Boolean</span></span>|<span data-ttu-id="cb4c3-220">Smart Lock や他の信頼エージェントをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-220">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="cb4c3-221">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="cb4c3-221">passwordExpirationDays</span></span>|<span data-ttu-id="cb4c3-222">Int32</span><span class="sxs-lookup"><span data-stu-id="cb4c3-222">Int32</span></span>|<span data-ttu-id="cb4c3-223">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-223">Number of days before the password expires.</span></span> <span data-ttu-id="cb4c3-224">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="cb4c3-224">Valid values 1 to 365</span></span>|
|<span data-ttu-id="cb4c3-225">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="cb4c3-225">passwordMinimumLength</span></span>|<span data-ttu-id="cb4c3-226">Int32</span><span class="sxs-lookup"><span data-stu-id="cb4c3-226">Int32</span></span>|<span data-ttu-id="cb4c3-227">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-227">Minimum length of passwords.</span></span> <span data-ttu-id="cb4c3-228">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="cb4c3-228">Valid values 4 to 16</span></span>|
|<span data-ttu-id="cb4c3-229">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="cb4c3-229">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="cb4c3-230">Int32</span><span class="sxs-lookup"><span data-stu-id="cb4c3-230">Int32</span></span>|<span data-ttu-id="cb4c3-231">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-231">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="cb4c3-232">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="cb4c3-232">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="cb4c3-233">Int32</span><span class="sxs-lookup"><span data-stu-id="cb4c3-233">Int32</span></span>|<span data-ttu-id="cb4c3-234">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-234">Number of previous passwords to block.</span></span> <span data-ttu-id="cb4c3-235">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="cb4c3-235">Valid values 0 to 24</span></span>|
|<span data-ttu-id="cb4c3-236">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="cb4c3-236">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="cb4c3-237">Int32</span><span class="sxs-lookup"><span data-stu-id="cb4c3-237">Int32</span></span>|<span data-ttu-id="cb4c3-238">出荷時の設定にリセットされるまでの、失敗が許可されるサインインの回数。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-238">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="cb4c3-239">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="cb4c3-239">Valid values 1 to 16</span></span>|
|<span data-ttu-id="cb4c3-240">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="cb4c3-240">passwordRequiredType</span></span>|[<span data-ttu-id="cb4c3-241">androidrequiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="cb4c3-241">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="cb4c3-242">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-242">Type of password that is required.</span></span> <span data-ttu-id="cb4c3-243">可能な値は、`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any` です。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-243">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="cb4c3-244">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="cb4c3-244">passwordRequired</span></span>|<span data-ttu-id="cb4c3-245">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-245">Boolean</span></span>|<span data-ttu-id="cb4c3-246">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-246">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="cb4c3-247">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="cb4c3-247">powerOffBlocked</span></span>|<span data-ttu-id="cb4c3-248">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-248">Boolean</span></span>|<span data-ttu-id="cb4c3-249">デバイスの電源オフをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-249">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="cb4c3-250">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="cb4c3-250">factoryResetBlocked</span></span>|<span data-ttu-id="cb4c3-251">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-251">Boolean</span></span>|<span data-ttu-id="cb4c3-252">ユーザーが出荷時の設定にリセットできないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-252">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="cb4c3-253">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="cb4c3-253">screenCaptureBlocked</span></span>|<span data-ttu-id="cb4c3-254">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-254">Boolean</span></span>|<span data-ttu-id="cb4c3-255">スクリーンショットを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-255">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="cb4c3-256">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="cb4c3-256">deviceSharingAllowed</span></span>|<span data-ttu-id="cb4c3-257">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-257">Boolean</span></span>|<span data-ttu-id="cb4c3-258">デバイスの共有モードを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-258">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="cb4c3-259">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="cb4c3-259">storageBlockGoogleBackup</span></span>|<span data-ttu-id="cb4c3-260">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-260">Boolean</span></span>|<span data-ttu-id="cb4c3-261">Google バックアップを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-261">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="cb4c3-262">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="cb4c3-262">storageBlockRemovableStorage</span></span>|<span data-ttu-id="cb4c3-263">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-263">Boolean</span></span>|<span data-ttu-id="cb4c3-264">リムーバブル記憶域の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-264">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="cb4c3-265">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="cb4c3-265">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="cb4c3-266">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-266">Boolean</span></span>|<span data-ttu-id="cb4c3-267">デバイスの暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-267">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="cb4c3-268">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="cb4c3-268">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="cb4c3-269">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-269">Boolean</span></span>|<span data-ttu-id="cb4c3-270">リムーバブル記憶域の暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-270">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="cb4c3-271">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="cb4c3-271">voiceAssistantBlocked</span></span>|<span data-ttu-id="cb4c3-272">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-272">Boolean</span></span>|<span data-ttu-id="cb4c3-273">音声アシスタントの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-273">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="cb4c3-274">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="cb4c3-274">voiceDialingBlocked</span></span>|<span data-ttu-id="cb4c3-275">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-275">Boolean</span></span>|<span data-ttu-id="cb4c3-276">音声ダイヤルをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-276">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="cb4c3-277">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="cb4c3-277">webBrowserBlockPopups</span></span>|<span data-ttu-id="cb4c3-278">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-278">Boolean</span></span>|<span data-ttu-id="cb4c3-279">Web ブラウザー内のポップアップをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-279">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="cb4c3-280">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="cb4c3-280">webBrowserBlockAutofill</span></span>|<span data-ttu-id="cb4c3-281">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-281">Boolean</span></span>|<span data-ttu-id="cb4c3-282">Web ブラウザーの自動塗りつぶし機能をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-282">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="cb4c3-283">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="cb4c3-283">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="cb4c3-284">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-284">Boolean</span></span>|<span data-ttu-id="cb4c3-285">Web ブラウザー内の JavaScript をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-285">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="cb4c3-286">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="cb4c3-286">webBrowserBlocked</span></span>|<span data-ttu-id="cb4c3-287">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-287">Boolean</span></span>|<span data-ttu-id="cb4c3-288">Web ブラウザーをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-288">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="cb4c3-289">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="cb4c3-289">webBrowserCookieSettings</span></span>|[<span data-ttu-id="cb4c3-290">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="cb4c3-290">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="cb4c3-291">Web ブラウザー内の Cookie の設定。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-291">Cookie settings within the web browser.</span></span> <span data-ttu-id="cb4c3-292">可能な値は、`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways` です。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-292">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="cb4c3-293">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="cb4c3-293">wiFiBlocked</span></span>|<span data-ttu-id="cb4c3-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb4c3-294">Boolean</span></span>|<span data-ttu-id="cb4c3-295">Wi-Fi の同期をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-295">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="cb4c3-296">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="cb4c3-296">appsInstallAllowList</span></span>|<span data-ttu-id="cb4c3-297">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cb4c3-297">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="cb4c3-298">KNOX デバイス上にインストールできるアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-298">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="cb4c3-299">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-299">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="cb4c3-300">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="cb4c3-300">appsLaunchBlockList</span></span>|<span data-ttu-id="cb4c3-301">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cb4c3-301">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="cb4c3-302">KNOX デバイス上での起動がブロックされているアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-302">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="cb4c3-303">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-303">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="cb4c3-304">appsHideList</span><span class="sxs-lookup"><span data-stu-id="cb4c3-304">appsHideList</span></span>|<span data-ttu-id="cb4c3-305">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cb4c3-305">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="cb4c3-306">KNOX デバイス上で非表示にするアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-306">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="cb4c3-307">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-307">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="cb4c3-308">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="cb4c3-308">securityRequireVerifyApps</span></span>|<span data-ttu-id="cb4c3-309">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb4c3-309">Boolean</span></span>|<span data-ttu-id="cb4c3-310">Android の検証アプリ機能をオンにするよう要求します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-310">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="cb4c3-311">応答</span><span class="sxs-lookup"><span data-stu-id="cb4c3-311">Response</span></span>
<span data-ttu-id="cb4c3-312">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-312">If successful, this method returns a `200 OK` response code and an updated [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb4c3-313">例</span><span class="sxs-lookup"><span data-stu-id="cb4c3-313">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb4c3-314">要求</span><span class="sxs-lookup"><span data-stu-id="cb4c3-314">Request</span></span>
<span data-ttu-id="cb4c3-315">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-315">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3033

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "appsBlockClipboardSharing": true,
  "appsBlockCopyPaste": true,
  "appsBlockYouTube": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockMessaging": true,
  "cellularBlockVoiceRoaming": true,
  "cellularBlockWiFiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphabetic",
  "passwordRequired": true,
  "powerOffBlocked": true,
  "factoryResetBlocked": true,
  "screenCaptureBlocked": true,
  "deviceSharingAllowed": true,
  "storageBlockGoogleBackup": true,
  "storageBlockRemovableStorage": true,
  "storageRequireDeviceEncryption": true,
  "storageRequireRemovableStorageEncryption": true,
  "voiceAssistantBlocked": true,
  "voiceDialingBlocked": true,
  "webBrowserBlockPopups": true,
  "webBrowserBlockAutofill": true,
  "webBrowserBlockJavaScript": true,
  "webBrowserBlocked": true,
  "webBrowserCookieSettings": "blockAlways",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a><span data-ttu-id="cb4c3-316">応答</span><span class="sxs-lookup"><span data-stu-id="cb4c3-316">Response</span></span>
<span data-ttu-id="cb4c3-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cb4c3-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3205

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "appsBlockClipboardSharing": true,
  "appsBlockCopyPaste": true,
  "appsBlockYouTube": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockMessaging": true,
  "cellularBlockVoiceRoaming": true,
  "cellularBlockWiFiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphabetic",
  "passwordRequired": true,
  "powerOffBlocked": true,
  "factoryResetBlocked": true,
  "screenCaptureBlocked": true,
  "deviceSharingAllowed": true,
  "storageBlockGoogleBackup": true,
  "storageBlockRemovableStorage": true,
  "storageRequireDeviceEncryption": true,
  "storageRequireRemovableStorageEncryption": true,
  "voiceAssistantBlocked": true,
  "voiceDialingBlocked": true,
  "webBrowserBlockPopups": true,
  "webBrowserBlockAutofill": true,
  "webBrowserBlockJavaScript": true,
  "webBrowserBlocked": true,
  "webBrowserCookieSettings": "blockAlways",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "securityRequireVerifyApps": true
}
```



