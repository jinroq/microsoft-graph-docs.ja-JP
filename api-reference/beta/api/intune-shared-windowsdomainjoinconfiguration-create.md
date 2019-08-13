---
title: WindowsDomainJoinConfiguration の作成
description: 新しい windowsDomainJoinConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a11a58f8edf38225ddbd01edfa4c55457840ac9e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350539"
---
# <a name="create-windowsdomainjoinconfiguration"></a><span data-ttu-id="20d1b-103">WindowsDomainJoinConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="20d1b-103">Create windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="20d1b-104">**重要:** Microsoft Graph の/ベータ版の Api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="20d1b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="20d1b-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20d1b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="20d1b-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="20d1b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20d1b-107">新しい[Windowsdomainjoinconfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="20d1b-107">Create a new [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="20d1b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="20d1b-108">Prerequisites</span></span>
<span data-ttu-id="20d1b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="20d1b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20d1b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="20d1b-111">Permission type</span></span>|<span data-ttu-id="20d1b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="20d1b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20d1b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="20d1b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="20d1b-114">&nbsp; &nbsp; **デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="20d1b-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="20d1b-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20d1b-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="20d1b-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="20d1b-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20d1b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20d1b-117">Not supported.</span></span>|
|<span data-ttu-id="20d1b-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="20d1b-118">Application</span></span>|<span data-ttu-id="20d1b-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20d1b-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20d1b-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="20d1b-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="20d1b-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="20d1b-121">Request headers</span></span>

|<span data-ttu-id="20d1b-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="20d1b-122">Header</span></span>|<span data-ttu-id="20d1b-123">値</span><span class="sxs-lookup"><span data-stu-id="20d1b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20d1b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="20d1b-124">Authorization</span></span>|<span data-ttu-id="20d1b-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="20d1b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20d1b-126">承諾</span><span class="sxs-lookup"><span data-stu-id="20d1b-126">Accept</span></span>|<span data-ttu-id="20d1b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="20d1b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20d1b-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="20d1b-128">Request body</span></span>

<span data-ttu-id="20d1b-129">要求本文で、windowsDomainJoinConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="20d1b-129">In the request body, supply a JSON representation for the windowsDomainJoinConfiguration object.</span></span>

<span data-ttu-id="20d1b-130">次の表に、windowsDomainJoinConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="20d1b-130">The following table shows the properties that are required when you create the windowsDomainJoinConfiguration.</span></span>

