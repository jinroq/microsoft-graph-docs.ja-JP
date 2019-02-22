---
title: androidDeviceOwnerWiFiConfiguration を作成する
description: 新しい androidDeviceOwnerWiFiConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7062e0bb32643474905d8c26921da6cb631b99b1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147524"
---
# <a name="create-androiddeviceownerwificonfiguration"></a><span data-ttu-id="96402-103">androidDeviceOwnerWiFiConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="96402-103">Create androidDeviceOwnerWiFiConfiguration</span></span>

> <span data-ttu-id="96402-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96402-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96402-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="96402-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96402-106">新しい[androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="96402-106">Create a new [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96402-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="96402-107">Prerequisites</span></span>
<span data-ttu-id="96402-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="96402-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="96402-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="96402-110">Permission type</span></span>|<span data-ttu-id="96402-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="96402-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96402-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="96402-112">Delegated (work or school account)</span></span>|<span data-ttu-id="96402-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96402-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="96402-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="96402-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96402-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96402-115">Not supported.</span></span>|
|<span data-ttu-id="96402-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="96402-116">Application</span></span>|<span data-ttu-id="96402-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96402-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96402-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="96402-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="96402-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="96402-119">Request headers</span></span>
|<span data-ttu-id="96402-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="96402-120">Header</span></span>|<span data-ttu-id="96402-121">値</span><span class="sxs-lookup"><span data-stu-id="96402-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96402-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="96402-122">Authorization</span></span>|<span data-ttu-id="96402-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="96402-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96402-124">承諾</span><span class="sxs-lookup"><span data-stu-id="96402-124">Accept</span></span>|<span data-ttu-id="96402-125">application/json</span><span class="sxs-lookup"><span data-stu-id="96402-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96402-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="96402-126">Request body</span></span>
<span data-ttu-id="96402-127">要求本文で、androidDeviceOwnerWiFiConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="96402-127">In the request body, supply a JSON representation for the androidDeviceOwnerWiFiConfiguration object.</span></span>

<span data-ttu-id="96402-128">次の表に、androidDeviceOwnerWiFiConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="96402-128">The following table shows the properties that are required when you create the androidDeviceOwnerWiFiConfiguration.</span></span>

