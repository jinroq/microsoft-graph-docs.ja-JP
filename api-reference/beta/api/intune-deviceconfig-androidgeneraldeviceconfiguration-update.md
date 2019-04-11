---
title: Update androidGeneralDeviceConfiguration
description: androidGeneralDeviceConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 511712cb44216f1efbdf0d9154dbf8ed970ee0e0
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31774919"
---
# <a name="update-androidgeneraldeviceconfiguration"></a><span data-ttu-id="e0e62-103">Update androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0e62-103">Update androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="e0e62-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0e62-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0e62-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e0e62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0e62-106">[androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-106">Update the properties of a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0e62-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e0e62-107">Prerequisites</span></span>
<span data-ttu-id="e0e62-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e0e62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0e62-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e0e62-110">Permission type</span></span>|<span data-ttu-id="e0e62-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e0e62-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0e62-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e0e62-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e0e62-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0e62-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e0e62-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e0e62-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0e62-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0e62-115">Not supported.</span></span>|
|<span data-ttu-id="e0e62-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e0e62-116">Application</span></span>|<span data-ttu-id="e0e62-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0e62-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0e62-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e0e62-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e0e62-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e0e62-119">Request headers</span></span>
|<span data-ttu-id="e0e62-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e0e62-120">Header</span></span>|<span data-ttu-id="e0e62-121">値</span><span class="sxs-lookup"><span data-stu-id="e0e62-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0e62-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0e62-122">Authorization</span></span>|<span data-ttu-id="e0e62-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e0e62-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0e62-124">承諾</span><span class="sxs-lookup"><span data-stu-id="e0e62-124">Accept</span></span>|<span data-ttu-id="e0e62-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e0e62-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0e62-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e0e62-126">Request body</span></span>
<span data-ttu-id="e0e62-127">要求本文で、[androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-127">In the request body, supply a JSON representation for the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="e0e62-128">次の表に、[androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-128">The following table shows the properties that are required when you create the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="e0e62-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e0e62-129">Property</span></span>|<span data-ttu-id="e0e62-130">型</span><span class="sxs-lookup"><span data-stu-id="e0e62-130">Type</span></span>|<span data-ttu-id="e0e62-131">説明</span><span class="sxs-lookup"><span data-stu-id="e0e62-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0e62-132">id</span><span class="sxs-lookup"><span data-stu-id="e0e62-132">id</span></span>|<span data-ttu-id="e0e62-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e0e62-133">String</span></span>|<span data-ttu-id="e0e62-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e0e62-134">Key of the entity.</span></span> <span data-ttu-id="e0e62-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e0e62-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0e62-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0e62-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e0e62-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0e62-137">DateTimeOffset</span></span>|<span data-ttu-id="e0e62-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="e0e62-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e0e62-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e0e62-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0e62-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e0e62-140">roleScopeTagIds</span></span>|<span data-ttu-id="e0e62-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="e0e62-141">String collection</span></span>|<span data-ttu-id="e0e62-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="e0e62-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e0e62-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e0e62-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0e62-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e0e62-144">supportsScopeTags</span></span>|<span data-ttu-id="e0e62-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-145">Boolean</span></span>|<span data-ttu-id="e0e62-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e0e62-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="e0e62-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e0e62-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="e0e62-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e0e62-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-149">This property is read-only.</span></span> <span data-ttu-id="e0e62-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e0e62-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0e62-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e0e62-151">createdDateTime</span></span>|<span data-ttu-id="e0e62-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0e62-152">DateTimeOffset</span></span>|<span data-ttu-id="e0e62-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e0e62-153">DateTime the object was created.</span></span> <span data-ttu-id="e0e62-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e0e62-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0e62-155">説明</span><span class="sxs-lookup"><span data-stu-id="e0e62-155">description</span></span>|<span data-ttu-id="e0e62-156">String</span><span class="sxs-lookup"><span data-stu-id="e0e62-156">String</span></span>|<span data-ttu-id="e0e62-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="e0e62-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e0e62-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e0e62-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0e62-159">displayName</span><span class="sxs-lookup"><span data-stu-id="e0e62-159">displayName</span></span>|<span data-ttu-id="e0e62-160">String</span><span class="sxs-lookup"><span data-stu-id="e0e62-160">String</span></span>|<span data-ttu-id="e0e62-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="e0e62-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e0e62-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e0e62-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0e62-163">version</span><span class="sxs-lookup"><span data-stu-id="e0e62-163">version</span></span>|<span data-ttu-id="e0e62-164">Int32</span><span class="sxs-lookup"><span data-stu-id="e0e62-164">Int32</span></span>|<span data-ttu-id="e0e62-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="e0e62-165">Version of the device configuration.</span></span> <span data-ttu-id="e0e62-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e0e62-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0e62-167">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="e0e62-167">appsBlockClipboardSharing</span></span>|<span data-ttu-id="e0e62-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-168">Boolean</span></span>|<span data-ttu-id="e0e62-169">アプリケーション間でコピー/貼り付けを行うためのクリップボードの共有をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-169">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="e0e62-170">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="e0e62-170">appsBlockCopyPaste</span></span>|<span data-ttu-id="e0e62-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-171">Boolean</span></span>|<span data-ttu-id="e0e62-172">アプリケーション内でのコピー/貼り付けをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-172">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="e0e62-173">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="e0e62-173">appsBlockYouTube</span></span>|<span data-ttu-id="e0e62-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-174">Boolean</span></span>|<span data-ttu-id="e0e62-175">YouTube アプリをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-175">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="e0e62-176">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="e0e62-176">bluetoothBlocked</span></span>|<span data-ttu-id="e0e62-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-177">Boolean</span></span>|<span data-ttu-id="e0e62-178">Bluetooth をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-178">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="e0e62-179">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="e0e62-179">cameraBlocked</span></span>|<span data-ttu-id="e0e62-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-180">Boolean</span></span>|<span data-ttu-id="e0e62-181">カメラの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-181">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="e0e62-182">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="e0e62-182">cellularBlockDataRoaming</span></span>|<span data-ttu-id="e0e62-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-183">Boolean</span></span>|<span data-ttu-id="e0e62-184">データ ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-184">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="e0e62-185">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="e0e62-185">cellularBlockMessaging</span></span>|<span data-ttu-id="e0e62-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-186">Boolean</span></span>|<span data-ttu-id="e0e62-187">SMS/MMS メッセージングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-187">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="e0e62-188">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="e0e62-188">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="e0e62-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-189">Boolean</span></span>|<span data-ttu-id="e0e62-190">音声通話ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-190">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="e0e62-191">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="e0e62-191">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="e0e62-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-192">Boolean</span></span>|<span data-ttu-id="e0e62-193">Wi-Fi テザリングの同期をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-193">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="e0e62-194">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="e0e62-194">compliantAppsList</span></span>|<span data-ttu-id="e0e62-195">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e0e62-195">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="e0e62-196">コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。</span><span class="sxs-lookup"><span data-stu-id="e0e62-196">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="e0e62-197">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e0e62-197">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="e0e62-198">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="e0e62-198">compliantAppListType</span></span>|[<span data-ttu-id="e0e62-199">アプライアンスの種類</span><span class="sxs-lookup"><span data-stu-id="e0e62-199">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="e0e62-200">CompliantAppsList 内にあるリストの種類。</span><span class="sxs-lookup"><span data-stu-id="e0e62-200">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="e0e62-201">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="e0e62-201">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="e0e62-202">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="e0e62-202">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="e0e62-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-203">Boolean</span></span>|<span data-ttu-id="e0e62-204">診断データの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-204">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="e0e62-205">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="e0e62-205">locationServicesBlocked</span></span>|<span data-ttu-id="e0e62-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-206">Boolean</span></span>|<span data-ttu-id="e0e62-207">位置情報サービスをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-207">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="e0e62-208">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="e0e62-208">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="e0e62-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-209">Boolean</span></span>|<span data-ttu-id="e0e62-210">Google アカウントの自動同期をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-210">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="e0e62-211">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="e0e62-211">googlePlayStoreBlocked</span></span>|<span data-ttu-id="e0e62-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-212">Boolean</span></span>|<span data-ttu-id="e0e62-213">Google Play ストアをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-213">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="e0e62-214">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="e0e62-214">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="e0e62-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-215">Boolean</span></span>|<span data-ttu-id="e0e62-216">キオスク モード中に画面スリープ ボタンをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-216">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="e0e62-217">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="e0e62-217">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="e0e62-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-218">Boolean</span></span>|<span data-ttu-id="e0e62-219">キオスク モード中にボリューム ボタンをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-219">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="e0e62-220">dateandtimeblockchanges</span><span class="sxs-lookup"><span data-stu-id="e0e62-220">dateAndTimeBlockChanges</span></span>|<span data-ttu-id="e0e62-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-221">Boolean</span></span>|<span data-ttu-id="e0e62-222">KNOX モードの間に日付と時刻の変更を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-222">Indicates whether or not to block changing date and time while in KNOX Mode.</span></span>|
|<span data-ttu-id="e0e62-223">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="e0e62-223">kioskModeApps</span></span>|<span data-ttu-id="e0e62-224">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e0e62-224">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="e0e62-225">デバイスがキオスク モードのときに実行できるアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="e0e62-225">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="e0e62-226">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e0e62-226">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e0e62-227">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="e0e62-227">nfcBlocked</span></span>|<span data-ttu-id="e0e62-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-228">Boolean</span></span>|<span data-ttu-id="e0e62-229">近距離無線通信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-229">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="e0e62-230">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="e0e62-230">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="e0e62-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-231">Boolean</span></span>|<span data-ttu-id="e0e62-232">指紋によるロック解除を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-232">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="e0e62-233">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="e0e62-233">passwordBlockTrustAgents</span></span>|<span data-ttu-id="e0e62-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-234">Boolean</span></span>|<span data-ttu-id="e0e62-235">Smart Lock や他の信頼エージェントをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-235">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="e0e62-236">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e0e62-236">passwordExpirationDays</span></span>|<span data-ttu-id="e0e62-237">Int32</span><span class="sxs-lookup"><span data-stu-id="e0e62-237">Int32</span></span>|<span data-ttu-id="e0e62-238">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="e0e62-238">Number of days before the password expires.</span></span> <span data-ttu-id="e0e62-239">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="e0e62-239">Valid values 1 to 365</span></span>|
|<span data-ttu-id="e0e62-240">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e0e62-240">passwordMinimumLength</span></span>|<span data-ttu-id="e0e62-241">Int32</span><span class="sxs-lookup"><span data-stu-id="e0e62-241">Int32</span></span>|<span data-ttu-id="e0e62-242">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="e0e62-242">Minimum length of passwords.</span></span> <span data-ttu-id="e0e62-243">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="e0e62-243">Valid values 4 to 16</span></span>|
|<span data-ttu-id="e0e62-244">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="e0e62-244">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="e0e62-245">Int32</span><span class="sxs-lookup"><span data-stu-id="e0e62-245">Int32</span></span>|<span data-ttu-id="e0e62-246">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="e0e62-246">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="e0e62-247">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e0e62-247">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e0e62-248">Int32</span><span class="sxs-lookup"><span data-stu-id="e0e62-248">Int32</span></span>|<span data-ttu-id="e0e62-249">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="e0e62-249">Number of previous passwords to block.</span></span> <span data-ttu-id="e0e62-250">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="e0e62-250">Valid values 0 to 24</span></span>|
|<span data-ttu-id="e0e62-251">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="e0e62-251">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="e0e62-252">Int32</span><span class="sxs-lookup"><span data-stu-id="e0e62-252">Int32</span></span>|<span data-ttu-id="e0e62-253">出荷時の設定にリセットされるまでの、失敗が許可されるサインインの回数。</span><span class="sxs-lookup"><span data-stu-id="e0e62-253">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="e0e62-254">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="e0e62-254">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e0e62-255">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e0e62-255">passwordRequiredType</span></span>|[<span data-ttu-id="e0e62-256">androidrequiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="e0e62-256">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="e0e62-257">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="e0e62-257">Type of password that is required.</span></span> <span data-ttu-id="e0e62-258">可能な値は、`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any` です。</span><span class="sxs-lookup"><span data-stu-id="e0e62-258">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="e0e62-259">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="e0e62-259">passwordRequired</span></span>|<span data-ttu-id="e0e62-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-260">Boolean</span></span>|<span data-ttu-id="e0e62-261">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-261">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="e0e62-262">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="e0e62-262">powerOffBlocked</span></span>|<span data-ttu-id="e0e62-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-263">Boolean</span></span>|<span data-ttu-id="e0e62-264">デバイスの電源オフをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-264">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="e0e62-265">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="e0e62-265">factoryResetBlocked</span></span>|<span data-ttu-id="e0e62-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-266">Boolean</span></span>|<span data-ttu-id="e0e62-267">ユーザーが出荷時の設定にリセットできないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-267">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="e0e62-268">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="e0e62-268">screenCaptureBlocked</span></span>|<span data-ttu-id="e0e62-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-269">Boolean</span></span>|<span data-ttu-id="e0e62-270">スクリーンショットを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-270">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="e0e62-271">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="e0e62-271">deviceSharingAllowed</span></span>|<span data-ttu-id="e0e62-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-272">Boolean</span></span>|<span data-ttu-id="e0e62-273">デバイスの共有モードを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-273">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="e0e62-274">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="e0e62-274">storageBlockGoogleBackup</span></span>|<span data-ttu-id="e0e62-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-275">Boolean</span></span>|<span data-ttu-id="e0e62-276">Google バックアップを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-276">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="e0e62-277">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="e0e62-277">storageBlockRemovableStorage</span></span>|<span data-ttu-id="e0e62-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-278">Boolean</span></span>|<span data-ttu-id="e0e62-279">リムーバブル記憶域の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-279">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="e0e62-280">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="e0e62-280">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="e0e62-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-281">Boolean</span></span>|<span data-ttu-id="e0e62-282">デバイスの暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-282">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="e0e62-283">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="e0e62-283">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="e0e62-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-284">Boolean</span></span>|<span data-ttu-id="e0e62-285">リムーバブル記憶域の暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-285">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="e0e62-286">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="e0e62-286">voiceAssistantBlocked</span></span>|<span data-ttu-id="e0e62-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-287">Boolean</span></span>|<span data-ttu-id="e0e62-288">音声アシスタントの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-288">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="e0e62-289">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="e0e62-289">voiceDialingBlocked</span></span>|<span data-ttu-id="e0e62-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-290">Boolean</span></span>|<span data-ttu-id="e0e62-291">音声ダイヤルをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-291">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="e0e62-292">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="e0e62-292">webBrowserBlockPopups</span></span>|<span data-ttu-id="e0e62-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-293">Boolean</span></span>|<span data-ttu-id="e0e62-294">Web ブラウザー内のポップアップをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-294">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="e0e62-295">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="e0e62-295">webBrowserBlockAutofill</span></span>|<span data-ttu-id="e0e62-296">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-296">Boolean</span></span>|<span data-ttu-id="e0e62-297">Web ブラウザーの自動塗りつぶし機能をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-297">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="e0e62-298">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="e0e62-298">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="e0e62-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-299">Boolean</span></span>|<span data-ttu-id="e0e62-300">Web ブラウザー内の JavaScript をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-300">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="e0e62-301">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="e0e62-301">webBrowserBlocked</span></span>|<span data-ttu-id="e0e62-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-302">Boolean</span></span>|<span data-ttu-id="e0e62-303">Web ブラウザーをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-303">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="e0e62-304">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="e0e62-304">webBrowserCookieSettings</span></span>|[<span data-ttu-id="e0e62-305">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="e0e62-305">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="e0e62-306">Web ブラウザー内の Cookie の設定。</span><span class="sxs-lookup"><span data-stu-id="e0e62-306">Cookie settings within the web browser.</span></span> <span data-ttu-id="e0e62-307">可能な値は、`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways` です。</span><span class="sxs-lookup"><span data-stu-id="e0e62-307">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="e0e62-308">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="e0e62-308">wiFiBlocked</span></span>|<span data-ttu-id="e0e62-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-309">Boolean</span></span>|<span data-ttu-id="e0e62-310">Wi-Fi の同期をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-310">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="e0e62-311">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="e0e62-311">appsInstallAllowList</span></span>|<span data-ttu-id="e0e62-312">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e0e62-312">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="e0e62-313">KNOX デバイス上にインストールできるアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="e0e62-313">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="e0e62-314">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e0e62-314">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e0e62-315">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="e0e62-315">appsLaunchBlockList</span></span>|<span data-ttu-id="e0e62-316">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e0e62-316">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="e0e62-317">KNOX デバイス上での起動がブロックされているアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="e0e62-317">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="e0e62-318">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e0e62-318">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e0e62-319">appsHideList</span><span class="sxs-lookup"><span data-stu-id="e0e62-319">appsHideList</span></span>|<span data-ttu-id="e0e62-320">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e0e62-320">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="e0e62-321">KNOX デバイス上で非表示にするアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="e0e62-321">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="e0e62-322">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e0e62-322">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e0e62-323">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="e0e62-323">securityRequireVerifyApps</span></span>|<span data-ttu-id="e0e62-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0e62-324">Boolean</span></span>|<span data-ttu-id="e0e62-325">Android の検証アプリ機能をオンにするよう要求します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-325">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="e0e62-326">応答</span><span class="sxs-lookup"><span data-stu-id="e0e62-326">Response</span></span>
<span data-ttu-id="e0e62-327">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e0e62-327">If successful, this method returns a `200 OK` response code and an updated [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0e62-328">例</span><span class="sxs-lookup"><span data-stu-id="e0e62-328">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0e62-329">要求</span><span class="sxs-lookup"><span data-stu-id="e0e62-329">Request</span></span>
<span data-ttu-id="e0e62-330">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e0e62-330">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="e0e62-331">応答</span><span class="sxs-lookup"><span data-stu-id="e0e62-331">Response</span></span>
<span data-ttu-id="e0e62-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e0e62-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





