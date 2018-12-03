---
title: AndroidDeviceOwnerWiFiConfiguration を作成します。
description: 新しい androidDeviceOwnerWiFiConfiguration オブジェクトを作成します。
ms.openlocfilehash: 7d2cfc8efca581e5c788df131f69c1fc0db285d9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070621"
---
# <a name="create-androiddeviceownerwificonfiguration"></a><span data-ttu-id="0a4c6-103">AndroidDeviceOwnerWiFiConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-103">Create androidDeviceOwnerWiFiConfiguration</span></span>

> <span data-ttu-id="0a4c6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a4c6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a4c6-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a4c6-107">新しい[androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-107">Create a new [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0a4c6-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="0a4c6-108">Prerequisites</span></span>
<span data-ttu-id="0a4c6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a4c6-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0a4c6-111">Permission type</span></span>|<span data-ttu-id="0a4c6-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0a4c6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a4c6-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0a4c6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0a4c6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a4c6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0a4c6-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0a4c6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a4c6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-116">Not supported.</span></span>|
|<span data-ttu-id="0a4c6-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0a4c6-117">Application</span></span>|<span data-ttu-id="0a4c6-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a4c6-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0a4c6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0a4c6-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a4c6-120">Request headers</span></span>
|<span data-ttu-id="0a4c6-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a4c6-121">Header</span></span>|<span data-ttu-id="0a4c6-122">値</span><span class="sxs-lookup"><span data-stu-id="0a4c6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a4c6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a4c6-123">Authorization</span></span>|<span data-ttu-id="0a4c6-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a4c6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0a4c6-125">Accept</span></span>|<span data-ttu-id="0a4c6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0a4c6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a4c6-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0a4c6-127">Request body</span></span>
<span data-ttu-id="0a4c6-128">要求の本文に androidDeviceOwnerWiFiConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-128">In the request body, supply a JSON representation for the androidDeviceOwnerWiFiConfiguration object.</span></span>

<span data-ttu-id="0a4c6-129">次の表は、androidDeviceOwnerWiFiConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-129">The following table shows the properties that are required when you create the androidDeviceOwnerWiFiConfiguration.</span></span>

|<span data-ttu-id="0a4c6-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a4c6-130">Property</span></span>|<span data-ttu-id="0a4c6-131">型</span><span class="sxs-lookup"><span data-stu-id="0a4c6-131">Type</span></span>|<span data-ttu-id="0a4c6-132">説明</span><span class="sxs-lookup"><span data-stu-id="0a4c6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a4c6-133">id</span><span class="sxs-lookup"><span data-stu-id="0a4c6-133">id</span></span>|<span data-ttu-id="0a4c6-134">String</span><span class="sxs-lookup"><span data-stu-id="0a4c6-134">String</span></span>|<span data-ttu-id="0a4c6-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-135">Key of the entity.</span></span> <span data-ttu-id="0a4c6-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0a4c6-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a4c6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0a4c6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0a4c6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a4c6-138">DateTimeOffset</span></span>|<span data-ttu-id="0a4c6-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0a4c6-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0a4c6-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a4c6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0a4c6-141">roleScopeTagIds</span></span>|<span data-ttu-id="0a4c6-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0a4c6-142">String collection</span></span>|<span data-ttu-id="0a4c6-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0a4c6-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0a4c6-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a4c6-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0a4c6-145">supportsScopeTags</span></span>|<span data-ttu-id="0a4c6-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a4c6-146">Boolean</span></span>|<span data-ttu-id="0a4c6-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0a4c6-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0a4c6-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0a4c6-150">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-150">This property is read-only.</span></span> <span data-ttu-id="0a4c6-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0a4c6-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a4c6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0a4c6-152">createdDateTime</span></span>|<span data-ttu-id="0a4c6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a4c6-153">DateTimeOffset</span></span>|<span data-ttu-id="0a4c6-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-154">DateTime the object was created.</span></span> <span data-ttu-id="0a4c6-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0a4c6-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a4c6-156">説明</span><span class="sxs-lookup"><span data-stu-id="0a4c6-156">description</span></span>|<span data-ttu-id="0a4c6-157">String</span><span class="sxs-lookup"><span data-stu-id="0a4c6-157">String</span></span>|<span data-ttu-id="0a4c6-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0a4c6-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0a4c6-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a4c6-160">displayName</span><span class="sxs-lookup"><span data-stu-id="0a4c6-160">displayName</span></span>|<span data-ttu-id="0a4c6-161">String</span><span class="sxs-lookup"><span data-stu-id="0a4c6-161">String</span></span>|<span data-ttu-id="0a4c6-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0a4c6-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0a4c6-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a4c6-164">version</span><span class="sxs-lookup"><span data-stu-id="0a4c6-164">version</span></span>|<span data-ttu-id="0a4c6-165">Int32</span><span class="sxs-lookup"><span data-stu-id="0a4c6-165">Int32</span></span>|<span data-ttu-id="0a4c6-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-166">Version of the device configuration.</span></span> <span data-ttu-id="0a4c6-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0a4c6-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a4c6-168">ネットワーク名リソース</span><span class="sxs-lookup"><span data-stu-id="0a4c6-168">networkName</span></span>|<span data-ttu-id="0a4c6-169">String</span><span class="sxs-lookup"><span data-stu-id="0a4c6-169">String</span></span>|<span data-ttu-id="0a4c6-170">ネットワーク名</span><span class="sxs-lookup"><span data-stu-id="0a4c6-170">Network Name</span></span>|
|<span data-ttu-id="0a4c6-171">ssid</span><span class="sxs-lookup"><span data-stu-id="0a4c6-171">ssid</span></span>|<span data-ttu-id="0a4c6-172">String</span><span class="sxs-lookup"><span data-stu-id="0a4c6-172">String</span></span>|<span data-ttu-id="0a4c6-173">これは、すべてのデバイスにブロードキャストされている Wi-fi ネットワークの名前です。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="0a4c6-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="0a4c6-174">connectAutomatically</span></span>|<span data-ttu-id="0a4c6-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a4c6-175">Boolean</span></span>|<span data-ttu-id="0a4c6-176">このネットワークが範囲内にすると自動的に接続します。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="0a4c6-177">これを true に設定、ユーザー プロンプトを省略して自動的に Wi-fi ネットワークにデバイスを接続します。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="0a4c6-178">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="0a4c6-178">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="0a4c6-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a4c6-179">Boolean</span></span>|<span data-ttu-id="0a4c6-180">True の場合、このプロファイルに設定されているすべてのデバイスに SSID をブロードキャストしていないネットワークに接続するデバイスを強制します。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="0a4c6-181">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="0a4c6-181">wiFiSecurityType</span></span>|[<span data-ttu-id="0a4c6-182">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="0a4c6-182">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="0a4c6-183">Wi-fi エンドポイントがベースの EAP セキュリティ タイプを使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="0a4c6-184">可能な値は、`open`、`wep`、`wpaPersonal` です。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-184">Possible values are: `open`, `wep`, `wpaPersonal`.</span></span>|
|<span data-ttu-id="0a4c6-185">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="0a4c6-185">preSharedKey</span></span>|<span data-ttu-id="0a4c6-186">String</span><span class="sxs-lookup"><span data-stu-id="0a4c6-186">String</span></span>|<span data-ttu-id="0a4c6-187">これは、WPA パーソナル Wi-fi ネットワークの事前共有キーです。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-187">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="0a4c6-188">preSharedKeyIsSet</span><span class="sxs-lookup"><span data-stu-id="0a4c6-188">preSharedKeyIsSet</span></span>|<span data-ttu-id="0a4c6-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a4c6-189">Boolean</span></span>|<span data-ttu-id="0a4c6-190">これは、WPA パーソナル Wi-fi ネットワークの事前共有キーです。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-190">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="0a4c6-191">応答</span><span class="sxs-lookup"><span data-stu-id="0a4c6-191">Response</span></span>
<span data-ttu-id="0a4c6-192">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-192">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a4c6-193">例</span><span class="sxs-lookup"><span data-stu-id="0a4c6-193">Example</span></span>
### <a name="request"></a><span data-ttu-id="0a4c6-194">要求</span><span class="sxs-lookup"><span data-stu-id="0a4c6-194">Request</span></span>
<span data-ttu-id="0a4c6-195">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-195">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 573

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerWiFiConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wep",
  "preSharedKey": "Pre Shared Key value",
  "preSharedKeyIsSet": true
}
```

### <a name="response"></a><span data-ttu-id="0a4c6-196">応答</span><span class="sxs-lookup"><span data-stu-id="0a4c6-196">Response</span></span>
<span data-ttu-id="0a4c6-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0a4c6-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 681

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerWiFiConfiguration",
  "id": "8d25beba-beba-8d25-babe-258dbabe258d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wep",
  "preSharedKey": "Pre Shared Key value",
  "preSharedKeyIsSet": true
}
```





