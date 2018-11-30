---
title: Windows10NetworkBoundaryConfiguration を作成します。
description: 新しい windows10NetworkBoundaryConfiguration オブジェクトを作成します。
ms.openlocfilehash: 23ecf0e8b223f0aa7ac36a1d8406ccd1f56d4bc9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073841"
---
# <a name="create-windows10networkboundaryconfiguration"></a><span data-ttu-id="e6c32-103">Windows10NetworkBoundaryConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="e6c32-103">Create windows10NetworkBoundaryConfiguration</span></span>

> <span data-ttu-id="e6c32-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e6c32-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e6c32-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e6c32-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e6c32-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e6c32-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e6c32-107">新しい[windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e6c32-107">Create a new [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e6c32-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="e6c32-108">Prerequisites</span></span>
<span data-ttu-id="e6c32-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e6c32-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6c32-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e6c32-111">Permission type</span></span>|<span data-ttu-id="e6c32-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e6c32-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6c32-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e6c32-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e6c32-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6c32-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e6c32-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e6c32-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6c32-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e6c32-116">Not supported.</span></span>|
|<span data-ttu-id="e6c32-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e6c32-117">Application</span></span>|<span data-ttu-id="e6c32-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e6c32-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6c32-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e6c32-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e6c32-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e6c32-120">Request headers</span></span>
|<span data-ttu-id="e6c32-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e6c32-121">Header</span></span>|<span data-ttu-id="e6c32-122">値</span><span class="sxs-lookup"><span data-stu-id="e6c32-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6c32-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6c32-123">Authorization</span></span>|<span data-ttu-id="e6c32-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e6c32-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6c32-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e6c32-125">Accept</span></span>|<span data-ttu-id="e6c32-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e6c32-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6c32-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e6c32-127">Request body</span></span>
<span data-ttu-id="e6c32-128">要求の本文に windows10NetworkBoundaryConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="e6c32-128">In the request body, supply a JSON representation for the windows10NetworkBoundaryConfiguration object.</span></span>

<span data-ttu-id="e6c32-129">次の表は、windows10NetworkBoundaryConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e6c32-129">The following table shows the properties that are required when you create the windows10NetworkBoundaryConfiguration.</span></span>

|<span data-ttu-id="e6c32-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e6c32-130">Property</span></span>|<span data-ttu-id="e6c32-131">型</span><span class="sxs-lookup"><span data-stu-id="e6c32-131">Type</span></span>|<span data-ttu-id="e6c32-132">説明</span><span class="sxs-lookup"><span data-stu-id="e6c32-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6c32-133">id</span><span class="sxs-lookup"><span data-stu-id="e6c32-133">id</span></span>|<span data-ttu-id="e6c32-134">String</span><span class="sxs-lookup"><span data-stu-id="e6c32-134">String</span></span>|<span data-ttu-id="e6c32-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e6c32-135">Key of the entity.</span></span> <span data-ttu-id="e6c32-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e6c32-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6c32-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6c32-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e6c32-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6c32-138">DateTimeOffset</span></span>|<span data-ttu-id="e6c32-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e6c32-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e6c32-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e6c32-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6c32-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e6c32-141">roleScopeTagIds</span></span>|<span data-ttu-id="e6c32-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="e6c32-142">String collection</span></span>|<span data-ttu-id="e6c32-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="e6c32-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e6c32-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e6c32-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6c32-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e6c32-145">supportsScopeTags</span></span>|<span data-ttu-id="e6c32-146">ブール値</span><span class="sxs-lookup"><span data-stu-id="e6c32-146">Boolean</span></span>|<span data-ttu-id="e6c32-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e6c32-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e6c32-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="e6c32-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e6c32-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="e6c32-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e6c32-150">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="e6c32-150">This property is read-only.</span></span> <span data-ttu-id="e6c32-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e6c32-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6c32-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e6c32-152">createdDateTime</span></span>|<span data-ttu-id="e6c32-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6c32-153">DateTimeOffset</span></span>|<span data-ttu-id="e6c32-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e6c32-154">DateTime the object was created.</span></span> <span data-ttu-id="e6c32-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e6c32-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6c32-156">説明</span><span class="sxs-lookup"><span data-stu-id="e6c32-156">description</span></span>|<span data-ttu-id="e6c32-157">String</span><span class="sxs-lookup"><span data-stu-id="e6c32-157">String</span></span>|<span data-ttu-id="e6c32-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="e6c32-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e6c32-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e6c32-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6c32-160">displayName</span><span class="sxs-lookup"><span data-stu-id="e6c32-160">displayName</span></span>|<span data-ttu-id="e6c32-161">String</span><span class="sxs-lookup"><span data-stu-id="e6c32-161">String</span></span>|<span data-ttu-id="e6c32-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="e6c32-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e6c32-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e6c32-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6c32-164">version</span><span class="sxs-lookup"><span data-stu-id="e6c32-164">version</span></span>|<span data-ttu-id="e6c32-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e6c32-165">Int32</span></span>|<span data-ttu-id="e6c32-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="e6c32-166">Version of the device configuration.</span></span> <span data-ttu-id="e6c32-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e6c32-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6c32-168">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="e6c32-168">windowsNetworkIsolationPolicy</span></span>|[<span data-ttu-id="e6c32-169">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="e6c32-169">windowsNetworkIsolationPolicy</span></span>](../resources/intune-deviceconfig-windowsnetworkisolationpolicy.md)|<span data-ttu-id="e6c32-170">Windows ネットワークの分離のポリシー</span><span class="sxs-lookup"><span data-stu-id="e6c32-170">Windows Network Isolation Policy</span></span>|



## <a name="response"></a><span data-ttu-id="e6c32-171">応答</span><span class="sxs-lookup"><span data-stu-id="e6c32-171">Response</span></span>
<span data-ttu-id="e6c32-172">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="e6c32-172">If successful, this method returns a `201 Created` response code and a [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6c32-173">例</span><span class="sxs-lookup"><span data-stu-id="e6c32-173">Example</span></span>
### <a name="request"></a><span data-ttu-id="e6c32-174">要求</span><span class="sxs-lookup"><span data-stu-id="e6c32-174">Request</span></span>
<span data-ttu-id="e6c32-175">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e6c32-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1308

{
  "@odata.type": "#microsoft.graph.windows10NetworkBoundaryConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "windowsNetworkIsolationPolicy": {
    "@odata.type": "microsoft.graph.windowsNetworkIsolationPolicy",
    "enterpriseNetworkDomainNames": [
      "Enterprise Network Domain Names value"
    ],
    "enterpriseCloudResources": [
      {
        "@odata.type": "microsoft.graph.proxiedDomain",
        "ipAddressOrFQDN": "Ip Address Or FQDN value",
        "proxy": "Proxy value"
      }
    ],
    "enterpriseIPRanges": [
      {
        "@odata.type": "microsoft.graph.iPv6Range",
        "lowerAddress": "Lower Address value",
        "upperAddress": "Upper Address value"
      }
    ],
    "enterpriseInternalProxyServers": [
      "Enterprise Internal Proxy Servers value"
    ],
    "enterpriseIPRangesAreAuthoritative": true,
    "enterpriseProxyServers": [
      "Enterprise Proxy Servers value"
    ],
    "enterpriseProxyServersAreAuthoritative": true,
    "neutralDomainResources": [
      "Neutral Domain Resources value"
    ]
  }
}
```

### <a name="response"></a><span data-ttu-id="e6c32-176">応答</span><span class="sxs-lookup"><span data-stu-id="e6c32-176">Response</span></span>
<span data-ttu-id="e6c32-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e6c32-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1416

{
  "@odata.type": "#microsoft.graph.windows10NetworkBoundaryConfiguration",
  "id": "afbc9e01-9e01-afbc-019e-bcaf019ebcaf",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "windowsNetworkIsolationPolicy": {
    "@odata.type": "microsoft.graph.windowsNetworkIsolationPolicy",
    "enterpriseNetworkDomainNames": [
      "Enterprise Network Domain Names value"
    ],
    "enterpriseCloudResources": [
      {
        "@odata.type": "microsoft.graph.proxiedDomain",
        "ipAddressOrFQDN": "Ip Address Or FQDN value",
        "proxy": "Proxy value"
      }
    ],
    "enterpriseIPRanges": [
      {
        "@odata.type": "microsoft.graph.iPv6Range",
        "lowerAddress": "Lower Address value",
        "upperAddress": "Upper Address value"
      }
    ],
    "enterpriseInternalProxyServers": [
      "Enterprise Internal Proxy Servers value"
    ],
    "enterpriseIPRangesAreAuthoritative": true,
    "enterpriseProxyServers": [
      "Enterprise Proxy Servers value"
    ],
    "enterpriseProxyServersAreAuthoritative": true,
    "neutralDomainResources": [
      "Neutral Domain Resources value"
    ]
  }
}
```





