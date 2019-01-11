---
title: MacOSTrustedRootCertificate を更新します。
description: MacOSTrustedRootCertificate オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 38e0d22621dfb7fa59d55ffc292fc4ea18addb73
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890833"
---
# <a name="update-macostrustedrootcertificate"></a><span data-ttu-id="f0223-103">MacOSTrustedRootCertificate を更新します。</span><span class="sxs-lookup"><span data-stu-id="f0223-103">Update macOSTrustedRootCertificate</span></span>

> <span data-ttu-id="f0223-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f0223-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0223-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0223-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f0223-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f0223-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f0223-107">[MacOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f0223-107">Update the properties of a [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f0223-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="f0223-108">Prerequisites</span></span>
<span data-ttu-id="f0223-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f0223-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0223-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f0223-111">Permission type</span></span>|<span data-ttu-id="f0223-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f0223-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0223-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f0223-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f0223-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0223-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f0223-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f0223-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0223-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0223-116">Not supported.</span></span>|
|<span data-ttu-id="f0223-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f0223-117">Application</span></span>|<span data-ttu-id="f0223-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0223-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0223-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f0223-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="f0223-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f0223-120">Request headers</span></span>
|<span data-ttu-id="f0223-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f0223-121">Header</span></span>|<span data-ttu-id="f0223-122">値</span><span class="sxs-lookup"><span data-stu-id="f0223-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0223-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0223-123">Authorization</span></span>|<span data-ttu-id="f0223-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f0223-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0223-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f0223-125">Accept</span></span>|<span data-ttu-id="f0223-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0223-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0223-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f0223-127">Request body</span></span>
<span data-ttu-id="f0223-128">要求の本文に[macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="f0223-128">In the request body, supply a JSON representation for the [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="f0223-129">[MacOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="f0223-129">The following table shows the properties that are required when you create the [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md).</span></span>

|<span data-ttu-id="f0223-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0223-130">Property</span></span>|<span data-ttu-id="f0223-131">種類</span><span class="sxs-lookup"><span data-stu-id="f0223-131">Type</span></span>|<span data-ttu-id="f0223-132">説明</span><span class="sxs-lookup"><span data-stu-id="f0223-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0223-133">ID</span><span class="sxs-lookup"><span data-stu-id="f0223-133">id</span></span>|<span data-ttu-id="f0223-134">String</span><span class="sxs-lookup"><span data-stu-id="f0223-134">String</span></span>|<span data-ttu-id="f0223-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f0223-135">Key of the entity.</span></span> <span data-ttu-id="f0223-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f0223-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0223-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0223-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f0223-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0223-138">DateTimeOffset</span></span>|<span data-ttu-id="f0223-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f0223-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f0223-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f0223-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0223-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f0223-141">roleScopeTagIds</span></span>|<span data-ttu-id="f0223-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f0223-142">String collection</span></span>|<span data-ttu-id="f0223-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="f0223-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f0223-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f0223-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0223-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f0223-145">supportsScopeTags</span></span>|<span data-ttu-id="f0223-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="f0223-146">Boolean</span></span>|<span data-ttu-id="f0223-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f0223-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f0223-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="f0223-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f0223-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="f0223-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f0223-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="f0223-150">This property is read-only.</span></span> <span data-ttu-id="f0223-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f0223-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0223-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f0223-152">createdDateTime</span></span>|<span data-ttu-id="f0223-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0223-153">DateTimeOffset</span></span>|<span data-ttu-id="f0223-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f0223-154">DateTime the object was created.</span></span> <span data-ttu-id="f0223-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f0223-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0223-156">説明</span><span class="sxs-lookup"><span data-stu-id="f0223-156">description</span></span>|<span data-ttu-id="f0223-157">String</span><span class="sxs-lookup"><span data-stu-id="f0223-157">String</span></span>|<span data-ttu-id="f0223-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="f0223-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f0223-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f0223-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0223-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f0223-160">displayName</span></span>|<span data-ttu-id="f0223-161">String</span><span class="sxs-lookup"><span data-stu-id="f0223-161">String</span></span>|<span data-ttu-id="f0223-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="f0223-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f0223-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f0223-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0223-164">version</span><span class="sxs-lookup"><span data-stu-id="f0223-164">version</span></span>|<span data-ttu-id="f0223-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f0223-165">Int32</span></span>|<span data-ttu-id="f0223-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="f0223-166">Version of the device configuration.</span></span> <span data-ttu-id="f0223-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f0223-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0223-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="f0223-168">trustedRootCertificate</span></span>|<span data-ttu-id="f0223-169">Binary</span><span class="sxs-lookup"><span data-stu-id="f0223-169">Binary</span></span>|<span data-ttu-id="f0223-170">信頼されたルート証明書です。</span><span class="sxs-lookup"><span data-stu-id="f0223-170">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="f0223-171">します</span><span class="sxs-lookup"><span data-stu-id="f0223-171">certFileName</span></span>|<span data-ttu-id="f0223-172">String</span><span class="sxs-lookup"><span data-stu-id="f0223-172">String</span></span>|<span data-ttu-id="f0223-173">UI に表示するファイル名です。</span><span class="sxs-lookup"><span data-stu-id="f0223-173">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="f0223-174">応答</span><span class="sxs-lookup"><span data-stu-id="f0223-174">Response</span></span>
<span data-ttu-id="f0223-175">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f0223-175">If successful, this method returns a `200 OK` response code and an updated [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0223-176">例</span><span class="sxs-lookup"><span data-stu-id="f0223-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="f0223-177">要求</span><span class="sxs-lookup"><span data-stu-id="f0223-177">Request</span></span>
<span data-ttu-id="f0223-178">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f0223-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate
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

### <a name="response"></a><span data-ttu-id="f0223-179">応答</span><span class="sxs-lookup"><span data-stu-id="f0223-179">Response</span></span>
<span data-ttu-id="f0223-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f0223-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 537

{
  "@odata.type": "#microsoft.graph.macOSTrustedRootCertificate",
  "id": "c5fac954-c954-c5fa-54c9-fac554c9fac5",
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





