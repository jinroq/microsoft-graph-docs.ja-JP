---
title: AndroidWorkProfileTrustedRootCertificate を作成します。
description: 新しい androidWorkProfileTrustedRootCertificate オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e59a3ff49123748cda47112572bd9afd0e225d78
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808149"
---
# <a name="create-androidworkprofiletrustedrootcertificate"></a><span data-ttu-id="0aec6-103">AndroidWorkProfileTrustedRootCertificate を作成します。</span><span class="sxs-lookup"><span data-stu-id="0aec6-103">Create androidWorkProfileTrustedRootCertificate</span></span>

> <span data-ttu-id="0aec6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0aec6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0aec6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0aec6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0aec6-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0aec6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0aec6-107">新しい[androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0aec6-107">Create a new [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0aec6-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="0aec6-108">Prerequisites</span></span>
<span data-ttu-id="0aec6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0aec6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0aec6-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0aec6-111">Permission type</span></span>|<span data-ttu-id="0aec6-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0aec6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0aec6-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0aec6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0aec6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0aec6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0aec6-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0aec6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0aec6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0aec6-116">Not supported.</span></span>|
|<span data-ttu-id="0aec6-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0aec6-117">Application</span></span>|<span data-ttu-id="0aec6-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0aec6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0aec6-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0aec6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0aec6-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0aec6-120">Request headers</span></span>
|<span data-ttu-id="0aec6-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0aec6-121">Header</span></span>|<span data-ttu-id="0aec6-122">値</span><span class="sxs-lookup"><span data-stu-id="0aec6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0aec6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0aec6-123">Authorization</span></span>|<span data-ttu-id="0aec6-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0aec6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0aec6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0aec6-125">Accept</span></span>|<span data-ttu-id="0aec6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0aec6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0aec6-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0aec6-127">Request body</span></span>
<span data-ttu-id="0aec6-128">要求の本文に androidWorkProfileTrustedRootCertificate オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="0aec6-128">In the request body, supply a JSON representation for the androidWorkProfileTrustedRootCertificate object.</span></span>

<span data-ttu-id="0aec6-129">次の表は、androidWorkProfileTrustedRootCertificate を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0aec6-129">The following table shows the properties that are required when you create the androidWorkProfileTrustedRootCertificate.</span></span>

|<span data-ttu-id="0aec6-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0aec6-130">Property</span></span>|<span data-ttu-id="0aec6-131">種類</span><span class="sxs-lookup"><span data-stu-id="0aec6-131">Type</span></span>|<span data-ttu-id="0aec6-132">説明</span><span class="sxs-lookup"><span data-stu-id="0aec6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0aec6-133">ID</span><span class="sxs-lookup"><span data-stu-id="0aec6-133">id</span></span>|<span data-ttu-id="0aec6-134">String</span><span class="sxs-lookup"><span data-stu-id="0aec6-134">String</span></span>|<span data-ttu-id="0aec6-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0aec6-135">Key of the entity.</span></span> <span data-ttu-id="0aec6-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0aec6-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0aec6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0aec6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0aec6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0aec6-138">DateTimeOffset</span></span>|<span data-ttu-id="0aec6-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0aec6-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0aec6-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0aec6-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0aec6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0aec6-141">roleScopeTagIds</span></span>|<span data-ttu-id="0aec6-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0aec6-142">String collection</span></span>|<span data-ttu-id="0aec6-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="0aec6-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0aec6-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0aec6-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0aec6-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0aec6-145">supportsScopeTags</span></span>|<span data-ttu-id="0aec6-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="0aec6-146">Boolean</span></span>|<span data-ttu-id="0aec6-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0aec6-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0aec6-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="0aec6-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0aec6-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="0aec6-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0aec6-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="0aec6-150">This property is read-only.</span></span> <span data-ttu-id="0aec6-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0aec6-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0aec6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0aec6-152">createdDateTime</span></span>|<span data-ttu-id="0aec6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0aec6-153">DateTimeOffset</span></span>|<span data-ttu-id="0aec6-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0aec6-154">DateTime the object was created.</span></span> <span data-ttu-id="0aec6-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0aec6-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0aec6-156">説明</span><span class="sxs-lookup"><span data-stu-id="0aec6-156">description</span></span>|<span data-ttu-id="0aec6-157">String</span><span class="sxs-lookup"><span data-stu-id="0aec6-157">String</span></span>|<span data-ttu-id="0aec6-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="0aec6-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0aec6-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0aec6-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0aec6-160">displayName</span><span class="sxs-lookup"><span data-stu-id="0aec6-160">displayName</span></span>|<span data-ttu-id="0aec6-161">String</span><span class="sxs-lookup"><span data-stu-id="0aec6-161">String</span></span>|<span data-ttu-id="0aec6-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="0aec6-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0aec6-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0aec6-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0aec6-164">version</span><span class="sxs-lookup"><span data-stu-id="0aec6-164">version</span></span>|<span data-ttu-id="0aec6-165">Int32</span><span class="sxs-lookup"><span data-stu-id="0aec6-165">Int32</span></span>|<span data-ttu-id="0aec6-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="0aec6-166">Version of the device configuration.</span></span> <span data-ttu-id="0aec6-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0aec6-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0aec6-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="0aec6-168">trustedRootCertificate</span></span>|<span data-ttu-id="0aec6-169">Binary</span><span class="sxs-lookup"><span data-stu-id="0aec6-169">Binary</span></span>|<span data-ttu-id="0aec6-170">信頼されたルート証明書</span><span class="sxs-lookup"><span data-stu-id="0aec6-170">Trusted Root Certificate</span></span>|
|<span data-ttu-id="0aec6-171">します</span><span class="sxs-lookup"><span data-stu-id="0aec6-171">certFileName</span></span>|<span data-ttu-id="0aec6-172">String</span><span class="sxs-lookup"><span data-stu-id="0aec6-172">String</span></span>|<span data-ttu-id="0aec6-173">UI に表示するファイル名です。</span><span class="sxs-lookup"><span data-stu-id="0aec6-173">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="0aec6-174">応答</span><span class="sxs-lookup"><span data-stu-id="0aec6-174">Response</span></span>
<span data-ttu-id="0aec6-175">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="0aec6-175">If successful, this method returns a `201 Created` response code and a [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0aec6-176">例</span><span class="sxs-lookup"><span data-stu-id="0aec6-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="0aec6-177">要求</span><span class="sxs-lookup"><span data-stu-id="0aec6-177">Request</span></span>
<span data-ttu-id="0aec6-178">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0aec6-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 442

{
  "@odata.type": "#microsoft.graph.androidWorkProfileTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="0aec6-179">応答</span><span class="sxs-lookup"><span data-stu-id="0aec6-179">Response</span></span>
<span data-ttu-id="0aec6-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0aec6-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 550

{
  "@odata.type": "#microsoft.graph.androidWorkProfileTrustedRootCertificate",
  "id": "37cc7454-7454-37cc-5474-cc375474cc37",
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





