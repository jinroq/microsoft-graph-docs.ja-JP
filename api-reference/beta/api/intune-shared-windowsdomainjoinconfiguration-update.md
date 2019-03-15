---
title: windowsdomainjoinconfiguration の更新
description: windowsdomainjoinconfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2e0700a630d3009520b290da269b213623bdf48a
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571663"
---
# <a name="update-windowsdomainjoinconfiguration"></a><span data-ttu-id="87322-103">windowsdomainjoinconfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="87322-103">Update windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="87322-104">**重要:** Microsoft Graph の/ベータ版の api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="87322-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="87322-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87322-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="87322-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="87322-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87322-107">[windowsdomainjoinconfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="87322-107">Update the properties of a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="87322-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="87322-108">Prerequisites</span></span>
<span data-ttu-id="87322-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="87322-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="87322-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="87322-111">Permission type</span></span>|<span data-ttu-id="87322-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="87322-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87322-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="87322-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="87322-114">&nbsp; &nbsp; **デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="87322-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="87322-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87322-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="87322-116">&nbsp;&nbsp; **登録**</span><span class="sxs-lookup"><span data-stu-id="87322-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="87322-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87322-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="87322-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="87322-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87322-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87322-119">Not supported.</span></span>|
|<span data-ttu-id="87322-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="87322-120">Application</span></span>|<span data-ttu-id="87322-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87322-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87322-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="87322-122">HTTP Request</span></span>

