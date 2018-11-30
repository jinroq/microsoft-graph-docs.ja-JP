---
title: WindowsDomainJoinConfiguration を作成します。
description: 新しい windowsDomainJoinConfiguration オブジェクトを作成します。
ms.openlocfilehash: 8069dfac727ee24d96f72875a4cec19fa42b8baa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073795"
---
# <a name="create-windowsdomainjoinconfiguration"></a><span data-ttu-id="fe473-103">WindowsDomainJoinConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="fe473-103">Create windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="fe473-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fe473-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe473-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe473-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fe473-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fe473-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe473-107">新しい[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="fe473-107">Create a new [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fe473-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="fe473-108">Prerequisites</span></span>
<span data-ttu-id="fe473-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe473-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe473-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fe473-111">Permission type</span></span>|<span data-ttu-id="fe473-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fe473-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe473-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fe473-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fe473-114">&nbsp; &nbsp; **デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="fe473-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="fe473-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe473-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="fe473-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fe473-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe473-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe473-117">Not supported.</span></span>|
|<span data-ttu-id="fe473-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fe473-118">Application</span></span>|<span data-ttu-id="fe473-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe473-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe473-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fe473-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fe473-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fe473-121">Request headers</span></span>

|<span data-ttu-id="fe473-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fe473-122">Header</span></span>|<span data-ttu-id="fe473-123">値</span><span class="sxs-lookup"><span data-stu-id="fe473-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe473-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe473-124">Authorization</span></span>|<span data-ttu-id="fe473-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="fe473-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe473-126">Accept</span><span class="sxs-lookup"><span data-stu-id="fe473-126">Accept</span></span>|<span data-ttu-id="fe473-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fe473-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe473-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="fe473-128">Request body</span></span>

<span data-ttu-id="fe473-129">要求の本文に windowsDomainJoinConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="fe473-129">In the request body, supply a JSON representation for the windowsDomainJoinConfiguration object.</span></span>

<span data-ttu-id="fe473-130">次の表は、windowsDomainJoinConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="fe473-130">The following table shows the properties that are required when you create the windowsDomainJoinConfiguration.</span></span>

