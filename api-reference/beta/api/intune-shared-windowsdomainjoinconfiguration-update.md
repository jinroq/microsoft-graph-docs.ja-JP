---
title: WindowsDomainJoinConfiguration を更新します。
description: WindowsDomainJoinConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 20d096d4ddbdb8abdbc1cb88679c480d3a29f37e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352081"
---
# <a name="update-windowsdomainjoinconfiguration"></a><span data-ttu-id="ed263-103">WindowsDomainJoinConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="ed263-103">Update windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="ed263-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ed263-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed263-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed263-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed263-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ed263-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed263-107">[WindowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ed263-107">Update the properties of a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ed263-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ed263-108">Prerequisites</span></span>
<span data-ttu-id="ed263-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ed263-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed263-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ed263-111">Permission type</span></span>|<span data-ttu-id="ed263-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ed263-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed263-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ed263-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ed263-114">&nbsp; &nbsp; **デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="ed263-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="ed263-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed263-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="ed263-116">&nbsp; &nbsp; **登録**</span><span class="sxs-lookup"><span data-stu-id="ed263-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="ed263-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed263-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ed263-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ed263-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed263-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed263-119">Not supported.</span></span>|
|<span data-ttu-id="ed263-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ed263-120">Application</span></span>|<span data-ttu-id="ed263-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed263-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed263-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ed263-122">HTTP Request</span></span>