<span data-ttu-id="87322-123">**デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="87322-123">**Device configuration**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="87322-124">**登録**</span><span class="sxs-lookup"><span data-stu-id="87322-124">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="87322-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="87322-125">Request headers</span></span>
|<span data-ttu-id="87322-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="87322-126">Header</span></span>|<span data-ttu-id="87322-127">値</span><span class="sxs-lookup"><span data-stu-id="87322-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87322-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="87322-128">Authorization</span></span>|<span data-ttu-id="87322-129">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="87322-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87322-130">承諾</span><span class="sxs-lookup"><span data-stu-id="87322-130">Accept</span></span>|<span data-ttu-id="87322-131">application/json</span><span class="sxs-lookup"><span data-stu-id="87322-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87322-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="87322-132">Request body</span></span>
<span data-ttu-id="87322-133">要求本文で、 [windowsdomainjoinconfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="87322-133">In the request body, supply a JSON representation for the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

<span data-ttu-id="87322-134">次の表に、 [windowsdomainjoinconfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="87322-134">The following table shows the properties that are required when you create the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>

|<span data-ttu-id="87322-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="87322-135">Property</span></span>|<span data-ttu-id="87322-136">型</span><span class="sxs-lookup"><span data-stu-id="87322-136">Type</span></span>|<span data-ttu-id="87322-137">説明</span><span class="sxs-lookup"><span data-stu-id="87322-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87322-138">id</span><span class="sxs-lookup"><span data-stu-id="87322-138">id</span></span>|<span data-ttu-id="87322-139">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="87322-139">String</span></span>|<span data-ttu-id="87322-140">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="87322-140">Key of the entity.</span></span> <span data-ttu-id="87322-141">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="87322-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87322-142">**デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="87322-142">**Device configuration**</span></span>|
|<span data-ttu-id="87322-143">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="87322-143">activeDirectoryDomainName</span></span>|<span data-ttu-id="87322-144">String</span><span class="sxs-lookup"><span data-stu-id="87322-144">String</span></span>|<span data-ttu-id="87322-145">参加する Active Directory ドメイン名。</span><span class="sxs-lookup"><span data-stu-id="87322-145">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="87322-146">computernamestaticprefix</span><span class="sxs-lookup"><span data-stu-id="87322-146">computerNameStaticPrefix</span></span>|<span data-ttu-id="87322-147">String</span><span class="sxs-lookup"><span data-stu-id="87322-147">String</span></span>|<span data-ttu-id="87322-148">コンピューター名に使用する固定のプレフィックス。</span><span class="sxs-lookup"><span data-stu-id="87322-148">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="87322-149">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="87322-149">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="87322-150">Int32</span><span class="sxs-lookup"><span data-stu-id="87322-150">Int32</span></span>|<span data-ttu-id="87322-151">コンピューター名のサフィックスとして使用される動的に生成される文字。</span><span class="sxs-lookup"><span data-stu-id="87322-151">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="87322-152">有効な値は 3 ~ 14</span><span class="sxs-lookup"><span data-stu-id="87322-152">Valid values 3 to 14</span></span>|
|<span data-ttu-id="87322-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="87322-153">createdDateTime</span></span>|<span data-ttu-id="87322-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87322-154">DateTimeOffset</span></span>|<span data-ttu-id="87322-155">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="87322-155">DateTime the object was created.</span></span> <span data-ttu-id="87322-156">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="87322-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87322-157">description</span><span class="sxs-lookup"><span data-stu-id="87322-157">description</span></span>|<span data-ttu-id="87322-158">String</span><span class="sxs-lookup"><span data-stu-id="87322-158">String</span></span>|<span data-ttu-id="87322-159">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="87322-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="87322-160">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="87322-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87322-161">displayName</span><span class="sxs-lookup"><span data-stu-id="87322-161">displayName</span></span>|<span data-ttu-id="87322-162">String</span><span class="sxs-lookup"><span data-stu-id="87322-162">String</span></span>|<span data-ttu-id="87322-163">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="87322-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="87322-164">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="87322-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87322-165">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="87322-165">lastModifiedDateTime</span></span>|<span data-ttu-id="87322-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87322-166">DateTimeOffset</span></span>|<span data-ttu-id="87322-167">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="87322-167">DateTime the object was last modified.</span></span> <span data-ttu-id="87322-168">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="87322-168">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87322-169">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="87322-169">organizationalUnit</span></span>|<span data-ttu-id="87322-170">String</span><span class="sxs-lookup"><span data-stu-id="87322-170">String</span></span>|<span data-ttu-id="87322-171">コンピューターアカウントを作成する組織単位 (OU)。</span><span class="sxs-lookup"><span data-stu-id="87322-171">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="87322-172">このパラメーターが NULL の場合は、既知のコンピューターオブジェクトコンテナーがドメイン内で公開されているものとして使用されます。</span><span class="sxs-lookup"><span data-stu-id="87322-172">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="87322-173">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="87322-173">roleScopeTagIds</span></span>|<span data-ttu-id="87322-174">String collection</span><span class="sxs-lookup"><span data-stu-id="87322-174">String collection</span></span>|<span data-ttu-id="87322-175">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="87322-175">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="87322-176">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="87322-176">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87322-177">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="87322-177">supportsScopeTags</span></span>|<span data-ttu-id="87322-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="87322-178">Boolean</span></span>|<span data-ttu-id="87322-179">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="87322-179">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="87322-180">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="87322-180">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="87322-181">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="87322-181">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="87322-182">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="87322-182">This property is read-only.</span></span> <span data-ttu-id="87322-183">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="87322-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87322-184">version</span><span class="sxs-lookup"><span data-stu-id="87322-184">version</span></span>|<span data-ttu-id="87322-185">Int32</span><span class="sxs-lookup"><span data-stu-id="87322-185">Int32</span></span>|<span data-ttu-id="87322-186">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="87322-186">Version of the device configuration.</span></span> <span data-ttu-id="87322-187">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="87322-187">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



<span data-ttu-id="87322-188">注: 要求本文のプロパティのサポートは、呼び出しのコンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="87322-188">Note: Request body properties support depends on the context of the call.</span></span>  <span data-ttu-id="87322-189">すべてのプロパティがすべてのワークフローに適切なわけではありません。</span><span class="sxs-lookup"><span data-stu-id="87322-189">Not all properties are appropriate for all workflows.</span></span>

## <a name="response"></a><span data-ttu-id="87322-190">応答</span><span class="sxs-lookup"><span data-stu-id="87322-190">Response</span></span>
<span data-ttu-id="87322-191">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsdomainjoinconfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="87322-191">If successful, this method returns a `200 OK` response code and an updated [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87322-192">例</span><span class="sxs-lookup"><span data-stu-id="87322-192">Example</span></span>
### <a name="request"></a><span data-ttu-id="87322-193">要求</span><span class="sxs-lookup"><span data-stu-id="87322-193">Request</span></span>
<span data-ttu-id="87322-194">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="87322-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 344

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "computerNameStaticPrefix": "Computer Name Static Prefix value",
  "computerNameSuffixRandomCharCount": 1,
  "activeDirectoryDomainName": "Active Directory Domain Name value"
}
```

### <a name="response"></a><span data-ttu-id="87322-195">応答</span><span class="sxs-lookup"><span data-stu-id="87322-195">Response</span></span>
<span data-ttu-id="87322-196">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="87322-196">Here is an example of the response.</span></span> <span data-ttu-id="87322-197">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="87322-197">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="87322-198">実際の呼び出しによって返されるプロパティは、コンテキストに応じて異なります。</span><span class="sxs-lookup"><span data-stu-id="87322-198">Properties returned by actual calls vary according to the context.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 521

{
  "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
  "id": "40118d08-8d08-4011-088d-1140088d1140",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "computerNameStaticPrefix": "Computer Name Static Prefix value",
  "computerNameSuffixRandomCharCount": 1,
  "activeDirectoryDomainName": "Active Directory Domain Name value"
}
```



