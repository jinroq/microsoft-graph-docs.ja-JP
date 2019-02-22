---
title: androidForWorkWiFiConfiguration を作成する
description: 新しい androidForWorkWiFiConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f66b1efd63baec06ca94a88a3d12f77d76190077
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162574"
---
# <a name="create-androidforworkwificonfiguration"></a><span data-ttu-id="44bee-103">androidForWorkWiFiConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="44bee-103">Create androidForWorkWiFiConfiguration</span></span>

> <span data-ttu-id="44bee-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44bee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44bee-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="44bee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44bee-106">新しい[androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="44bee-106">Create a new [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44bee-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="44bee-107">Prerequisites</span></span>
<span data-ttu-id="44bee-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44bee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="44bee-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="44bee-110">Permission type</span></span>|<span data-ttu-id="44bee-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="44bee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44bee-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="44bee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="44bee-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44bee-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="44bee-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="44bee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44bee-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44bee-115">Not supported.</span></span>|
|<span data-ttu-id="44bee-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="44bee-116">Application</span></span>|<span data-ttu-id="44bee-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44bee-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44bee-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="44bee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="44bee-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="44bee-119">Request headers</span></span>
|<span data-ttu-id="44bee-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="44bee-120">Header</span></span>|<span data-ttu-id="44bee-121">値</span><span class="sxs-lookup"><span data-stu-id="44bee-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44bee-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="44bee-122">Authorization</span></span>|<span data-ttu-id="44bee-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="44bee-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44bee-124">承諾</span><span class="sxs-lookup"><span data-stu-id="44bee-124">Accept</span></span>|<span data-ttu-id="44bee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="44bee-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44bee-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="44bee-126">Request body</span></span>
<span data-ttu-id="44bee-127">要求本文で、androidForWorkWiFiConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="44bee-127">In the request body, supply a JSON representation for the androidForWorkWiFiConfiguration object.</span></span>

<span data-ttu-id="44bee-128">次の表に、androidForWorkWiFiConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="44bee-128">The following table shows the properties that are required when you create the androidForWorkWiFiConfiguration.</span></span>