<span data-ttu-id="ed263-123">**デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="ed263-123">**Device configuration**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="ed263-124">**登録**</span><span class="sxs-lookup"><span data-stu-id="ed263-124">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="ed263-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed263-125">Request headers</span></span>
|<span data-ttu-id="ed263-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed263-126">Header</span></span>|<span data-ttu-id="ed263-127">値</span><span class="sxs-lookup"><span data-stu-id="ed263-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed263-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed263-128">Authorization</span></span>|<span data-ttu-id="ed263-129">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ed263-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed263-130">Accept</span><span class="sxs-lookup"><span data-stu-id="ed263-130">Accept</span></span>|<span data-ttu-id="ed263-131">application/json</span><span class="sxs-lookup"><span data-stu-id="ed263-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed263-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="ed263-132">Request body</span></span>
<span data-ttu-id="ed263-133">要求の本文に[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="ed263-133">In the request body, supply a JSON representation for the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

<span data-ttu-id="ed263-134">[WindowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="ed263-134">The following table shows the properties that are required when you create the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>

|<span data-ttu-id="ed263-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ed263-135">Property</span></span>|<span data-ttu-id="ed263-136">種類</span><span class="sxs-lookup"><span data-stu-id="ed263-136">Type</span></span>|<span data-ttu-id="ed263-137">説明</span><span class="sxs-lookup"><span data-stu-id="ed263-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed263-138">ID</span><span class="sxs-lookup"><span data-stu-id="ed263-138">id</span></span>|<span data-ttu-id="ed263-139">String</span><span class="sxs-lookup"><span data-stu-id="ed263-139">String</span></span>|<span data-ttu-id="ed263-140">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ed263-140">Key of the entity.</span></span> <span data-ttu-id="ed263-141">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ed263-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed263-142">**デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="ed263-142">**Device configuration**</span></span>|
|<span data-ttu-id="ed263-143">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="ed263-143">activeDirectoryDomainName</span></span>|<span data-ttu-id="ed263-144">String</span><span class="sxs-lookup"><span data-stu-id="ed263-144">String</span></span>|<span data-ttu-id="ed263-145">参加するアクティブなディレクトリ ドメイン名です。</span><span class="sxs-lookup"><span data-stu-id="ed263-145">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="ed263-146">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="ed263-146">computerNameStaticPrefix</span></span>|<span data-ttu-id="ed263-147">String</span><span class="sxs-lookup"><span data-stu-id="ed263-147">String</span></span>|<span data-ttu-id="ed263-148">コンピューター名に使用するプレフィックスを固定します。</span><span class="sxs-lookup"><span data-stu-id="ed263-148">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="ed263-149">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="ed263-149">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="ed263-150">Int32</span><span class="sxs-lookup"><span data-stu-id="ed263-150">Int32</span></span>|<span data-ttu-id="ed263-151">コンピューター名にサフィックスとして使用される文字を動的に生成します。</span><span class="sxs-lookup"><span data-stu-id="ed263-151">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="ed263-152">3 ~ 14 の有効な値</span><span class="sxs-lookup"><span data-stu-id="ed263-152">Valid values 3 to 14</span></span>|
|<span data-ttu-id="ed263-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ed263-153">createdDateTime</span></span>|<span data-ttu-id="ed263-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed263-154">DateTimeOffset</span></span>|<span data-ttu-id="ed263-155">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="ed263-155">DateTime the object was created.</span></span> <span data-ttu-id="ed263-156">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ed263-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed263-157">説明</span><span class="sxs-lookup"><span data-stu-id="ed263-157">description</span></span>|<span data-ttu-id="ed263-158">String</span><span class="sxs-lookup"><span data-stu-id="ed263-158">String</span></span>|<span data-ttu-id="ed263-159">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="ed263-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ed263-160">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ed263-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed263-161">displayName</span><span class="sxs-lookup"><span data-stu-id="ed263-161">displayName</span></span>|<span data-ttu-id="ed263-162">String</span><span class="sxs-lookup"><span data-stu-id="ed263-162">String</span></span>|<span data-ttu-id="ed263-163">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="ed263-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ed263-164">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ed263-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed263-165">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed263-165">lastModifiedDateTime</span></span>|<span data-ttu-id="ed263-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed263-166">DateTimeOffset</span></span>|<span data-ttu-id="ed263-167">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="ed263-167">DateTime the object was last modified.</span></span> <span data-ttu-id="ed263-168">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ed263-168">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed263-169">組織単位</span><span class="sxs-lookup"><span data-stu-id="ed263-169">organizationalUnit</span></span>|<span data-ttu-id="ed263-170">String</span><span class="sxs-lookup"><span data-stu-id="ed263-170">String</span></span>|<span data-ttu-id="ed263-171">組織単位 (OU) のコンピューター アカウントを作成する場所です。</span><span class="sxs-lookup"><span data-stu-id="ed263-171">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="ed263-172">このパラメーターが NULL の場合は、ドメインで公開されている、よく知られているコンピューター オブジェクトのコンテナーが使用されます。</span><span class="sxs-lookup"><span data-stu-id="ed263-172">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="ed263-173">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ed263-173">roleScopeTagIds</span></span>|<span data-ttu-id="ed263-174">String コレクション</span><span class="sxs-lookup"><span data-stu-id="ed263-174">String collection</span></span>|<span data-ttu-id="ed263-175">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="ed263-175">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ed263-176">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ed263-176">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed263-177">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ed263-177">supportsScopeTags</span></span>|<span data-ttu-id="ed263-178">ブール型</span><span class="sxs-lookup"><span data-stu-id="ed263-178">Boolean</span></span>|<span data-ttu-id="ed263-179">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ed263-179">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ed263-180">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="ed263-180">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ed263-181">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="ed263-181">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ed263-182">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="ed263-182">This property is read-only.</span></span> <span data-ttu-id="ed263-183">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ed263-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed263-184">version</span><span class="sxs-lookup"><span data-stu-id="ed263-184">version</span></span>|<span data-ttu-id="ed263-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ed263-185">Int32</span></span>|<span data-ttu-id="ed263-186">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="ed263-186">Version of the device configuration.</span></span> <span data-ttu-id="ed263-187">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ed263-187">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



<span data-ttu-id="ed263-188">注意: 要求の本文のプロパティのサポートは、呼び出しのコンテキストに依存します。</span><span class="sxs-lookup"><span data-stu-id="ed263-188">Note: Request body properties support depends on the context of the call.</span></span>  <span data-ttu-id="ed263-189">すべてのプロパティは、すべてのワークフローに適しています。</span><span class="sxs-lookup"><span data-stu-id="ed263-189">Not all properties are appropriate for all workflows.</span></span>

## <a name="response"></a><span data-ttu-id="ed263-190">応答</span><span class="sxs-lookup"><span data-stu-id="ed263-190">Response</span></span>
<span data-ttu-id="ed263-191">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="ed263-191">If successful, this method returns a `200 OK` response code and an updated [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed263-192">例</span><span class="sxs-lookup"><span data-stu-id="ed263-192">Example</span></span>
### <a name="request"></a><span data-ttu-id="ed263-193">要求</span><span class="sxs-lookup"><span data-stu-id="ed263-193">Request</span></span>
<span data-ttu-id="ed263-194">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ed263-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ed263-195">応答</span><span class="sxs-lookup"><span data-stu-id="ed263-195">Response</span></span>
<span data-ttu-id="ed263-196">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ed263-196">Here is an example of the response.</span></span> <span data-ttu-id="ed263-197">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="ed263-197">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ed263-198">実際の呼び出しによって返されるプロパティは、コンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="ed263-198">Properties returned by actual calls vary according to the context.</span></span>
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