|<span data-ttu-id="fe473-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe473-131">Property</span></span>|<span data-ttu-id="fe473-132">型</span><span class="sxs-lookup"><span data-stu-id="fe473-132">Type</span></span>|<span data-ttu-id="fe473-133">説明</span><span class="sxs-lookup"><span data-stu-id="fe473-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe473-134">id</span><span class="sxs-lookup"><span data-stu-id="fe473-134">id</span></span>|<span data-ttu-id="fe473-135">String</span><span class="sxs-lookup"><span data-stu-id="fe473-135">String</span></span>|<span data-ttu-id="fe473-136">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="fe473-136">Key of the entity.</span></span> <span data-ttu-id="fe473-137">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe473-137">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe473-138">**デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="fe473-138">**Device configuration**</span></span>|
|<span data-ttu-id="fe473-139">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="fe473-139">activeDirectoryDomainName</span></span>|<span data-ttu-id="fe473-140">String</span><span class="sxs-lookup"><span data-stu-id="fe473-140">String</span></span>|<span data-ttu-id="fe473-141">参加するアクティブなディレクトリ ドメイン名です。</span><span class="sxs-lookup"><span data-stu-id="fe473-141">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="fe473-142">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="fe473-142">computerNameStaticPrefix</span></span>|<span data-ttu-id="fe473-143">String</span><span class="sxs-lookup"><span data-stu-id="fe473-143">String</span></span>|<span data-ttu-id="fe473-144">コンピューター名に使用するプレフィックスを固定します。</span><span class="sxs-lookup"><span data-stu-id="fe473-144">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="fe473-145">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="fe473-145">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="fe473-146">Int32</span><span class="sxs-lookup"><span data-stu-id="fe473-146">Int32</span></span>|<span data-ttu-id="fe473-147">コンピューター名にサフィックスとして使用される文字を動的に生成します。</span><span class="sxs-lookup"><span data-stu-id="fe473-147">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="fe473-148">3 ~ 14 の有効な値</span><span class="sxs-lookup"><span data-stu-id="fe473-148">Valid values 3 to 14</span></span>|
|<span data-ttu-id="fe473-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fe473-149">createdDateTime</span></span>|<span data-ttu-id="fe473-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe473-150">DateTimeOffset</span></span>|<span data-ttu-id="fe473-151">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="fe473-151">DateTime the object was created.</span></span> <span data-ttu-id="fe473-152">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe473-152">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe473-153">説明</span><span class="sxs-lookup"><span data-stu-id="fe473-153">description</span></span>|<span data-ttu-id="fe473-154">String</span><span class="sxs-lookup"><span data-stu-id="fe473-154">String</span></span>|<span data-ttu-id="fe473-155">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="fe473-155">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fe473-156">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe473-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe473-157">displayName</span><span class="sxs-lookup"><span data-stu-id="fe473-157">displayName</span></span>|<span data-ttu-id="fe473-158">String</span><span class="sxs-lookup"><span data-stu-id="fe473-158">String</span></span>|<span data-ttu-id="fe473-159">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="fe473-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fe473-160">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe473-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe473-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe473-161">lastModifiedDateTime</span></span>|<span data-ttu-id="fe473-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe473-162">DateTimeOffset</span></span>|<span data-ttu-id="fe473-163">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="fe473-163">DateTime the object was last modified.</span></span> <span data-ttu-id="fe473-164">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe473-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe473-165">組織単位</span><span class="sxs-lookup"><span data-stu-id="fe473-165">organizationalUnit</span></span>|<span data-ttu-id="fe473-166">String</span><span class="sxs-lookup"><span data-stu-id="fe473-166">String</span></span>|<span data-ttu-id="fe473-167">組織単位 (OU) のコンピューター アカウントを作成する場所です。</span><span class="sxs-lookup"><span data-stu-id="fe473-167">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="fe473-168">このパラメーターが NULL の場合は、ドメインで公開されている、よく知られているコンピューター オブジェクトのコンテナーが使用されます。</span><span class="sxs-lookup"><span data-stu-id="fe473-168">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="fe473-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fe473-169">roleScopeTagIds</span></span>|<span data-ttu-id="fe473-170">String コレクション</span><span class="sxs-lookup"><span data-stu-id="fe473-170">String collection</span></span>|<span data-ttu-id="fe473-171">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="fe473-171">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fe473-172">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe473-172">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe473-173">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fe473-173">supportsScopeTags</span></span>|<span data-ttu-id="fe473-174">ブール値</span><span class="sxs-lookup"><span data-stu-id="fe473-174">Boolean</span></span>|<span data-ttu-id="fe473-175">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fe473-175">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fe473-176">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="fe473-176">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fe473-177">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="fe473-177">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fe473-178">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="fe473-178">This property is read-only.</span></span> <span data-ttu-id="fe473-179">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe473-179">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe473-180">version</span><span class="sxs-lookup"><span data-stu-id="fe473-180">version</span></span>|<span data-ttu-id="fe473-181">Int32</span><span class="sxs-lookup"><span data-stu-id="fe473-181">Int32</span></span>|<span data-ttu-id="fe473-182">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="fe473-182">Version of the device configuration.</span></span> <span data-ttu-id="fe473-183">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe473-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="fe473-184">応答</span><span class="sxs-lookup"><span data-stu-id="fe473-184">Response</span></span>

<span data-ttu-id="fe473-185">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="fe473-185">If successful, this method returns a `201 Created` response code and a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe473-186">例</span><span class="sxs-lookup"><span data-stu-id="fe473-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe473-187">要求</span><span class="sxs-lookup"><span data-stu-id="fe473-187">Request</span></span>

<span data-ttu-id="fe473-188">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fe473-188">Here is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="fe473-189">応答</span><span class="sxs-lookup"><span data-stu-id="fe473-189">Response</span></span>

<span data-ttu-id="fe473-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fe473-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



