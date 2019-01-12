---
title: Windows81TrustedRootCertificate を更新します。
description: Windows81TrustedRootCertificate オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1e3f6ca1cebbedd1f3603cbc7b0294d3ab616b31
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944671"
---
# <a name="update-windows81trustedrootcertificate"></a><span data-ttu-id="20826-103">Windows81TrustedRootCertificate を更新します。</span><span class="sxs-lookup"><span data-stu-id="20826-103">Update windows81TrustedRootCertificate</span></span>

> <span data-ttu-id="20826-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="20826-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="20826-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20826-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="20826-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="20826-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20826-107">[Windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="20826-107">Update the properties of a [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="20826-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="20826-108">Prerequisites</span></span>
<span data-ttu-id="20826-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="20826-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20826-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="20826-111">Permission type</span></span>|<span data-ttu-id="20826-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="20826-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20826-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="20826-113">Delegated (work or school account)</span></span>|<span data-ttu-id="20826-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20826-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="20826-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="20826-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20826-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20826-116">Not supported.</span></span>|
|<span data-ttu-id="20826-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="20826-117">Application</span></span>|<span data-ttu-id="20826-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20826-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20826-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="20826-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="20826-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="20826-120">Request headers</span></span>
|<span data-ttu-id="20826-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="20826-121">Header</span></span>|<span data-ttu-id="20826-122">値</span><span class="sxs-lookup"><span data-stu-id="20826-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20826-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="20826-123">Authorization</span></span>|<span data-ttu-id="20826-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="20826-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20826-125">Accept</span><span class="sxs-lookup"><span data-stu-id="20826-125">Accept</span></span>|<span data-ttu-id="20826-126">application/json</span><span class="sxs-lookup"><span data-stu-id="20826-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20826-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="20826-127">Request body</span></span>
<span data-ttu-id="20826-128">要求の本文に[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="20826-128">In the request body, supply a JSON representation for the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

<span data-ttu-id="20826-129">[Windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="20826-129">The following table shows the properties that are required when you create the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md).</span></span>

|<span data-ttu-id="20826-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="20826-130">Property</span></span>|<span data-ttu-id="20826-131">種類</span><span class="sxs-lookup"><span data-stu-id="20826-131">Type</span></span>|<span data-ttu-id="20826-132">説明</span><span class="sxs-lookup"><span data-stu-id="20826-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20826-133">ID</span><span class="sxs-lookup"><span data-stu-id="20826-133">id</span></span>|<span data-ttu-id="20826-134">String</span><span class="sxs-lookup"><span data-stu-id="20826-134">String</span></span>|<span data-ttu-id="20826-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="20826-135">Key of the entity.</span></span> <span data-ttu-id="20826-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20826-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20826-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="20826-137">lastModifiedDateTime</span></span>|<span data-ttu-id="20826-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20826-138">DateTimeOffset</span></span>|<span data-ttu-id="20826-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="20826-139">DateTime the object was last modified.</span></span> <span data-ttu-id="20826-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20826-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20826-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="20826-141">roleScopeTagIds</span></span>|<span data-ttu-id="20826-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="20826-142">String collection</span></span>|<span data-ttu-id="20826-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="20826-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="20826-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20826-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20826-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="20826-145">supportsScopeTags</span></span>|<span data-ttu-id="20826-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="20826-146">Boolean</span></span>|<span data-ttu-id="20826-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="20826-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="20826-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="20826-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="20826-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="20826-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="20826-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="20826-150">This property is read-only.</span></span> <span data-ttu-id="20826-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20826-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20826-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="20826-152">createdDateTime</span></span>|<span data-ttu-id="20826-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20826-153">DateTimeOffset</span></span>|<span data-ttu-id="20826-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="20826-154">DateTime the object was created.</span></span> <span data-ttu-id="20826-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20826-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20826-156">説明</span><span class="sxs-lookup"><span data-stu-id="20826-156">description</span></span>|<span data-ttu-id="20826-157">String</span><span class="sxs-lookup"><span data-stu-id="20826-157">String</span></span>|<span data-ttu-id="20826-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="20826-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="20826-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20826-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20826-160">displayName</span><span class="sxs-lookup"><span data-stu-id="20826-160">displayName</span></span>|<span data-ttu-id="20826-161">String</span><span class="sxs-lookup"><span data-stu-id="20826-161">String</span></span>|<span data-ttu-id="20826-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="20826-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="20826-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20826-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20826-164">version</span><span class="sxs-lookup"><span data-stu-id="20826-164">version</span></span>|<span data-ttu-id="20826-165">Int32</span><span class="sxs-lookup"><span data-stu-id="20826-165">Int32</span></span>|<span data-ttu-id="20826-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="20826-166">Version of the device configuration.</span></span> <span data-ttu-id="20826-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20826-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20826-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="20826-168">trustedRootCertificate</span></span>|<span data-ttu-id="20826-169">Binary</span><span class="sxs-lookup"><span data-stu-id="20826-169">Binary</span></span>|<span data-ttu-id="20826-170">信頼されたルート証明書</span><span class="sxs-lookup"><span data-stu-id="20826-170">Trusted Root Certificate</span></span>|
|<span data-ttu-id="20826-171">します</span><span class="sxs-lookup"><span data-stu-id="20826-171">certFileName</span></span>|<span data-ttu-id="20826-172">String</span><span class="sxs-lookup"><span data-stu-id="20826-172">String</span></span>|<span data-ttu-id="20826-173">UI に表示するファイル名です。</span><span class="sxs-lookup"><span data-stu-id="20826-173">File name to display in UI.</span></span>|
|<span data-ttu-id="20826-174">destinationStore</span><span class="sxs-lookup"><span data-stu-id="20826-174">destinationStore</span></span>|[<span data-ttu-id="20826-175">certificateDestinationStore</span><span class="sxs-lookup"><span data-stu-id="20826-175">certificateDestinationStore</span></span>](../resources/intune-deviceconfig-certificatedestinationstore.md)|<span data-ttu-id="20826-176">信頼されたルート証明書のコピー先の保存場所。</span><span class="sxs-lookup"><span data-stu-id="20826-176">Destination store location for the Trusted Root Certificate.</span></span> <span data-ttu-id="20826-177">可能な値は、`computerCertStoreRoot`、`computerCertStoreIntermediate`、`userCertStoreIntermediate` です。</span><span class="sxs-lookup"><span data-stu-id="20826-177">Possible values are: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span></span>|



## <a name="response"></a><span data-ttu-id="20826-178">応答</span><span class="sxs-lookup"><span data-stu-id="20826-178">Response</span></span>
<span data-ttu-id="20826-179">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="20826-179">If successful, this method returns a `200 OK` response code and an updated [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20826-180">例</span><span class="sxs-lookup"><span data-stu-id="20826-180">Example</span></span>
### <a name="request"></a><span data-ttu-id="20826-181">要求</span><span class="sxs-lookup"><span data-stu-id="20826-181">Request</span></span>
<span data-ttu-id="20826-182">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="20826-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
Content-type: application/json
Content-length: 419

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```

### <a name="response"></a><span data-ttu-id="20826-183">応答</span><span class="sxs-lookup"><span data-stu-id="20826-183">Response</span></span>
<span data-ttu-id="20826-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="20826-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 597

{
  "@odata.type": "#microsoft.graph.windows81TrustedRootCertificate",
  "id": "3fb588f9-88f9-3fb5-f988-b53ff988b53f",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```





