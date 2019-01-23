---
title: WindowsDomainJoinConfiguration を作成します。
description: 新しい windowsDomainJoinConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c462608c5595bbb1b0644b6e99285f87347d8065
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423210"
---
# <a name="create-windowsdomainjoinconfiguration"></a><span data-ttu-id="c83f5-103">WindowsDomainJoinConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="c83f5-103">Create windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="c83f5-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c83f5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c83f5-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c83f5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c83f5-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c83f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c83f5-107">新しい[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c83f5-107">Create a new [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c83f5-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c83f5-108">Prerequisites</span></span>
<span data-ttu-id="c83f5-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c83f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c83f5-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c83f5-111">Permission type</span></span>|<span data-ttu-id="c83f5-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c83f5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c83f5-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c83f5-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c83f5-114">&nbsp; &nbsp; **デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="c83f5-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="c83f5-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c83f5-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="c83f5-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c83f5-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c83f5-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c83f5-117">Not supported.</span></span>|
|<span data-ttu-id="c83f5-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c83f5-118">Application</span></span>|<span data-ttu-id="c83f5-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c83f5-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c83f5-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c83f5-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c83f5-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c83f5-121">Request headers</span></span>

|<span data-ttu-id="c83f5-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c83f5-122">Header</span></span>|<span data-ttu-id="c83f5-123">値</span><span class="sxs-lookup"><span data-stu-id="c83f5-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c83f5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c83f5-124">Authorization</span></span>|<span data-ttu-id="c83f5-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c83f5-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c83f5-126">Accept</span><span class="sxs-lookup"><span data-stu-id="c83f5-126">Accept</span></span>|<span data-ttu-id="c83f5-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c83f5-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c83f5-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="c83f5-128">Request body</span></span>

<span data-ttu-id="c83f5-129">要求の本文に windowsDomainJoinConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="c83f5-129">In the request body, supply a JSON representation for the windowsDomainJoinConfiguration object.</span></span>

<span data-ttu-id="c83f5-130">次の表は、windowsDomainJoinConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c83f5-130">The following table shows the properties that are required when you create the windowsDomainJoinConfiguration.</span></span>

