---
title: Create androidGeneralDeviceConfiguration
description: 新しい androidGeneralDeviceConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0ea439b593f1e0e8d26cf43450a104806140634f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31796788"
---
# <a name="create-androidgeneraldeviceconfiguration"></a><span data-ttu-id="8da47-103">Create androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="8da47-103">Create androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="8da47-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8da47-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8da47-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8da47-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8da47-106">新しい [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8da47-106">Create a new [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8da47-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8da47-107">Prerequisites</span></span>
<span data-ttu-id="8da47-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8da47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8da47-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8da47-110">Permission type</span></span>|<span data-ttu-id="8da47-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8da47-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8da47-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8da47-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8da47-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8da47-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8da47-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8da47-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8da47-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8da47-115">Not supported.</span></span>|
|<span data-ttu-id="8da47-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8da47-116">Application</span></span>|<span data-ttu-id="8da47-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8da47-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8da47-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8da47-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8da47-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8da47-119">Request headers</span></span>
|<span data-ttu-id="8da47-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8da47-120">Header</span></span>|<span data-ttu-id="8da47-121">値</span><span class="sxs-lookup"><span data-stu-id="8da47-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8da47-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8da47-122">Authorization</span></span>|<span data-ttu-id="8da47-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8da47-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8da47-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8da47-124">Accept</span></span>|<span data-ttu-id="8da47-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8da47-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8da47-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8da47-126">Request body</span></span>
<span data-ttu-id="8da47-127">要求本文で、androidGeneralDeviceConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8da47-127">In the request body, supply a JSON representation for the androidGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="8da47-128">次の表に、androidGeneralDeviceConfiguration 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-128">The following table shows the properties that are required when you create the androidGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="8da47-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8da47-129">Property</span></span>|<span data-ttu-id="8da47-130">型</span><span class="sxs-lookup"><span data-stu-id="8da47-130">Type</span></span>|<span data-ttu-id="8da47-131">説明</span><span class="sxs-lookup"><span data-stu-id="8da47-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8da47-132">id</span><span class="sxs-lookup"><span data-stu-id="8da47-132">id</span></span>|<span data-ttu-id="8da47-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="8da47-133">String</span></span>|<span data-ttu-id="8da47-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8da47-134">Key of the entity.</span></span> <span data-ttu-id="8da47-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8da47-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8da47-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8da47-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8da47-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8da47-137">DateTimeOffset</span></span>|<span data-ttu-id="8da47-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="8da47-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8da47-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8da47-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8da47-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8da47-140">roleScopeTagIds</span></span>|<span data-ttu-id="8da47-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="8da47-141">String collection</span></span>|<span data-ttu-id="8da47-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="8da47-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8da47-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8da47-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8da47-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8da47-144">supportsScopeTags</span></span>|<span data-ttu-id="8da47-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-145">Boolean</span></span>|<span data-ttu-id="8da47-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8da47-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="8da47-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8da47-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="8da47-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8da47-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="8da47-149">This property is read-only.</span></span> <span data-ttu-id="8da47-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8da47-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8da47-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8da47-151">createdDateTime</span></span>|<span data-ttu-id="8da47-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8da47-152">DateTimeOffset</span></span>|<span data-ttu-id="8da47-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="8da47-153">DateTime the object was created.</span></span> <span data-ttu-id="8da47-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8da47-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8da47-155">説明</span><span class="sxs-lookup"><span data-stu-id="8da47-155">description</span></span>|<span data-ttu-id="8da47-156">String</span><span class="sxs-lookup"><span data-stu-id="8da47-156">String</span></span>|<span data-ttu-id="8da47-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="8da47-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8da47-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8da47-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8da47-159">displayName</span><span class="sxs-lookup"><span data-stu-id="8da47-159">displayName</span></span>|<span data-ttu-id="8da47-160">String</span><span class="sxs-lookup"><span data-stu-id="8da47-160">String</span></span>|<span data-ttu-id="8da47-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="8da47-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8da47-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8da47-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8da47-163">version</span><span class="sxs-lookup"><span data-stu-id="8da47-163">version</span></span>|<span data-ttu-id="8da47-164">Int32</span><span class="sxs-lookup"><span data-stu-id="8da47-164">Int32</span></span>|<span data-ttu-id="8da47-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="8da47-165">Version of the device configuration.</span></span> <span data-ttu-id="8da47-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8da47-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8da47-167">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="8da47-167">appsBlockClipboardSharing</span></span>|<span data-ttu-id="8da47-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-168">Boolean</span></span>|<span data-ttu-id="8da47-169">アプリケーション間でコピー/貼り付けを行うためのクリップボードの共有をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-169">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="8da47-170">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="8da47-170">appsBlockCopyPaste</span></span>|<span data-ttu-id="8da47-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-171">Boolean</span></span>|<span data-ttu-id="8da47-172">アプリケーション内でのコピー/貼り付けをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-172">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="8da47-173">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="8da47-173">appsBlockYouTube</span></span>|<span data-ttu-id="8da47-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-174">Boolean</span></span>|<span data-ttu-id="8da47-175">YouTube アプリをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-175">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="8da47-176">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="8da47-176">bluetoothBlocked</span></span>|<span data-ttu-id="8da47-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-177">Boolean</span></span>|<span data-ttu-id="8da47-178">Bluetooth をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-178">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="8da47-179">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="8da47-179">cameraBlocked</span></span>|<span data-ttu-id="8da47-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-180">Boolean</span></span>|<span data-ttu-id="8da47-181">カメラの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-181">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="8da47-182">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="8da47-182">cellularBlockDataRoaming</span></span>|<span data-ttu-id="8da47-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-183">Boolean</span></span>|<span data-ttu-id="8da47-184">データ ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-184">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="8da47-185">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="8da47-185">cellularBlockMessaging</span></span>|<span data-ttu-id="8da47-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-186">Boolean</span></span>|<span data-ttu-id="8da47-187">SMS/MMS メッセージングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-187">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="8da47-188">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="8da47-188">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="8da47-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-189">Boolean</span></span>|<span data-ttu-id="8da47-190">音声通話ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-190">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="8da47-191">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="8da47-191">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="8da47-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-192">Boolean</span></span>|<span data-ttu-id="8da47-193">Wi-Fi テザリングの同期をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-193">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="8da47-194">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="8da47-194">compliantAppsList</span></span>|<span data-ttu-id="8da47-195">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8da47-195">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="8da47-196">コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。</span><span class="sxs-lookup"><span data-stu-id="8da47-196">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="8da47-197">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="8da47-197">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="8da47-198">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="8da47-198">compliantAppListType</span></span>|[<span data-ttu-id="8da47-199">アプライアンスの種類</span><span class="sxs-lookup"><span data-stu-id="8da47-199">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="8da47-200">CompliantAppsList 内にあるリストの種類。</span><span class="sxs-lookup"><span data-stu-id="8da47-200">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="8da47-201">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="8da47-201">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="8da47-202">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="8da47-202">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="8da47-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-203">Boolean</span></span>|<span data-ttu-id="8da47-204">診断データの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-204">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="8da47-205">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="8da47-205">locationServicesBlocked</span></span>|<span data-ttu-id="8da47-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-206">Boolean</span></span>|<span data-ttu-id="8da47-207">位置情報サービスをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-207">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="8da47-208">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="8da47-208">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="8da47-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-209">Boolean</span></span>|<span data-ttu-id="8da47-210">Google アカウントの自動同期をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-210">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="8da47-211">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="8da47-211">googlePlayStoreBlocked</span></span>|<span data-ttu-id="8da47-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-212">Boolean</span></span>|<span data-ttu-id="8da47-213">Google Play ストアをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-213">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="8da47-214">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="8da47-214">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="8da47-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-215">Boolean</span></span>|<span data-ttu-id="8da47-216">キオスク モード中に画面スリープ ボタンをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-216">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="8da47-217">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="8da47-217">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="8da47-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-218">Boolean</span></span>|<span data-ttu-id="8da47-219">キオスク モード中にボリューム ボタンをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-219">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="8da47-220">dateandtimeblockchanges</span><span class="sxs-lookup"><span data-stu-id="8da47-220">dateAndTimeBlockChanges</span></span>|<span data-ttu-id="8da47-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-221">Boolean</span></span>|<span data-ttu-id="8da47-222">KNOX モードの間に日付と時刻の変更を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-222">Indicates whether or not to block changing date and time while in KNOX Mode.</span></span>|
|<span data-ttu-id="8da47-223">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="8da47-223">kioskModeApps</span></span>|<span data-ttu-id="8da47-224">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8da47-224">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="8da47-225">デバイスがキオスク モードのときに実行できるアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="8da47-225">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="8da47-226">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="8da47-226">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8da47-227">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="8da47-227">nfcBlocked</span></span>|<span data-ttu-id="8da47-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-228">Boolean</span></span>|<span data-ttu-id="8da47-229">近距離無線通信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-229">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="8da47-230">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="8da47-230">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="8da47-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-231">Boolean</span></span>|<span data-ttu-id="8da47-232">指紋によるロック解除を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-232">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="8da47-233">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="8da47-233">passwordBlockTrustAgents</span></span>|<span data-ttu-id="8da47-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-234">Boolean</span></span>|<span data-ttu-id="8da47-235">Smart Lock や他の信頼エージェントをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-235">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="8da47-236">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8da47-236">passwordExpirationDays</span></span>|<span data-ttu-id="8da47-237">Int32</span><span class="sxs-lookup"><span data-stu-id="8da47-237">Int32</span></span>|<span data-ttu-id="8da47-238">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="8da47-238">Number of days before the password expires.</span></span> <span data-ttu-id="8da47-239">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="8da47-239">Valid values 1 to 365</span></span>|
|<span data-ttu-id="8da47-240">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8da47-240">passwordMinimumLength</span></span>|<span data-ttu-id="8da47-241">Int32</span><span class="sxs-lookup"><span data-stu-id="8da47-241">Int32</span></span>|<span data-ttu-id="8da47-242">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="8da47-242">Minimum length of passwords.</span></span> <span data-ttu-id="8da47-243">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="8da47-243">Valid values 4 to 16</span></span>|
|<span data-ttu-id="8da47-244">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="8da47-244">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="8da47-245">Int32</span><span class="sxs-lookup"><span data-stu-id="8da47-245">Int32</span></span>|<span data-ttu-id="8da47-246">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="8da47-246">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="8da47-247">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="8da47-247">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="8da47-248">Int32</span><span class="sxs-lookup"><span data-stu-id="8da47-248">Int32</span></span>|<span data-ttu-id="8da47-249">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="8da47-249">Number of previous passwords to block.</span></span> <span data-ttu-id="8da47-250">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="8da47-250">Valid values 0 to 24</span></span>|
|<span data-ttu-id="8da47-251">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="8da47-251">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="8da47-252">Int32</span><span class="sxs-lookup"><span data-stu-id="8da47-252">Int32</span></span>|<span data-ttu-id="8da47-253">出荷時の設定にリセットされるまでの、失敗が許可されるサインインの回数。</span><span class="sxs-lookup"><span data-stu-id="8da47-253">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="8da47-254">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="8da47-254">Valid values 1 to 16</span></span>|
|<span data-ttu-id="8da47-255">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="8da47-255">passwordRequiredType</span></span>|[<span data-ttu-id="8da47-256">androidrequiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="8da47-256">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="8da47-257">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="8da47-257">Type of password that is required.</span></span> <span data-ttu-id="8da47-258">可能な値は、`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any` です。</span><span class="sxs-lookup"><span data-stu-id="8da47-258">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="8da47-259">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="8da47-259">passwordRequired</span></span>|<span data-ttu-id="8da47-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-260">Boolean</span></span>|<span data-ttu-id="8da47-261">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8da47-261">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="8da47-262">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="8da47-262">powerOffBlocked</span></span>|<span data-ttu-id="8da47-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-263">Boolean</span></span>|<span data-ttu-id="8da47-264">デバイスの電源オフをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-264">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="8da47-265">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="8da47-265">factoryResetBlocked</span></span>|<span data-ttu-id="8da47-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-266">Boolean</span></span>|<span data-ttu-id="8da47-267">ユーザーが出荷時の設定にリセットできないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-267">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="8da47-268">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="8da47-268">screenCaptureBlocked</span></span>|<span data-ttu-id="8da47-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-269">Boolean</span></span>|<span data-ttu-id="8da47-270">スクリーンショットを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-270">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="8da47-271">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="8da47-271">deviceSharingAllowed</span></span>|<span data-ttu-id="8da47-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-272">Boolean</span></span>|<span data-ttu-id="8da47-273">デバイスの共有モードを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-273">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="8da47-274">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="8da47-274">storageBlockGoogleBackup</span></span>|<span data-ttu-id="8da47-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-275">Boolean</span></span>|<span data-ttu-id="8da47-276">Google バックアップを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-276">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="8da47-277">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="8da47-277">storageBlockRemovableStorage</span></span>|<span data-ttu-id="8da47-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-278">Boolean</span></span>|<span data-ttu-id="8da47-279">リムーバブル記憶域の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-279">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="8da47-280">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="8da47-280">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="8da47-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-281">Boolean</span></span>|<span data-ttu-id="8da47-282">デバイスの暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-282">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="8da47-283">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="8da47-283">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="8da47-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-284">Boolean</span></span>|<span data-ttu-id="8da47-285">リムーバブル記憶域の暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-285">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="8da47-286">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="8da47-286">voiceAssistantBlocked</span></span>|<span data-ttu-id="8da47-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-287">Boolean</span></span>|<span data-ttu-id="8da47-288">音声アシスタントの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-288">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="8da47-289">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="8da47-289">voiceDialingBlocked</span></span>|<span data-ttu-id="8da47-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-290">Boolean</span></span>|<span data-ttu-id="8da47-291">音声ダイヤルをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-291">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="8da47-292">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="8da47-292">webBrowserBlockPopups</span></span>|<span data-ttu-id="8da47-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-293">Boolean</span></span>|<span data-ttu-id="8da47-294">Web ブラウザー内のポップアップをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-294">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="8da47-295">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="8da47-295">webBrowserBlockAutofill</span></span>|<span data-ttu-id="8da47-296">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-296">Boolean</span></span>|<span data-ttu-id="8da47-297">Web ブラウザーの自動塗りつぶし機能をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-297">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="8da47-298">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="8da47-298">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="8da47-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-299">Boolean</span></span>|<span data-ttu-id="8da47-300">Web ブラウザー内の JavaScript をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-300">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="8da47-301">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="8da47-301">webBrowserBlocked</span></span>|<span data-ttu-id="8da47-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-302">Boolean</span></span>|<span data-ttu-id="8da47-303">Web ブラウザーをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-303">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="8da47-304">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="8da47-304">webBrowserCookieSettings</span></span>|[<span data-ttu-id="8da47-305">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="8da47-305">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="8da47-306">Web ブラウザー内の Cookie の設定。</span><span class="sxs-lookup"><span data-stu-id="8da47-306">Cookie settings within the web browser.</span></span> <span data-ttu-id="8da47-307">可能な値は、`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways` です。</span><span class="sxs-lookup"><span data-stu-id="8da47-307">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="8da47-308">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="8da47-308">wiFiBlocked</span></span>|<span data-ttu-id="8da47-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-309">Boolean</span></span>|<span data-ttu-id="8da47-310">Wi-Fi の同期をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8da47-310">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="8da47-311">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="8da47-311">appsInstallAllowList</span></span>|<span data-ttu-id="8da47-312">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8da47-312">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="8da47-313">KNOX デバイス上にインストールできるアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="8da47-313">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="8da47-314">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="8da47-314">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8da47-315">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="8da47-315">appsLaunchBlockList</span></span>|<span data-ttu-id="8da47-316">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8da47-316">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="8da47-317">KNOX デバイス上での起動がブロックされているアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="8da47-317">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="8da47-318">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="8da47-318">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8da47-319">appsHideList</span><span class="sxs-lookup"><span data-stu-id="8da47-319">appsHideList</span></span>|<span data-ttu-id="8da47-320">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8da47-320">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="8da47-321">KNOX デバイス上で非表示にするアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="8da47-321">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="8da47-322">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="8da47-322">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8da47-323">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="8da47-323">securityRequireVerifyApps</span></span>|<span data-ttu-id="8da47-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="8da47-324">Boolean</span></span>|<span data-ttu-id="8da47-325">Android の検証アプリ機能をオンにするよう要求します。</span><span class="sxs-lookup"><span data-stu-id="8da47-325">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="8da47-326">応答</span><span class="sxs-lookup"><span data-stu-id="8da47-326">Response</span></span>
<span data-ttu-id="8da47-327">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8da47-327">If successful, this method returns a `201 Created` response code and a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8da47-328">例</span><span class="sxs-lookup"><span data-stu-id="8da47-328">Example</span></span>

### <a name="request"></a><span data-ttu-id="8da47-329">要求</span><span class="sxs-lookup"><span data-stu-id="8da47-329">Request</span></span>
<span data-ttu-id="8da47-330">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8da47-330">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3161

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "dateAndTimeBlockChanges": true,
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

### <a name="response"></a><span data-ttu-id="8da47-331">応答</span><span class="sxs-lookup"><span data-stu-id="8da47-331">Response</span></span>
<span data-ttu-id="8da47-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8da47-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3333

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "dateAndTimeBlockChanges": true,
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