|<span data-ttu-id="96402-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96402-129">Property</span></span>|<span data-ttu-id="96402-130">型</span><span class="sxs-lookup"><span data-stu-id="96402-130">Type</span></span>|<span data-ttu-id="96402-131">説明</span><span class="sxs-lookup"><span data-stu-id="96402-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96402-132">id</span><span class="sxs-lookup"><span data-stu-id="96402-132">id</span></span>|<span data-ttu-id="96402-133">文字列</span><span class="sxs-lookup"><span data-stu-id="96402-133">String</span></span>|<span data-ttu-id="96402-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="96402-134">Key of the entity.</span></span> <span data-ttu-id="96402-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="96402-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96402-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="96402-136">lastModifiedDateTime</span></span>|<span data-ttu-id="96402-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96402-137">DateTimeOffset</span></span>|<span data-ttu-id="96402-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="96402-138">DateTime the object was last modified.</span></span> <span data-ttu-id="96402-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="96402-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96402-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="96402-140">roleScopeTagIds</span></span>|<span data-ttu-id="96402-141">String collection</span><span class="sxs-lookup"><span data-stu-id="96402-141">String collection</span></span>|<span data-ttu-id="96402-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="96402-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="96402-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="96402-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96402-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="96402-144">supportsScopeTags</span></span>|<span data-ttu-id="96402-145">ブール値</span><span class="sxs-lookup"><span data-stu-id="96402-145">Boolean</span></span>|<span data-ttu-id="96402-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="96402-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="96402-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="96402-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="96402-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="96402-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="96402-149">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="96402-149">This property is read-only.</span></span> <span data-ttu-id="96402-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="96402-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96402-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="96402-151">createdDateTime</span></span>|<span data-ttu-id="96402-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96402-152">DateTimeOffset</span></span>|<span data-ttu-id="96402-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="96402-153">DateTime the object was created.</span></span> <span data-ttu-id="96402-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="96402-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96402-155">説明</span><span class="sxs-lookup"><span data-stu-id="96402-155">description</span></span>|<span data-ttu-id="96402-156">String</span><span class="sxs-lookup"><span data-stu-id="96402-156">String</span></span>|<span data-ttu-id="96402-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="96402-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="96402-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="96402-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96402-159">displayName</span><span class="sxs-lookup"><span data-stu-id="96402-159">displayName</span></span>|<span data-ttu-id="96402-160">String</span><span class="sxs-lookup"><span data-stu-id="96402-160">String</span></span>|<span data-ttu-id="96402-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="96402-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="96402-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="96402-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96402-163">version</span><span class="sxs-lookup"><span data-stu-id="96402-163">version</span></span>|<span data-ttu-id="96402-164">Int32</span><span class="sxs-lookup"><span data-stu-id="96402-164">Int32</span></span>|<span data-ttu-id="96402-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="96402-165">Version of the device configuration.</span></span> <span data-ttu-id="96402-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="96402-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96402-167">networkname</span><span class="sxs-lookup"><span data-stu-id="96402-167">networkName</span></span>|<span data-ttu-id="96402-168">String</span><span class="sxs-lookup"><span data-stu-id="96402-168">String</span></span>|<span data-ttu-id="96402-169">ネットワーク名</span><span class="sxs-lookup"><span data-stu-id="96402-169">Network Name</span></span>|
|<span data-ttu-id="96402-170">ssid</span><span class="sxs-lookup"><span data-stu-id="96402-170">ssid</span></span>|<span data-ttu-id="96402-171">String</span><span class="sxs-lookup"><span data-stu-id="96402-171">String</span></span>|<span data-ttu-id="96402-172">これは、すべてのデバイスにブロードキャストされている wi-fi ネットワークの名前です。</span><span class="sxs-lookup"><span data-stu-id="96402-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="96402-173">connectautomatically に</span><span class="sxs-lookup"><span data-stu-id="96402-173">connectAutomatically</span></span>|<span data-ttu-id="96402-174">ブール値</span><span class="sxs-lookup"><span data-stu-id="96402-174">Boolean</span></span>|<span data-ttu-id="96402-175">このネットワークが範囲内にあるときに自動的に接続します。</span><span class="sxs-lookup"><span data-stu-id="96402-175">Connect automatically when this network is in range.</span></span> <span data-ttu-id="96402-176">この値を true に設定すると、ユーザープロンプトがスキップされ、デバイスが wi-fi ネットワークに自動的に接続されます。</span><span class="sxs-lookup"><span data-stu-id="96402-176">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="96402-177">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="96402-177">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="96402-178">ブール値</span><span class="sxs-lookup"><span data-stu-id="96402-178">Boolean</span></span>|<span data-ttu-id="96402-179">このプロファイルが true に設定されている場合、デバイスは、その SSID をすべてのデバイスにブロードキャストしないネットワークに強制的に接続します。</span><span class="sxs-lookup"><span data-stu-id="96402-179">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="96402-180">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="96402-180">wiFiSecurityType</span></span>|[<span data-ttu-id="96402-181">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="96402-181">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="96402-182">wi-fi エンドポイントで EAP ベースのセキュリティの種類を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="96402-182">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="96402-183">可能な値は `open`、`wep`、`wpaPersonal` です。</span><span class="sxs-lookup"><span data-stu-id="96402-183">Possible values are: `open`, `wep`, `wpaPersonal`.</span></span>|
|<span data-ttu-id="96402-184">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="96402-184">preSharedKey</span></span>|<span data-ttu-id="96402-185">String</span><span class="sxs-lookup"><span data-stu-id="96402-185">String</span></span>|<span data-ttu-id="96402-186">これは、WPA 個人用 wi-fi ネットワークの事前共有キーです。</span><span class="sxs-lookup"><span data-stu-id="96402-186">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="96402-187">preSharedKeyIsSet</span><span class="sxs-lookup"><span data-stu-id="96402-187">preSharedKeyIsSet</span></span>|<span data-ttu-id="96402-188">ブール値</span><span class="sxs-lookup"><span data-stu-id="96402-188">Boolean</span></span>|<span data-ttu-id="96402-189">これは、WPA 個人用 wi-fi ネットワークの事前共有キーです。</span><span class="sxs-lookup"><span data-stu-id="96402-189">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="96402-190">応答</span><span class="sxs-lookup"><span data-stu-id="96402-190">Response</span></span>
<span data-ttu-id="96402-191">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="96402-191">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96402-192">例</span><span class="sxs-lookup"><span data-stu-id="96402-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="96402-193">要求</span><span class="sxs-lookup"><span data-stu-id="96402-193">Request</span></span>
<span data-ttu-id="96402-194">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="96402-194">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 509

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="96402-195">応答</span><span class="sxs-lookup"><span data-stu-id="96402-195">Response</span></span>
<span data-ttu-id="96402-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="96402-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