|<span data-ttu-id="c83f5-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c83f5-131">Property</span></span>|<span data-ttu-id="c83f5-132">型</span><span class="sxs-lookup"><span data-stu-id="c83f5-132">Type</span></span>|<span data-ttu-id="c83f5-133">説明</span><span class="sxs-lookup"><span data-stu-id="c83f5-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c83f5-134">id</span><span class="sxs-lookup"><span data-stu-id="c83f5-134">id</span></span>|<span data-ttu-id="c83f5-135">String</span><span class="sxs-lookup"><span data-stu-id="c83f5-135">String</span></span>|<span data-ttu-id="c83f5-136">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c83f5-136">Key of the entity.</span></span> <span data-ttu-id="c83f5-137">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c83f5-137">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c83f5-138">**デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="c83f5-138">**Device configuration**</span></span>|
|<span data-ttu-id="c83f5-139">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="c83f5-139">activeDirectoryDomainName</span></span>|<span data-ttu-id="c83f5-140">String</span><span class="sxs-lookup"><span data-stu-id="c83f5-140">String</span></span>|<span data-ttu-id="c83f5-141">参加するアクティブなディレクトリ ドメイン名です。</span><span class="sxs-lookup"><span data-stu-id="c83f5-141">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="c83f5-142">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="c83f5-142">computerNameStaticPrefix</span></span>|<span data-ttu-id="c83f5-143">String</span><span class="sxs-lookup"><span data-stu-id="c83f5-143">String</span></span>|<span data-ttu-id="c83f5-144">コンピューター名に使用するプレフィックスを固定します。</span><span class="sxs-lookup"><span data-stu-id="c83f5-144">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="c83f5-145">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="c83f5-145">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="c83f5-146">Int32</span><span class="sxs-lookup"><span data-stu-id="c83f5-146">Int32</span></span>|<span data-ttu-id="c83f5-147">コンピューター名にサフィックスとして使用される文字を動的に生成します。</span><span class="sxs-lookup"><span data-stu-id="c83f5-147">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="c83f5-148">3 ~ 14 の有効な値</span><span class="sxs-lookup"><span data-stu-id="c83f5-148">Valid values 3 to 14</span></span>|
|<span data-ttu-id="c83f5-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c83f5-149">createdDateTime</span></span>|<span data-ttu-id="c83f5-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c83f5-150">DateTimeOffset</span></span>|<span data-ttu-id="c83f5-151">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c83f5-151">DateTime the object was created.</span></span> <span data-ttu-id="c83f5-152">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c83f5-152">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c83f5-153">説明</span><span class="sxs-lookup"><span data-stu-id="c83f5-153">description</span></span>|<span data-ttu-id="c83f5-154">String</span><span class="sxs-lookup"><span data-stu-id="c83f5-154">String</span></span>|<span data-ttu-id="c83f5-155">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="c83f5-155">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c83f5-156">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c83f5-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c83f5-157">displayName</span><span class="sxs-lookup"><span data-stu-id="c83f5-157">displayName</span></span>|<span data-ttu-id="c83f5-158">String</span><span class="sxs-lookup"><span data-stu-id="c83f5-158">String</span></span>|<span data-ttu-id="c83f5-159">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="c83f5-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c83f5-160">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c83f5-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c83f5-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c83f5-161">lastModifiedDateTime</span></span>|<span data-ttu-id="c83f5-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c83f5-162">DateTimeOffset</span></span>|<span data-ttu-id="c83f5-163">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c83f5-163">DateTime the object was last modified.</span></span> <span data-ttu-id="c83f5-164">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c83f5-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c83f5-165">組織単位</span><span class="sxs-lookup"><span data-stu-id="c83f5-165">organizationalUnit</span></span>|<span data-ttu-id="c83f5-166">String</span><span class="sxs-lookup"><span data-stu-id="c83f5-166">String</span></span>|<span data-ttu-id="c83f5-167">組織単位 (OU) のコンピューター アカウントを作成する場所です。</span><span class="sxs-lookup"><span data-stu-id="c83f5-167">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="c83f5-168">このパラメーターが NULL の場合は、ドメインで公開されている、よく知られているコンピューター オブジェクトのコンテナーが使用されます。</span><span class="sxs-lookup"><span data-stu-id="c83f5-168">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="c83f5-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c83f5-169">roleScopeTagIds</span></span>|<span data-ttu-id="c83f5-170">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c83f5-170">String collection</span></span>|<span data-ttu-id="c83f5-171">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="c83f5-171">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c83f5-172">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c83f5-172">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c83f5-173">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c83f5-173">supportsScopeTags</span></span>|<span data-ttu-id="c83f5-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="c83f5-174">Boolean</span></span>|<span data-ttu-id="c83f5-175">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c83f5-175">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c83f5-176">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="c83f5-176">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c83f5-177">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="c83f5-177">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c83f5-178">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="c83f5-178">This property is read-only.</span></span> <span data-ttu-id="c83f5-179">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c83f5-179">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c83f5-180">version</span><span class="sxs-lookup"><span data-stu-id="c83f5-180">version</span></span>|<span data-ttu-id="c83f5-181">Int32</span><span class="sxs-lookup"><span data-stu-id="c83f5-181">Int32</span></span>|<span data-ttu-id="c83f5-182">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="c83f5-182">Version of the device configuration.</span></span> <span data-ttu-id="c83f5-183">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c83f5-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="c83f5-184">応答</span><span class="sxs-lookup"><span data-stu-id="c83f5-184">Response</span></span>

<span data-ttu-id="c83f5-185">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c83f5-185">If successful, this method returns a `201 Created` response code and a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c83f5-186">例</span><span class="sxs-lookup"><span data-stu-id="c83f5-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="c83f5-187">要求</span><span class="sxs-lookup"><span data-stu-id="c83f5-187">Request</span></span>

<span data-ttu-id="c83f5-188">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c83f5-188">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 559

{
  "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "computerNameStaticPrefix": "Computer Name Static Prefix value",
  "computerNameSuffixRandomCharCount": 1,
  "activeDirectoryDomainName": "Active Directory Domain Name value",
  "organizationalUnit": "Organizational Unit value"
}
```

### <a name="response"></a><span data-ttu-id="c83f5-189">応答</span><span class="sxs-lookup"><span data-stu-id="c83f5-189">Response</span></span>

<span data-ttu-id="c83f5-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c83f5-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 667

{
  "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
  "id": "40118d08-8d08-4011-088d-1140088d1140",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "computerNameStaticPrefix": "Computer Name Static Prefix value",
  "computerNameSuffixRandomCharCount": 1,
  "activeDirectoryDomainName": "Active Directory Domain Name value",
  "organizationalUnit": "Organizational Unit value"
}
```



