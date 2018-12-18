---
title: Windows81TrustedRootCertificate を作成します。
description: 新しい windows81TrustedRootCertificate オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 62703ff94b239b4daca1bca755a85c4ef8755ace
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350756"
---
# <a name="create-windows81trustedrootcertificate"></a><span data-ttu-id="156e7-103">Windows81TrustedRootCertificate を作成します。</span><span class="sxs-lookup"><span data-stu-id="156e7-103">Create windows81TrustedRootCertificate</span></span>

> <span data-ttu-id="156e7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="156e7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="156e7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="156e7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="156e7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="156e7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="156e7-107">新しい[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="156e7-107">Create a new [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="156e7-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="156e7-108">Prerequisites</span></span>
<span data-ttu-id="156e7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="156e7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="156e7-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="156e7-111">Permission type</span></span>|<span data-ttu-id="156e7-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="156e7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="156e7-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="156e7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="156e7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="156e7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="156e7-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="156e7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="156e7-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="156e7-116">Not supported.</span></span>|
|<span data-ttu-id="156e7-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="156e7-117">Application</span></span>|<span data-ttu-id="156e7-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="156e7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="156e7-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="156e7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="156e7-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="156e7-120">Request headers</span></span>
|<span data-ttu-id="156e7-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="156e7-121">Header</span></span>|<span data-ttu-id="156e7-122">値</span><span class="sxs-lookup"><span data-stu-id="156e7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="156e7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="156e7-123">Authorization</span></span>|<span data-ttu-id="156e7-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="156e7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="156e7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="156e7-125">Accept</span></span>|<span data-ttu-id="156e7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="156e7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="156e7-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="156e7-127">Request body</span></span>
<span data-ttu-id="156e7-128">要求の本文に windows81TrustedRootCertificate オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="156e7-128">In the request body, supply a JSON representation for the windows81TrustedRootCertificate object.</span></span>

<span data-ttu-id="156e7-129">次の表は、windows81TrustedRootCertificate を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="156e7-129">The following table shows the properties that are required when you create the windows81TrustedRootCertificate.</span></span>

|<span data-ttu-id="156e7-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="156e7-130">Property</span></span>|<span data-ttu-id="156e7-131">種類</span><span class="sxs-lookup"><span data-stu-id="156e7-131">Type</span></span>|<span data-ttu-id="156e7-132">説明</span><span class="sxs-lookup"><span data-stu-id="156e7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="156e7-133">ID</span><span class="sxs-lookup"><span data-stu-id="156e7-133">id</span></span>|<span data-ttu-id="156e7-134">String</span><span class="sxs-lookup"><span data-stu-id="156e7-134">String</span></span>|<span data-ttu-id="156e7-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="156e7-135">Key of the entity.</span></span> <span data-ttu-id="156e7-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="156e7-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="156e7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="156e7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="156e7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="156e7-138">DateTimeOffset</span></span>|<span data-ttu-id="156e7-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="156e7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="156e7-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="156e7-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="156e7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="156e7-141">roleScopeTagIds</span></span>|<span data-ttu-id="156e7-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="156e7-142">String collection</span></span>|<span data-ttu-id="156e7-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="156e7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="156e7-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="156e7-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="156e7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="156e7-145">supportsScopeTags</span></span>|<span data-ttu-id="156e7-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="156e7-146">Boolean</span></span>|<span data-ttu-id="156e7-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="156e7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="156e7-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="156e7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="156e7-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="156e7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="156e7-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="156e7-150">This property is read-only.</span></span> <span data-ttu-id="156e7-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="156e7-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="156e7-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="156e7-152">createdDateTime</span></span>|<span data-ttu-id="156e7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="156e7-153">DateTimeOffset</span></span>|<span data-ttu-id="156e7-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="156e7-154">DateTime the object was created.</span></span> <span data-ttu-id="156e7-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="156e7-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="156e7-156">説明</span><span class="sxs-lookup"><span data-stu-id="156e7-156">description</span></span>|<span data-ttu-id="156e7-157">String</span><span class="sxs-lookup"><span data-stu-id="156e7-157">String</span></span>|<span data-ttu-id="156e7-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="156e7-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="156e7-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="156e7-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="156e7-160">displayName</span><span class="sxs-lookup"><span data-stu-id="156e7-160">displayName</span></span>|<span data-ttu-id="156e7-161">String</span><span class="sxs-lookup"><span data-stu-id="156e7-161">String</span></span>|<span data-ttu-id="156e7-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="156e7-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="156e7-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="156e7-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="156e7-164">version</span><span class="sxs-lookup"><span data-stu-id="156e7-164">version</span></span>|<span data-ttu-id="156e7-165">Int32</span><span class="sxs-lookup"><span data-stu-id="156e7-165">Int32</span></span>|<span data-ttu-id="156e7-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="156e7-166">Version of the device configuration.</span></span> <span data-ttu-id="156e7-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="156e7-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="156e7-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="156e7-168">trustedRootCertificate</span></span>|<span data-ttu-id="156e7-169">Binary</span><span class="sxs-lookup"><span data-stu-id="156e7-169">Binary</span></span>|<span data-ttu-id="156e7-170">信頼されたルート証明書</span><span class="sxs-lookup"><span data-stu-id="156e7-170">Trusted Root Certificate</span></span>|
|<span data-ttu-id="156e7-171">します</span><span class="sxs-lookup"><span data-stu-id="156e7-171">certFileName</span></span>|<span data-ttu-id="156e7-172">String</span><span class="sxs-lookup"><span data-stu-id="156e7-172">String</span></span>|<span data-ttu-id="156e7-173">UI に表示するファイル名です。</span><span class="sxs-lookup"><span data-stu-id="156e7-173">File name to display in UI.</span></span>|
|<span data-ttu-id="156e7-174">destinationStore</span><span class="sxs-lookup"><span data-stu-id="156e7-174">destinationStore</span></span>|[<span data-ttu-id="156e7-175">certificateDestinationStore</span><span class="sxs-lookup"><span data-stu-id="156e7-175">certificateDestinationStore</span></span>](../resources/intune-deviceconfig-certificatedestinationstore.md)|<span data-ttu-id="156e7-176">信頼されたルート証明書のコピー先の保存場所。</span><span class="sxs-lookup"><span data-stu-id="156e7-176">Destination store location for the Trusted Root Certificate.</span></span> <span data-ttu-id="156e7-177">可能な値は、`computerCertStoreRoot`、`computerCertStoreIntermediate`、`userCertStoreIntermediate` です。</span><span class="sxs-lookup"><span data-stu-id="156e7-177">Possible values are: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span></span>|



## <a name="response"></a><span data-ttu-id="156e7-178">応答</span><span class="sxs-lookup"><span data-stu-id="156e7-178">Response</span></span>
<span data-ttu-id="156e7-179">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="156e7-179">If successful, this method returns a `201 Created` response code and a [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="156e7-180">例</span><span class="sxs-lookup"><span data-stu-id="156e7-180">Example</span></span>
### <a name="request"></a><span data-ttu-id="156e7-181">要求</span><span class="sxs-lookup"><span data-stu-id="156e7-181">Request</span></span>
<span data-ttu-id="156e7-182">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="156e7-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation
Content-type: application/json
Content-length: 489

{
  "@odata.type": "#microsoft.graph.windows81TrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="156e7-183">応答</span><span class="sxs-lookup"><span data-stu-id="156e7-183">Response</span></span>
<span data-ttu-id="156e7-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="156e7-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





