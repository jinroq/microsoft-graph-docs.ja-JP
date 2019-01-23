---
title: AndroidWorkProfileTrustedRootCertificate を作成します。
description: 新しい androidWorkProfileTrustedRootCertificate オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fc819fb720d6620f03abd9cdb011cde8f71a86f5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424477"
---
# <a name="create-androidworkprofiletrustedrootcertificate"></a><span data-ttu-id="3e94e-103">AndroidWorkProfileTrustedRootCertificate を作成します。</span><span class="sxs-lookup"><span data-stu-id="3e94e-103">Create androidWorkProfileTrustedRootCertificate</span></span>

> <span data-ttu-id="3e94e-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3e94e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3e94e-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3e94e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3e94e-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3e94e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e94e-107">新しい[androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3e94e-107">Create a new [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e94e-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="3e94e-108">Prerequisites</span></span>
<span data-ttu-id="3e94e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3e94e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3e94e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3e94e-111">Permission type</span></span>|<span data-ttu-id="3e94e-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3e94e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e94e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3e94e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3e94e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e94e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3e94e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3e94e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e94e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3e94e-116">Not supported.</span></span>|
|<span data-ttu-id="3e94e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3e94e-117">Application</span></span>|<span data-ttu-id="3e94e-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3e94e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e94e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3e94e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3e94e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3e94e-120">Request headers</span></span>
|<span data-ttu-id="3e94e-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3e94e-121">Header</span></span>|<span data-ttu-id="3e94e-122">値</span><span class="sxs-lookup"><span data-stu-id="3e94e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e94e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e94e-123">Authorization</span></span>|<span data-ttu-id="3e94e-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3e94e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e94e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3e94e-125">Accept</span></span>|<span data-ttu-id="3e94e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3e94e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e94e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3e94e-127">Request body</span></span>
<span data-ttu-id="3e94e-128">要求の本文に androidWorkProfileTrustedRootCertificate オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="3e94e-128">In the request body, supply a JSON representation for the androidWorkProfileTrustedRootCertificate object.</span></span>

<span data-ttu-id="3e94e-129">次の表は、androidWorkProfileTrustedRootCertificate を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3e94e-129">The following table shows the properties that are required when you create the androidWorkProfileTrustedRootCertificate.</span></span>

|<span data-ttu-id="3e94e-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3e94e-130">Property</span></span>|<span data-ttu-id="3e94e-131">型</span><span class="sxs-lookup"><span data-stu-id="3e94e-131">Type</span></span>|<span data-ttu-id="3e94e-132">説明</span><span class="sxs-lookup"><span data-stu-id="3e94e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e94e-133">id</span><span class="sxs-lookup"><span data-stu-id="3e94e-133">id</span></span>|<span data-ttu-id="3e94e-134">String</span><span class="sxs-lookup"><span data-stu-id="3e94e-134">String</span></span>|<span data-ttu-id="3e94e-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3e94e-135">Key of the entity.</span></span> <span data-ttu-id="3e94e-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3e94e-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e94e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e94e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3e94e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e94e-138">DateTimeOffset</span></span>|<span data-ttu-id="3e94e-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="3e94e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3e94e-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3e94e-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e94e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3e94e-141">roleScopeTagIds</span></span>|<span data-ttu-id="3e94e-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="3e94e-142">String collection</span></span>|<span data-ttu-id="3e94e-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="3e94e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3e94e-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3e94e-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e94e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3e94e-145">supportsScopeTags</span></span>|<span data-ttu-id="3e94e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e94e-146">Boolean</span></span>|<span data-ttu-id="3e94e-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3e94e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3e94e-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="3e94e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3e94e-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="3e94e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3e94e-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="3e94e-150">This property is read-only.</span></span> <span data-ttu-id="3e94e-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3e94e-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e94e-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3e94e-152">createdDateTime</span></span>|<span data-ttu-id="3e94e-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e94e-153">DateTimeOffset</span></span>|<span data-ttu-id="3e94e-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="3e94e-154">DateTime the object was created.</span></span> <span data-ttu-id="3e94e-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3e94e-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e94e-156">説明</span><span class="sxs-lookup"><span data-stu-id="3e94e-156">description</span></span>|<span data-ttu-id="3e94e-157">String</span><span class="sxs-lookup"><span data-stu-id="3e94e-157">String</span></span>|<span data-ttu-id="3e94e-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="3e94e-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3e94e-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3e94e-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e94e-160">displayName</span><span class="sxs-lookup"><span data-stu-id="3e94e-160">displayName</span></span>|<span data-ttu-id="3e94e-161">String</span><span class="sxs-lookup"><span data-stu-id="3e94e-161">String</span></span>|<span data-ttu-id="3e94e-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="3e94e-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3e94e-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3e94e-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e94e-164">version</span><span class="sxs-lookup"><span data-stu-id="3e94e-164">version</span></span>|<span data-ttu-id="3e94e-165">Int32</span><span class="sxs-lookup"><span data-stu-id="3e94e-165">Int32</span></span>|<span data-ttu-id="3e94e-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="3e94e-166">Version of the device configuration.</span></span> <span data-ttu-id="3e94e-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3e94e-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e94e-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="3e94e-168">trustedRootCertificate</span></span>|<span data-ttu-id="3e94e-169">Binary</span><span class="sxs-lookup"><span data-stu-id="3e94e-169">Binary</span></span>|<span data-ttu-id="3e94e-170">信頼されたルート証明書</span><span class="sxs-lookup"><span data-stu-id="3e94e-170">Trusted Root Certificate</span></span>|
|<span data-ttu-id="3e94e-171">します</span><span class="sxs-lookup"><span data-stu-id="3e94e-171">certFileName</span></span>|<span data-ttu-id="3e94e-172">String</span><span class="sxs-lookup"><span data-stu-id="3e94e-172">String</span></span>|<span data-ttu-id="3e94e-173">UI に表示するファイル名です。</span><span class="sxs-lookup"><span data-stu-id="3e94e-173">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="3e94e-174">応答</span><span class="sxs-lookup"><span data-stu-id="3e94e-174">Response</span></span>
<span data-ttu-id="3e94e-175">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="3e94e-175">If successful, this method returns a `201 Created` response code and a [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e94e-176">例</span><span class="sxs-lookup"><span data-stu-id="3e94e-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e94e-177">要求</span><span class="sxs-lookup"><span data-stu-id="3e94e-177">Request</span></span>
<span data-ttu-id="3e94e-178">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3e94e-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 378

{
  "@odata.type": "#microsoft.graph.androidWorkProfileTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="3e94e-179">応答</span><span class="sxs-lookup"><span data-stu-id="3e94e-179">Response</span></span>
<span data-ttu-id="3e94e-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3e94e-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