|<span data-ttu-id="20d1b-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="20d1b-131">Property</span></span>|<span data-ttu-id="20d1b-132">型</span><span class="sxs-lookup"><span data-stu-id="20d1b-132">Type</span></span>|<span data-ttu-id="20d1b-133">説明</span><span class="sxs-lookup"><span data-stu-id="20d1b-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20d1b-134">id</span><span class="sxs-lookup"><span data-stu-id="20d1b-134">id</span></span>|<span data-ttu-id="20d1b-135">文字列</span><span class="sxs-lookup"><span data-stu-id="20d1b-135">String</span></span>|<span data-ttu-id="20d1b-136">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="20d1b-136">Key of the entity.</span></span> <span data-ttu-id="20d1b-137">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20d1b-137">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20d1b-138">**デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="20d1b-138">**Device configuration**</span></span>|
|<span data-ttu-id="20d1b-139">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="20d1b-139">activeDirectoryDomainName</span></span>|<span data-ttu-id="20d1b-140">String</span><span class="sxs-lookup"><span data-stu-id="20d1b-140">String</span></span>|<span data-ttu-id="20d1b-141">参加する Active Directory ドメイン名。</span><span class="sxs-lookup"><span data-stu-id="20d1b-141">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="20d1b-142">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="20d1b-142">computerNameStaticPrefix</span></span>|<span data-ttu-id="20d1b-143">String</span><span class="sxs-lookup"><span data-stu-id="20d1b-143">String</span></span>|<span data-ttu-id="20d1b-144">コンピューター名に使用する固定のプレフィックス。</span><span class="sxs-lookup"><span data-stu-id="20d1b-144">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="20d1b-145">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="20d1b-145">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="20d1b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="20d1b-146">Int32</span></span>|<span data-ttu-id="20d1b-147">コンピューター名のサフィックスとして使用される動的に生成される文字。</span><span class="sxs-lookup"><span data-stu-id="20d1b-147">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="20d1b-148">有効な値は 3 ~ 14</span><span class="sxs-lookup"><span data-stu-id="20d1b-148">Valid values 3 to 14</span></span>|
|<span data-ttu-id="20d1b-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="20d1b-149">createdDateTime</span></span>|<span data-ttu-id="20d1b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20d1b-150">DateTimeOffset</span></span>|<span data-ttu-id="20d1b-151">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="20d1b-151">DateTime the object was created.</span></span> <span data-ttu-id="20d1b-152">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20d1b-152">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20d1b-153">description</span><span class="sxs-lookup"><span data-stu-id="20d1b-153">description</span></span>|<span data-ttu-id="20d1b-154">String</span><span class="sxs-lookup"><span data-stu-id="20d1b-154">String</span></span>|<span data-ttu-id="20d1b-155">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="20d1b-155">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="20d1b-156">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20d1b-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20d1b-157">displayName</span><span class="sxs-lookup"><span data-stu-id="20d1b-157">displayName</span></span>|<span data-ttu-id="20d1b-158">String</span><span class="sxs-lookup"><span data-stu-id="20d1b-158">String</span></span>|<span data-ttu-id="20d1b-159">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="20d1b-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="20d1b-160">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20d1b-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20d1b-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="20d1b-161">lastModifiedDateTime</span></span>|<span data-ttu-id="20d1b-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20d1b-162">DateTimeOffset</span></span>|<span data-ttu-id="20d1b-163">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="20d1b-163">DateTime the object was last modified.</span></span> <span data-ttu-id="20d1b-164">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20d1b-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20d1b-165">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="20d1b-165">organizationalUnit</span></span>|<span data-ttu-id="20d1b-166">String</span><span class="sxs-lookup"><span data-stu-id="20d1b-166">String</span></span>|<span data-ttu-id="20d1b-167">コンピューターアカウントを作成する組織単位 (OU)。</span><span class="sxs-lookup"><span data-stu-id="20d1b-167">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="20d1b-168">このパラメーターが NULL の場合は、既知のコンピューターオブジェクトコンテナーがドメイン内で公開されているものとして使用されます。</span><span class="sxs-lookup"><span data-stu-id="20d1b-168">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="20d1b-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="20d1b-169">roleScopeTagIds</span></span>|<span data-ttu-id="20d1b-170">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="20d1b-170">String collection</span></span>|<span data-ttu-id="20d1b-171">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="20d1b-171">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="20d1b-172">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20d1b-172">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20d1b-173">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="20d1b-173">supportsScopeTags</span></span>|<span data-ttu-id="20d1b-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="20d1b-174">Boolean</span></span>|<span data-ttu-id="20d1b-175">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="20d1b-175">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="20d1b-176">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="20d1b-176">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="20d1b-177">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="20d1b-177">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="20d1b-178">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="20d1b-178">This property is read-only.</span></span> <span data-ttu-id="20d1b-179">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20d1b-179">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20d1b-180">version</span><span class="sxs-lookup"><span data-stu-id="20d1b-180">version</span></span>|<span data-ttu-id="20d1b-181">Int32</span><span class="sxs-lookup"><span data-stu-id="20d1b-181">Int32</span></span>|<span data-ttu-id="20d1b-182">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="20d1b-182">Version of the device configuration.</span></span> <span data-ttu-id="20d1b-183">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20d1b-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="20d1b-184">応答</span><span class="sxs-lookup"><span data-stu-id="20d1b-184">Response</span></span>

<span data-ttu-id="20d1b-185">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Windowsdomainjoinconfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="20d1b-185">If successful, this method returns a `201 Created` response code and a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20d1b-186">例</span><span class="sxs-lookup"><span data-stu-id="20d1b-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="20d1b-187">要求</span><span class="sxs-lookup"><span data-stu-id="20d1b-187">Request</span></span>

<span data-ttu-id="20d1b-188">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="20d1b-188">Here is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="20d1b-189">応答</span><span class="sxs-lookup"><span data-stu-id="20d1b-189">Response</span></span>

<span data-ttu-id="20d1b-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="20d1b-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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






