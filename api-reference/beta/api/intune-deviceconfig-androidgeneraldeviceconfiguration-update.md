---
title: Update androidGeneralDeviceConfiguration
description: androidGeneralDeviceConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 175546ec4f91067605b8af05eb517563c1f4897e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887704"
---
# <a name="update-androidgeneraldeviceconfiguration"></a><span data-ttu-id="df4ad-103">Update androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="df4ad-103">Update androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="df4ad-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="df4ad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df4ad-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df4ad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df4ad-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="df4ad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df4ad-107">[androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-107">Update the properties of a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="df4ad-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="df4ad-108">Prerequisites</span></span>
<span data-ttu-id="df4ad-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="df4ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df4ad-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="df4ad-111">Permission type</span></span>|<span data-ttu-id="df4ad-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="df4ad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df4ad-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="df4ad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="df4ad-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df4ad-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="df4ad-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="df4ad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df4ad-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df4ad-116">Not supported.</span></span>|
|<span data-ttu-id="df4ad-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="df4ad-117">Application</span></span>|<span data-ttu-id="df4ad-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df4ad-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df4ad-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="df4ad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="df4ad-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="df4ad-120">Request headers</span></span>
|<span data-ttu-id="df4ad-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="df4ad-121">Header</span></span>|<span data-ttu-id="df4ad-122">値</span><span class="sxs-lookup"><span data-stu-id="df4ad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df4ad-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="df4ad-123">Authorization</span></span>|<span data-ttu-id="df4ad-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="df4ad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df4ad-125">Accept</span><span class="sxs-lookup"><span data-stu-id="df4ad-125">Accept</span></span>|<span data-ttu-id="df4ad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df4ad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df4ad-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="df4ad-127">Request body</span></span>
<span data-ttu-id="df4ad-128">要求本文で、[androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-128">In the request body, supply a JSON representation for the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="df4ad-129">次の表に、[androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-129">The following table shows the properties that are required when you create the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="df4ad-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="df4ad-130">Property</span></span>|<span data-ttu-id="df4ad-131">種類</span><span class="sxs-lookup"><span data-stu-id="df4ad-131">Type</span></span>|<span data-ttu-id="df4ad-132">説明</span><span class="sxs-lookup"><span data-stu-id="df4ad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df4ad-133">ID</span><span class="sxs-lookup"><span data-stu-id="df4ad-133">id</span></span>|<span data-ttu-id="df4ad-134">String</span><span class="sxs-lookup"><span data-stu-id="df4ad-134">String</span></span>|<span data-ttu-id="df4ad-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="df4ad-135">Key of the entity.</span></span> <span data-ttu-id="df4ad-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df4ad-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df4ad-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="df4ad-137">lastModifiedDateTime</span></span>|<span data-ttu-id="df4ad-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df4ad-138">DateTimeOffset</span></span>|<span data-ttu-id="df4ad-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="df4ad-139">DateTime the object was last modified.</span></span> <span data-ttu-id="df4ad-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df4ad-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df4ad-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="df4ad-141">roleScopeTagIds</span></span>|<span data-ttu-id="df4ad-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="df4ad-142">String collection</span></span>|<span data-ttu-id="df4ad-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="df4ad-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="df4ad-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df4ad-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df4ad-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="df4ad-145">supportsScopeTags</span></span>|<span data-ttu-id="df4ad-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="df4ad-146">Boolean</span></span>|<span data-ttu-id="df4ad-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="df4ad-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="df4ad-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="df4ad-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="df4ad-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="df4ad-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="df4ad-150">This property is read-only.</span></span> <span data-ttu-id="df4ad-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df4ad-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df4ad-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="df4ad-152">createdDateTime</span></span>|<span data-ttu-id="df4ad-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df4ad-153">DateTimeOffset</span></span>|<span data-ttu-id="df4ad-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="df4ad-154">DateTime the object was created.</span></span> <span data-ttu-id="df4ad-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df4ad-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df4ad-156">説明</span><span class="sxs-lookup"><span data-stu-id="df4ad-156">description</span></span>|<span data-ttu-id="df4ad-157">String</span><span class="sxs-lookup"><span data-stu-id="df4ad-157">String</span></span>|<span data-ttu-id="df4ad-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="df4ad-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="df4ad-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df4ad-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df4ad-160">displayName</span><span class="sxs-lookup"><span data-stu-id="df4ad-160">displayName</span></span>|<span data-ttu-id="df4ad-161">String</span><span class="sxs-lookup"><span data-stu-id="df4ad-161">String</span></span>|<span data-ttu-id="df4ad-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="df4ad-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="df4ad-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df4ad-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df4ad-164">version</span><span class="sxs-lookup"><span data-stu-id="df4ad-164">version</span></span>|<span data-ttu-id="df4ad-165">Int32</span><span class="sxs-lookup"><span data-stu-id="df4ad-165">Int32</span></span>|<span data-ttu-id="df4ad-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="df4ad-166">Version of the device configuration.</span></span> <span data-ttu-id="df4ad-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df4ad-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df4ad-168">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="df4ad-168">appsBlockClipboardSharing</span></span>|<span data-ttu-id="df4ad-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-169">Boolean</span></span>|<span data-ttu-id="df4ad-170">アプリケーション間でコピー/貼り付けを行うためのクリップボードの共有をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-170">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="df4ad-171">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="df4ad-171">appsBlockCopyPaste</span></span>|<span data-ttu-id="df4ad-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-172">Boolean</span></span>|<span data-ttu-id="df4ad-173">アプリケーション内でのコピー/貼り付けをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-173">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="df4ad-174">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="df4ad-174">appsBlockYouTube</span></span>|<span data-ttu-id="df4ad-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-175">Boolean</span></span>|<span data-ttu-id="df4ad-176">YouTube アプリをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-176">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="df4ad-177">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="df4ad-177">bluetoothBlocked</span></span>|<span data-ttu-id="df4ad-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-178">Boolean</span></span>|<span data-ttu-id="df4ad-179">Bluetooth をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-179">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="df4ad-180">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="df4ad-180">cameraBlocked</span></span>|<span data-ttu-id="df4ad-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-181">Boolean</span></span>|<span data-ttu-id="df4ad-182">カメラの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-182">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="df4ad-183">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="df4ad-183">cellularBlockDataRoaming</span></span>|<span data-ttu-id="df4ad-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-184">Boolean</span></span>|<span data-ttu-id="df4ad-185">データ ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-185">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="df4ad-186">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="df4ad-186">cellularBlockMessaging</span></span>|<span data-ttu-id="df4ad-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-187">Boolean</span></span>|<span data-ttu-id="df4ad-188">SMS/MMS メッセージングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-188">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="df4ad-189">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="df4ad-189">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="df4ad-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-190">Boolean</span></span>|<span data-ttu-id="df4ad-191">音声通話ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-191">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="df4ad-192">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="df4ad-192">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="df4ad-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-193">Boolean</span></span>|<span data-ttu-id="df4ad-194">Wi-Fi テザリングの同期をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-194">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="df4ad-195">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="df4ad-195">compliantAppsList</span></span>|<span data-ttu-id="df4ad-196">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="df4ad-196">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="df4ad-197">コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。</span><span class="sxs-lookup"><span data-stu-id="df4ad-197">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="df4ad-198">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="df4ad-198">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="df4ad-199">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="df4ad-199">compliantAppListType</span></span>|[<span data-ttu-id="df4ad-200">appListType</span><span class="sxs-lookup"><span data-stu-id="df4ad-200">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="df4ad-201">CompliantAppsList 内にあるリストの種類。</span><span class="sxs-lookup"><span data-stu-id="df4ad-201">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="df4ad-202">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="df4ad-202">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="df4ad-203">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="df4ad-203">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="df4ad-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-204">Boolean</span></span>|<span data-ttu-id="df4ad-205">診断データの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-205">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="df4ad-206">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="df4ad-206">locationServicesBlocked</span></span>|<span data-ttu-id="df4ad-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-207">Boolean</span></span>|<span data-ttu-id="df4ad-208">位置情報サービスをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-208">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="df4ad-209">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="df4ad-209">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="df4ad-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-210">Boolean</span></span>|<span data-ttu-id="df4ad-211">Google アカウントの自動同期をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-211">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="df4ad-212">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="df4ad-212">googlePlayStoreBlocked</span></span>|<span data-ttu-id="df4ad-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-213">Boolean</span></span>|<span data-ttu-id="df4ad-214">Google Play ストアをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-214">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="df4ad-215">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="df4ad-215">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="df4ad-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-216">Boolean</span></span>|<span data-ttu-id="df4ad-217">キオスク モード中に画面スリープ ボタンをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-217">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="df4ad-218">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="df4ad-218">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="df4ad-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-219">Boolean</span></span>|<span data-ttu-id="df4ad-220">キオスク モード中にボリューム ボタンをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-220">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="df4ad-221">dateAndTimeBlockChanges</span><span class="sxs-lookup"><span data-stu-id="df4ad-221">dateAndTimeBlockChanges</span></span>|<span data-ttu-id="df4ad-222">ブール型</span><span class="sxs-lookup"><span data-stu-id="df4ad-222">Boolean</span></span>|<span data-ttu-id="df4ad-223">日付や連盟ノックス ・ モードでの時間の変更をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-223">Indicates whether or not to block changing date and time while in KNOX Mode.</span></span>|
|<span data-ttu-id="df4ad-224">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="df4ad-224">kioskModeApps</span></span>|<span data-ttu-id="df4ad-225">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="df4ad-225">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="df4ad-226">デバイスがキオスク モードのときに実行できるアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="df4ad-226">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="df4ad-227">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="df4ad-227">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="df4ad-228">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="df4ad-228">nfcBlocked</span></span>|<span data-ttu-id="df4ad-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-229">Boolean</span></span>|<span data-ttu-id="df4ad-230">近距離無線通信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-230">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="df4ad-231">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="df4ad-231">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="df4ad-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-232">Boolean</span></span>|<span data-ttu-id="df4ad-233">指紋によるロック解除を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-233">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="df4ad-234">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="df4ad-234">passwordBlockTrustAgents</span></span>|<span data-ttu-id="df4ad-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-235">Boolean</span></span>|<span data-ttu-id="df4ad-236">Smart Lock や他の信頼エージェントをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-236">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="df4ad-237">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="df4ad-237">passwordExpirationDays</span></span>|<span data-ttu-id="df4ad-238">Int32</span><span class="sxs-lookup"><span data-stu-id="df4ad-238">Int32</span></span>|<span data-ttu-id="df4ad-239">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="df4ad-239">Number of days before the password expires.</span></span> <span data-ttu-id="df4ad-240">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="df4ad-240">Valid values 1 to 365</span></span>|
|<span data-ttu-id="df4ad-241">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="df4ad-241">passwordMinimumLength</span></span>|<span data-ttu-id="df4ad-242">Int32</span><span class="sxs-lookup"><span data-stu-id="df4ad-242">Int32</span></span>|<span data-ttu-id="df4ad-243">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="df4ad-243">Minimum length of passwords.</span></span> <span data-ttu-id="df4ad-244">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="df4ad-244">Valid values 4 to 16</span></span>|
|<span data-ttu-id="df4ad-245">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="df4ad-245">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="df4ad-246">Int32</span><span class="sxs-lookup"><span data-stu-id="df4ad-246">Int32</span></span>|<span data-ttu-id="df4ad-247">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="df4ad-247">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="df4ad-248">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="df4ad-248">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="df4ad-249">Int32</span><span class="sxs-lookup"><span data-stu-id="df4ad-249">Int32</span></span>|<span data-ttu-id="df4ad-250">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="df4ad-250">Number of previous passwords to block.</span></span> <span data-ttu-id="df4ad-251">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="df4ad-251">Valid values 0 to 24</span></span>|
|<span data-ttu-id="df4ad-252">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="df4ad-252">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="df4ad-253">Int32</span><span class="sxs-lookup"><span data-stu-id="df4ad-253">Int32</span></span>|<span data-ttu-id="df4ad-254">出荷時の設定にリセットされるまでの、失敗が許可されるサインインの回数。</span><span class="sxs-lookup"><span data-stu-id="df4ad-254">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="df4ad-255">有効な値は 4 から 11 までです</span><span class="sxs-lookup"><span data-stu-id="df4ad-255">Valid values 4 to 11</span></span>|
|<span data-ttu-id="df4ad-256">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="df4ad-256">passwordRequiredType</span></span>|[<span data-ttu-id="df4ad-257">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="df4ad-257">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="df4ad-258">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="df4ad-258">Type of password that is required.</span></span> <span data-ttu-id="df4ad-259">可能な値は、`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any` です。</span><span class="sxs-lookup"><span data-stu-id="df4ad-259">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="df4ad-260">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="df4ad-260">passwordRequired</span></span>|<span data-ttu-id="df4ad-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-261">Boolean</span></span>|<span data-ttu-id="df4ad-262">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-262">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="df4ad-263">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="df4ad-263">powerOffBlocked</span></span>|<span data-ttu-id="df4ad-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-264">Boolean</span></span>|<span data-ttu-id="df4ad-265">デバイスの電源オフをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-265">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="df4ad-266">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="df4ad-266">factoryResetBlocked</span></span>|<span data-ttu-id="df4ad-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-267">Boolean</span></span>|<span data-ttu-id="df4ad-268">ユーザーが出荷時の設定にリセットできないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-268">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="df4ad-269">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="df4ad-269">screenCaptureBlocked</span></span>|<span data-ttu-id="df4ad-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-270">Boolean</span></span>|<span data-ttu-id="df4ad-271">スクリーンショットを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-271">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="df4ad-272">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="df4ad-272">deviceSharingAllowed</span></span>|<span data-ttu-id="df4ad-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-273">Boolean</span></span>|<span data-ttu-id="df4ad-274">デバイスの共有モードを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-274">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="df4ad-275">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="df4ad-275">storageBlockGoogleBackup</span></span>|<span data-ttu-id="df4ad-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-276">Boolean</span></span>|<span data-ttu-id="df4ad-277">Google バックアップを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-277">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="df4ad-278">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="df4ad-278">storageBlockRemovableStorage</span></span>|<span data-ttu-id="df4ad-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-279">Boolean</span></span>|<span data-ttu-id="df4ad-280">リムーバブル記憶域の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-280">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="df4ad-281">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="df4ad-281">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="df4ad-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-282">Boolean</span></span>|<span data-ttu-id="df4ad-283">デバイスの暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-283">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="df4ad-284">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="df4ad-284">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="df4ad-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-285">Boolean</span></span>|<span data-ttu-id="df4ad-286">リムーバブル記憶域の暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-286">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="df4ad-287">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="df4ad-287">voiceAssistantBlocked</span></span>|<span data-ttu-id="df4ad-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-288">Boolean</span></span>|<span data-ttu-id="df4ad-289">音声アシスタントの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-289">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="df4ad-290">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="df4ad-290">voiceDialingBlocked</span></span>|<span data-ttu-id="df4ad-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-291">Boolean</span></span>|<span data-ttu-id="df4ad-292">音声ダイヤルをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-292">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="df4ad-293">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="df4ad-293">webBrowserBlockPopups</span></span>|<span data-ttu-id="df4ad-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-294">Boolean</span></span>|<span data-ttu-id="df4ad-295">Web ブラウザー内のポップアップをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-295">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="df4ad-296">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="df4ad-296">webBrowserBlockAutofill</span></span>|<span data-ttu-id="df4ad-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-297">Boolean</span></span>|<span data-ttu-id="df4ad-298">Web ブラウザーの自動塗りつぶし機能をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-298">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="df4ad-299">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="df4ad-299">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="df4ad-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-300">Boolean</span></span>|<span data-ttu-id="df4ad-301">Web ブラウザー内の JavaScript をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-301">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="df4ad-302">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="df4ad-302">webBrowserBlocked</span></span>|<span data-ttu-id="df4ad-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-303">Boolean</span></span>|<span data-ttu-id="df4ad-304">Web ブラウザーをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-304">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="df4ad-305">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="df4ad-305">webBrowserCookieSettings</span></span>|[<span data-ttu-id="df4ad-306">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="df4ad-306">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="df4ad-307">Web ブラウザー内の Cookie の設定。</span><span class="sxs-lookup"><span data-stu-id="df4ad-307">Cookie settings within the web browser.</span></span> <span data-ttu-id="df4ad-308">可能な値は、`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways` です。</span><span class="sxs-lookup"><span data-stu-id="df4ad-308">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="df4ad-309">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="df4ad-309">wiFiBlocked</span></span>|<span data-ttu-id="df4ad-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-310">Boolean</span></span>|<span data-ttu-id="df4ad-311">Wi-Fi の同期をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-311">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="df4ad-312">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="df4ad-312">appsInstallAllowList</span></span>|<span data-ttu-id="df4ad-313">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="df4ad-313">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="df4ad-314">KNOX デバイス上にインストールできるアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="df4ad-314">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="df4ad-315">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="df4ad-315">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="df4ad-316">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="df4ad-316">appsLaunchBlockList</span></span>|<span data-ttu-id="df4ad-317">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="df4ad-317">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="df4ad-318">KNOX デバイス上での起動がブロックされているアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="df4ad-318">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="df4ad-319">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="df4ad-319">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="df4ad-320">appsHideList</span><span class="sxs-lookup"><span data-stu-id="df4ad-320">appsHideList</span></span>|<span data-ttu-id="df4ad-321">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="df4ad-321">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="df4ad-322">KNOX デバイス上で非表示にするアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="df4ad-322">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="df4ad-323">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="df4ad-323">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="df4ad-324">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="df4ad-324">securityRequireVerifyApps</span></span>|<span data-ttu-id="df4ad-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="df4ad-325">Boolean</span></span>|<span data-ttu-id="df4ad-326">Android の検証アプリ機能をオンにするよう要求します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-326">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="df4ad-327">応答</span><span class="sxs-lookup"><span data-stu-id="df4ad-327">Response</span></span>
<span data-ttu-id="df4ad-328">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="df4ad-328">If successful, this method returns a `200 OK` response code and an updated [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df4ad-329">例</span><span class="sxs-lookup"><span data-stu-id="df4ad-329">Example</span></span>
### <a name="request"></a><span data-ttu-id="df4ad-330">要求</span><span class="sxs-lookup"><span data-stu-id="df4ad-330">Request</span></span>
<span data-ttu-id="df4ad-331">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="df4ad-331">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3153

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="df4ad-332">応答</span><span class="sxs-lookup"><span data-stu-id="df4ad-332">Response</span></span>
<span data-ttu-id="df4ad-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="df4ad-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





