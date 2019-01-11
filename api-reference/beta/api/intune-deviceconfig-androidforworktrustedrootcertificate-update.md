---
title: AndroidForWorkTrustedRootCertificate を更新します。
description: AndroidForWorkTrustedRootCertificate オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0ebe70fc53ce18d0bd369adf5ea2585ebfa8b934
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891078"
---
# <a name="update-androidforworktrustedrootcertificate"></a><span data-ttu-id="ecbbd-103">AndroidForWorkTrustedRootCertificate を更新します。</span><span class="sxs-lookup"><span data-stu-id="ecbbd-103">Update androidForWorkTrustedRootCertificate</span></span>

> <span data-ttu-id="ecbbd-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ecbbd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ecbbd-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ecbbd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ecbbd-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ecbbd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ecbbd-107">[AndroidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ecbbd-107">Update the properties of a [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ecbbd-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ecbbd-108">Prerequisites</span></span>
<span data-ttu-id="ecbbd-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ecbbd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecbbd-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ecbbd-111">Permission type</span></span>|<span data-ttu-id="ecbbd-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ecbbd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecbbd-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ecbbd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ecbbd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecbbd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ecbbd-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ecbbd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecbbd-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ecbbd-116">Not supported.</span></span>|
|<span data-ttu-id="ecbbd-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ecbbd-117">Application</span></span>|<span data-ttu-id="ecbbd-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ecbbd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecbbd-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ecbbd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="ecbbd-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ecbbd-120">Request headers</span></span>
|<span data-ttu-id="ecbbd-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ecbbd-121">Header</span></span>|<span data-ttu-id="ecbbd-122">値</span><span class="sxs-lookup"><span data-stu-id="ecbbd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ecbbd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ecbbd-123">Authorization</span></span>|<span data-ttu-id="ecbbd-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ecbbd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ecbbd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ecbbd-125">Accept</span></span>|<span data-ttu-id="ecbbd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ecbbd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecbbd-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ecbbd-127">Request body</span></span>
<span data-ttu-id="ecbbd-128">要求の本文に[androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="ecbbd-128">In the request body, supply a JSON representation for the [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="ecbbd-129">[AndroidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="ecbbd-129">The following table shows the properties that are required when you create the [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md).</span></span>

|<span data-ttu-id="ecbbd-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ecbbd-130">Property</span></span>|<span data-ttu-id="ecbbd-131">種類</span><span class="sxs-lookup"><span data-stu-id="ecbbd-131">Type</span></span>|<span data-ttu-id="ecbbd-132">説明</span><span class="sxs-lookup"><span data-stu-id="ecbbd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecbbd-133">ID</span><span class="sxs-lookup"><span data-stu-id="ecbbd-133">id</span></span>|<span data-ttu-id="ecbbd-134">String</span><span class="sxs-lookup"><span data-stu-id="ecbbd-134">String</span></span>|<span data-ttu-id="ecbbd-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ecbbd-135">Key of the entity.</span></span> <span data-ttu-id="ecbbd-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ecbbd-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecbbd-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ecbbd-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ecbbd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ecbbd-138">DateTimeOffset</span></span>|<span data-ttu-id="ecbbd-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="ecbbd-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ecbbd-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ecbbd-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecbbd-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ecbbd-141">roleScopeTagIds</span></span>|<span data-ttu-id="ecbbd-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="ecbbd-142">String collection</span></span>|<span data-ttu-id="ecbbd-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="ecbbd-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ecbbd-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ecbbd-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecbbd-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ecbbd-145">supportsScopeTags</span></span>|<span data-ttu-id="ecbbd-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="ecbbd-146">Boolean</span></span>|<span data-ttu-id="ecbbd-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ecbbd-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ecbbd-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="ecbbd-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ecbbd-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="ecbbd-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ecbbd-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="ecbbd-150">This property is read-only.</span></span> <span data-ttu-id="ecbbd-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ecbbd-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecbbd-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ecbbd-152">createdDateTime</span></span>|<span data-ttu-id="ecbbd-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ecbbd-153">DateTimeOffset</span></span>|<span data-ttu-id="ecbbd-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="ecbbd-154">DateTime the object was created.</span></span> <span data-ttu-id="ecbbd-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ecbbd-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecbbd-156">説明</span><span class="sxs-lookup"><span data-stu-id="ecbbd-156">description</span></span>|<span data-ttu-id="ecbbd-157">String</span><span class="sxs-lookup"><span data-stu-id="ecbbd-157">String</span></span>|<span data-ttu-id="ecbbd-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="ecbbd-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ecbbd-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ecbbd-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecbbd-160">displayName</span><span class="sxs-lookup"><span data-stu-id="ecbbd-160">displayName</span></span>|<span data-ttu-id="ecbbd-161">String</span><span class="sxs-lookup"><span data-stu-id="ecbbd-161">String</span></span>|<span data-ttu-id="ecbbd-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="ecbbd-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ecbbd-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ecbbd-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecbbd-164">version</span><span class="sxs-lookup"><span data-stu-id="ecbbd-164">version</span></span>|<span data-ttu-id="ecbbd-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ecbbd-165">Int32</span></span>|<span data-ttu-id="ecbbd-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="ecbbd-166">Version of the device configuration.</span></span> <span data-ttu-id="ecbbd-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ecbbd-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecbbd-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="ecbbd-168">trustedRootCertificate</span></span>|<span data-ttu-id="ecbbd-169">Binary</span><span class="sxs-lookup"><span data-stu-id="ecbbd-169">Binary</span></span>|<span data-ttu-id="ecbbd-170">信頼されたルート証明書</span><span class="sxs-lookup"><span data-stu-id="ecbbd-170">Trusted Root Certificate</span></span>|
|<span data-ttu-id="ecbbd-171">します</span><span class="sxs-lookup"><span data-stu-id="ecbbd-171">certFileName</span></span>|<span data-ttu-id="ecbbd-172">String</span><span class="sxs-lookup"><span data-stu-id="ecbbd-172">String</span></span>|<span data-ttu-id="ecbbd-173">UI に表示するファイル名です。</span><span class="sxs-lookup"><span data-stu-id="ecbbd-173">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="ecbbd-174">応答</span><span class="sxs-lookup"><span data-stu-id="ecbbd-174">Response</span></span>
<span data-ttu-id="ecbbd-175">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="ecbbd-175">If successful, this method returns a `200 OK` response code and an updated [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecbbd-176">例</span><span class="sxs-lookup"><span data-stu-id="ecbbd-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="ecbbd-177">要求</span><span class="sxs-lookup"><span data-stu-id="ecbbd-177">Request</span></span>
<span data-ttu-id="ecbbd-178">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ecbbd-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate
Content-type: application/json
Content-length: 363

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
  "certFileName": "Cert File Name value"
}
```

### <a name="response"></a><span data-ttu-id="ecbbd-179">応答</span><span class="sxs-lookup"><span data-stu-id="ecbbd-179">Response</span></span>
<span data-ttu-id="ecbbd-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ecbbd-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 546

{
  "@odata.type": "#microsoft.graph.androidForWorkTrustedRootCertificate",
  "id": "2f78834c-834c-2f78-4c83-782f4c83782f",
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
  "certFileName": "Cert File Name value"
}
```