|<span data-ttu-id="44bee-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="44bee-129">Property</span></span>|<span data-ttu-id="44bee-130">型</span><span class="sxs-lookup"><span data-stu-id="44bee-130">Type</span></span>|<span data-ttu-id="44bee-131">説明</span><span class="sxs-lookup"><span data-stu-id="44bee-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44bee-132">id</span><span class="sxs-lookup"><span data-stu-id="44bee-132">id</span></span>|<span data-ttu-id="44bee-133">文字列</span><span class="sxs-lookup"><span data-stu-id="44bee-133">String</span></span>|<span data-ttu-id="44bee-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="44bee-134">Key of the entity.</span></span> <span data-ttu-id="44bee-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="44bee-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44bee-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="44bee-136">lastModifiedDateTime</span></span>|<span data-ttu-id="44bee-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44bee-137">DateTimeOffset</span></span>|<span data-ttu-id="44bee-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="44bee-138">DateTime the object was last modified.</span></span> <span data-ttu-id="44bee-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="44bee-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44bee-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="44bee-140">roleScopeTagIds</span></span>|<span data-ttu-id="44bee-141">String collection</span><span class="sxs-lookup"><span data-stu-id="44bee-141">String collection</span></span>|<span data-ttu-id="44bee-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="44bee-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="44bee-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="44bee-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44bee-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="44bee-144">supportsScopeTags</span></span>|<span data-ttu-id="44bee-145">ブール値</span><span class="sxs-lookup"><span data-stu-id="44bee-145">Boolean</span></span>|<span data-ttu-id="44bee-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="44bee-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="44bee-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="44bee-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="44bee-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="44bee-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="44bee-149">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="44bee-149">This property is read-only.</span></span> <span data-ttu-id="44bee-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="44bee-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44bee-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="44bee-151">createdDateTime</span></span>|<span data-ttu-id="44bee-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44bee-152">DateTimeOffset</span></span>|<span data-ttu-id="44bee-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="44bee-153">DateTime the object was created.</span></span> <span data-ttu-id="44bee-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="44bee-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44bee-155">説明</span><span class="sxs-lookup"><span data-stu-id="44bee-155">description</span></span>|<span data-ttu-id="44bee-156">String</span><span class="sxs-lookup"><span data-stu-id="44bee-156">String</span></span>|<span data-ttu-id="44bee-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="44bee-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="44bee-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="44bee-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44bee-159">displayName</span><span class="sxs-lookup"><span data-stu-id="44bee-159">displayName</span></span>|<span data-ttu-id="44bee-160">String</span><span class="sxs-lookup"><span data-stu-id="44bee-160">String</span></span>|<span data-ttu-id="44bee-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="44bee-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="44bee-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="44bee-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44bee-163">version</span><span class="sxs-lookup"><span data-stu-id="44bee-163">version</span></span>|<span data-ttu-id="44bee-164">Int32</span><span class="sxs-lookup"><span data-stu-id="44bee-164">Int32</span></span>|<span data-ttu-id="44bee-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="44bee-165">Version of the device configuration.</span></span> <span data-ttu-id="44bee-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="44bee-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44bee-167">networkname</span><span class="sxs-lookup"><span data-stu-id="44bee-167">networkName</span></span>|<span data-ttu-id="44bee-168">String</span><span class="sxs-lookup"><span data-stu-id="44bee-168">String</span></span>|<span data-ttu-id="44bee-169">ネットワーク名</span><span class="sxs-lookup"><span data-stu-id="44bee-169">Network Name</span></span>|
|<span data-ttu-id="44bee-170">ssid</span><span class="sxs-lookup"><span data-stu-id="44bee-170">ssid</span></span>|<span data-ttu-id="44bee-171">String</span><span class="sxs-lookup"><span data-stu-id="44bee-171">String</span></span>|<span data-ttu-id="44bee-172">これは、すべてのデバイスにブロードキャストされている wi-fi ネットワークの名前です。</span><span class="sxs-lookup"><span data-stu-id="44bee-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="44bee-173">connectautomatically に</span><span class="sxs-lookup"><span data-stu-id="44bee-173">connectAutomatically</span></span>|<span data-ttu-id="44bee-174">ブール値</span><span class="sxs-lookup"><span data-stu-id="44bee-174">Boolean</span></span>|<span data-ttu-id="44bee-175">このネットワークが範囲内にあるときに自動的に接続します。</span><span class="sxs-lookup"><span data-stu-id="44bee-175">Connect automatically when this network is in range.</span></span> <span data-ttu-id="44bee-176">この値を true に設定すると、ユーザープロンプトがスキップされ、デバイスが wi-fi ネットワークに自動的に接続されます。</span><span class="sxs-lookup"><span data-stu-id="44bee-176">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="44bee-177">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="44bee-177">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="44bee-178">ブール値</span><span class="sxs-lookup"><span data-stu-id="44bee-178">Boolean</span></span>|<span data-ttu-id="44bee-179">このプロファイルが true に設定されている場合、デバイスは、その SSID をすべてのデバイスにブロードキャストしないネットワークに強制的に接続します。</span><span class="sxs-lookup"><span data-stu-id="44bee-179">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="44bee-180">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="44bee-180">wiFiSecurityType</span></span>|[<span data-ttu-id="44bee-181">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="44bee-181">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="44bee-182">wi-fi エンドポイントで EAP ベースのセキュリティの種類を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="44bee-182">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="44bee-183">使用可能な値は、`open`、`wpaEnterprise` です。</span><span class="sxs-lookup"><span data-stu-id="44bee-183">Possible values are: `open`, `wpaEnterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="44bee-184">応答</span><span class="sxs-lookup"><span data-stu-id="44bee-184">Response</span></span>
<span data-ttu-id="44bee-185">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="44bee-185">If successful, this method returns a `201 Created` response code and a [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44bee-186">例</span><span class="sxs-lookup"><span data-stu-id="44bee-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="44bee-187">要求</span><span class="sxs-lookup"><span data-stu-id="44bee-187">Request</span></span>
<span data-ttu-id="44bee-188">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="44bee-188">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="44bee-189">応答</span><span class="sxs-lookup"><span data-stu-id="44bee-189">Response</span></span>
<span data-ttu-id="44bee-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="44bee-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




