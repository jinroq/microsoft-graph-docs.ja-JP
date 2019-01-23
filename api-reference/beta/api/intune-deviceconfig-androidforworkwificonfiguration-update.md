---
title: AndroidForWorkWiFiConfiguration を更新します。
description: AndroidForWorkWiFiConfiguration オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 50716b9e8dfc3a7e4952244afe87e28d310906c5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413130"
---
# <a name="update-androidforworkwificonfiguration"></a><span data-ttu-id="2ab33-103">AndroidForWorkWiFiConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="2ab33-103">Update androidForWorkWiFiConfiguration</span></span>

> <span data-ttu-id="2ab33-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2ab33-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2ab33-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ab33-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2ab33-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2ab33-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ab33-107">[AndroidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2ab33-107">Update the properties of a [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ab33-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="2ab33-108">Prerequisites</span></span>
<span data-ttu-id="2ab33-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2ab33-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2ab33-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2ab33-111">Permission type</span></span>|<span data-ttu-id="2ab33-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2ab33-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ab33-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2ab33-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2ab33-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ab33-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2ab33-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2ab33-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ab33-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ab33-116">Not supported.</span></span>|
|<span data-ttu-id="2ab33-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2ab33-117">Application</span></span>|<span data-ttu-id="2ab33-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ab33-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ab33-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2ab33-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2ab33-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2ab33-120">Request headers</span></span>
|<span data-ttu-id="2ab33-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2ab33-121">Header</span></span>|<span data-ttu-id="2ab33-122">値</span><span class="sxs-lookup"><span data-stu-id="2ab33-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ab33-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ab33-123">Authorization</span></span>|<span data-ttu-id="2ab33-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="2ab33-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ab33-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2ab33-125">Accept</span></span>|<span data-ttu-id="2ab33-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2ab33-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ab33-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="2ab33-127">Request body</span></span>
<span data-ttu-id="2ab33-128">要求の本文に[androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="2ab33-128">In the request body, supply a JSON representation for the [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>

<span data-ttu-id="2ab33-129">[AndroidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="2ab33-129">The following table shows the properties that are required when you create the [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span></span>

|<span data-ttu-id="2ab33-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ab33-130">Property</span></span>|<span data-ttu-id="2ab33-131">型</span><span class="sxs-lookup"><span data-stu-id="2ab33-131">Type</span></span>|<span data-ttu-id="2ab33-132">説明</span><span class="sxs-lookup"><span data-stu-id="2ab33-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ab33-133">id</span><span class="sxs-lookup"><span data-stu-id="2ab33-133">id</span></span>|<span data-ttu-id="2ab33-134">String</span><span class="sxs-lookup"><span data-stu-id="2ab33-134">String</span></span>|<span data-ttu-id="2ab33-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2ab33-135">Key of the entity.</span></span> <span data-ttu-id="2ab33-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ab33-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ab33-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ab33-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2ab33-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ab33-138">DateTimeOffset</span></span>|<span data-ttu-id="2ab33-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="2ab33-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2ab33-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ab33-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ab33-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2ab33-141">roleScopeTagIds</span></span>|<span data-ttu-id="2ab33-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="2ab33-142">String collection</span></span>|<span data-ttu-id="2ab33-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="2ab33-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2ab33-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ab33-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ab33-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2ab33-145">supportsScopeTags</span></span>|<span data-ttu-id="2ab33-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ab33-146">Boolean</span></span>|<span data-ttu-id="2ab33-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2ab33-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2ab33-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="2ab33-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2ab33-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="2ab33-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2ab33-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="2ab33-150">This property is read-only.</span></span> <span data-ttu-id="2ab33-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ab33-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ab33-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2ab33-152">createdDateTime</span></span>|<span data-ttu-id="2ab33-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ab33-153">DateTimeOffset</span></span>|<span data-ttu-id="2ab33-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="2ab33-154">DateTime the object was created.</span></span> <span data-ttu-id="2ab33-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ab33-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ab33-156">説明</span><span class="sxs-lookup"><span data-stu-id="2ab33-156">description</span></span>|<span data-ttu-id="2ab33-157">String</span><span class="sxs-lookup"><span data-stu-id="2ab33-157">String</span></span>|<span data-ttu-id="2ab33-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="2ab33-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2ab33-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ab33-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ab33-160">displayName</span><span class="sxs-lookup"><span data-stu-id="2ab33-160">displayName</span></span>|<span data-ttu-id="2ab33-161">String</span><span class="sxs-lookup"><span data-stu-id="2ab33-161">String</span></span>|<span data-ttu-id="2ab33-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="2ab33-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2ab33-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ab33-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ab33-164">version</span><span class="sxs-lookup"><span data-stu-id="2ab33-164">version</span></span>|<span data-ttu-id="2ab33-165">Int32</span><span class="sxs-lookup"><span data-stu-id="2ab33-165">Int32</span></span>|<span data-ttu-id="2ab33-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="2ab33-166">Version of the device configuration.</span></span> <span data-ttu-id="2ab33-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ab33-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ab33-168">ネットワーク名リソース</span><span class="sxs-lookup"><span data-stu-id="2ab33-168">networkName</span></span>|<span data-ttu-id="2ab33-169">String</span><span class="sxs-lookup"><span data-stu-id="2ab33-169">String</span></span>|<span data-ttu-id="2ab33-170">ネットワーク名</span><span class="sxs-lookup"><span data-stu-id="2ab33-170">Network Name</span></span>|
|<span data-ttu-id="2ab33-171">ssid</span><span class="sxs-lookup"><span data-stu-id="2ab33-171">ssid</span></span>|<span data-ttu-id="2ab33-172">String</span><span class="sxs-lookup"><span data-stu-id="2ab33-172">String</span></span>|<span data-ttu-id="2ab33-173">これは、すべてのデバイスにブロードキャストされている Wi-fi ネットワークの名前です。</span><span class="sxs-lookup"><span data-stu-id="2ab33-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="2ab33-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="2ab33-174">connectAutomatically</span></span>|<span data-ttu-id="2ab33-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ab33-175">Boolean</span></span>|<span data-ttu-id="2ab33-176">このネットワークが範囲内にすると自動的に接続します。</span><span class="sxs-lookup"><span data-stu-id="2ab33-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="2ab33-177">これを true に設定、ユーザー プロンプトを省略して自動的に Wi-fi ネットワークにデバイスを接続します。</span><span class="sxs-lookup"><span data-stu-id="2ab33-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="2ab33-178">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="2ab33-178">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="2ab33-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ab33-179">Boolean</span></span>|<span data-ttu-id="2ab33-180">True の場合、このプロファイルに設定されているすべてのデバイスに SSID をブロードキャストしていないネットワークに接続するデバイスを強制します。</span><span class="sxs-lookup"><span data-stu-id="2ab33-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="2ab33-181">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="2ab33-181">wiFiSecurityType</span></span>|[<span data-ttu-id="2ab33-182">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="2ab33-182">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="2ab33-183">Wi-fi エンドポイントがベースの EAP セキュリティ タイプを使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2ab33-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="2ab33-184">使用可能な値は、`open`、`wpaEnterprise` です。</span><span class="sxs-lookup"><span data-stu-id="2ab33-184">Possible values are: `open`, `wpaEnterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="2ab33-185">応答</span><span class="sxs-lookup"><span data-stu-id="2ab33-185">Response</span></span>
<span data-ttu-id="2ab33-186">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="2ab33-186">If successful, this method returns a `200 OK` response code and an updated [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ab33-187">例</span><span class="sxs-lookup"><span data-stu-id="2ab33-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ab33-188">要求</span><span class="sxs-lookup"><span data-stu-id="2ab33-188">Request</span></span>
<span data-ttu-id="2ab33-189">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2ab33-189">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 442

{
  "@odata.type": "#microsoft.graph.androidForWorkWiFiConfiguration",
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
  "wiFiSecurityType": "wpaEnterprise"
}
```

### <a name="response"></a><span data-ttu-id="2ab33-190">応答</span><span class="sxs-lookup"><span data-stu-id="2ab33-190">Response</span></span>
<span data-ttu-id="2ab33-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2ab33-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 614

{
  "@odata.type": "#microsoft.graph.androidForWorkWiFiConfiguration",
  "id": "58bcfe05-fe05-58bc-05fe-bc5805febc58",
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
  "wiFiSecurityType": "wpaEnterprise"
}
```




