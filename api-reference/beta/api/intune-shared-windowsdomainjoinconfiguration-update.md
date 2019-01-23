---
title: WindowsDomainJoinConfiguration を更新します。
description: WindowsDomainJoinConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 66314179f65748abca432dcf4f41bab3c16ebd32
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410855"
---
# <a name="update-windowsdomainjoinconfiguration"></a><span data-ttu-id="d650a-103">WindowsDomainJoinConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="d650a-103">Update windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="d650a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d650a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d650a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d650a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d650a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d650a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d650a-107">[WindowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d650a-107">Update the properties of a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d650a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="d650a-108">Prerequisites</span></span>
<span data-ttu-id="d650a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d650a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d650a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d650a-111">Permission type</span></span>|<span data-ttu-id="d650a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d650a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d650a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d650a-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d650a-114">&nbsp; &nbsp; **デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="d650a-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d650a-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d650a-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="d650a-116">&nbsp; &nbsp; **登録**</span><span class="sxs-lookup"><span data-stu-id="d650a-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="d650a-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d650a-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d650a-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d650a-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d650a-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d650a-119">Not supported.</span></span>|
|<span data-ttu-id="d650a-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d650a-120">Application</span></span>|<span data-ttu-id="d650a-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d650a-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d650a-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d650a-122">HTTP Request</span></span>

<span data-ttu-id="d650a-123">**デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="d650a-123">**Device configuration**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="d650a-124">**登録**</span><span class="sxs-lookup"><span data-stu-id="d650a-124">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="d650a-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d650a-125">Request headers</span></span>
|<span data-ttu-id="d650a-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d650a-126">Header</span></span>|<span data-ttu-id="d650a-127">値</span><span class="sxs-lookup"><span data-stu-id="d650a-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d650a-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="d650a-128">Authorization</span></span>|<span data-ttu-id="d650a-129">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d650a-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d650a-130">Accept</span><span class="sxs-lookup"><span data-stu-id="d650a-130">Accept</span></span>|<span data-ttu-id="d650a-131">application/json</span><span class="sxs-lookup"><span data-stu-id="d650a-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d650a-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="d650a-132">Request body</span></span>
<span data-ttu-id="d650a-133">要求の本文に[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="d650a-133">In the request body, supply a JSON representation for the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

<span data-ttu-id="d650a-134">[WindowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="d650a-134">The following table shows the properties that are required when you create the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>

|<span data-ttu-id="d650a-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d650a-135">Property</span></span>|<span data-ttu-id="d650a-136">型</span><span class="sxs-lookup"><span data-stu-id="d650a-136">Type</span></span>|<span data-ttu-id="d650a-137">説明</span><span class="sxs-lookup"><span data-stu-id="d650a-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d650a-138">id</span><span class="sxs-lookup"><span data-stu-id="d650a-138">id</span></span>|<span data-ttu-id="d650a-139">String</span><span class="sxs-lookup"><span data-stu-id="d650a-139">String</span></span>|<span data-ttu-id="d650a-140">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d650a-140">Key of the entity.</span></span> <span data-ttu-id="d650a-141">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d650a-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d650a-142">**デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="d650a-142">**Device configuration**</span></span>|
|<span data-ttu-id="d650a-143">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="d650a-143">activeDirectoryDomainName</span></span>|<span data-ttu-id="d650a-144">String</span><span class="sxs-lookup"><span data-stu-id="d650a-144">String</span></span>|<span data-ttu-id="d650a-145">参加するアクティブなディレクトリ ドメイン名です。</span><span class="sxs-lookup"><span data-stu-id="d650a-145">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="d650a-146">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="d650a-146">computerNameStaticPrefix</span></span>|<span data-ttu-id="d650a-147">String</span><span class="sxs-lookup"><span data-stu-id="d650a-147">String</span></span>|<span data-ttu-id="d650a-148">コンピューター名に使用するプレフィックスを固定します。</span><span class="sxs-lookup"><span data-stu-id="d650a-148">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="d650a-149">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="d650a-149">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="d650a-150">Int32</span><span class="sxs-lookup"><span data-stu-id="d650a-150">Int32</span></span>|<span data-ttu-id="d650a-151">コンピューター名にサフィックスとして使用される文字を動的に生成します。</span><span class="sxs-lookup"><span data-stu-id="d650a-151">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="d650a-152">3 ~ 14 の有効な値</span><span class="sxs-lookup"><span data-stu-id="d650a-152">Valid values 3 to 14</span></span>|
|<span data-ttu-id="d650a-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d650a-153">createdDateTime</span></span>|<span data-ttu-id="d650a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d650a-154">DateTimeOffset</span></span>|<span data-ttu-id="d650a-155">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d650a-155">DateTime the object was created.</span></span> <span data-ttu-id="d650a-156">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d650a-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d650a-157">説明</span><span class="sxs-lookup"><span data-stu-id="d650a-157">description</span></span>|<span data-ttu-id="d650a-158">String</span><span class="sxs-lookup"><span data-stu-id="d650a-158">String</span></span>|<span data-ttu-id="d650a-159">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="d650a-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d650a-160">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d650a-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d650a-161">displayName</span><span class="sxs-lookup"><span data-stu-id="d650a-161">displayName</span></span>|<span data-ttu-id="d650a-162">String</span><span class="sxs-lookup"><span data-stu-id="d650a-162">String</span></span>|<span data-ttu-id="d650a-163">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="d650a-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d650a-164">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d650a-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d650a-165">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d650a-165">lastModifiedDateTime</span></span>|<span data-ttu-id="d650a-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d650a-166">DateTimeOffset</span></span>|<span data-ttu-id="d650a-167">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d650a-167">DateTime the object was last modified.</span></span> <span data-ttu-id="d650a-168">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d650a-168">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d650a-169">組織単位</span><span class="sxs-lookup"><span data-stu-id="d650a-169">organizationalUnit</span></span>|<span data-ttu-id="d650a-170">String</span><span class="sxs-lookup"><span data-stu-id="d650a-170">String</span></span>|<span data-ttu-id="d650a-171">組織単位 (OU) のコンピューター アカウントを作成する場所です。</span><span class="sxs-lookup"><span data-stu-id="d650a-171">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="d650a-172">このパラメーターが NULL の場合は、ドメインで公開されている、よく知られているコンピューター オブジェクトのコンテナーが使用されます。</span><span class="sxs-lookup"><span data-stu-id="d650a-172">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="d650a-173">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d650a-173">roleScopeTagIds</span></span>|<span data-ttu-id="d650a-174">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d650a-174">String collection</span></span>|<span data-ttu-id="d650a-175">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="d650a-175">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d650a-176">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d650a-176">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d650a-177">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d650a-177">supportsScopeTags</span></span>|<span data-ttu-id="d650a-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="d650a-178">Boolean</span></span>|<span data-ttu-id="d650a-179">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d650a-179">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d650a-180">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="d650a-180">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d650a-181">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="d650a-181">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d650a-182">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="d650a-182">This property is read-only.</span></span> <span data-ttu-id="d650a-183">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d650a-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d650a-184">version</span><span class="sxs-lookup"><span data-stu-id="d650a-184">version</span></span>|<span data-ttu-id="d650a-185">Int32</span><span class="sxs-lookup"><span data-stu-id="d650a-185">Int32</span></span>|<span data-ttu-id="d650a-186">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="d650a-186">Version of the device configuration.</span></span> <span data-ttu-id="d650a-187">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d650a-187">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



<span data-ttu-id="d650a-188">注意: 要求の本文のプロパティのサポートは、呼び出しのコンテキストに依存します。</span><span class="sxs-lookup"><span data-stu-id="d650a-188">Note: Request body properties support depends on the context of the call.</span></span>  <span data-ttu-id="d650a-189">すべてのプロパティは、すべてのワークフローに適しています。</span><span class="sxs-lookup"><span data-stu-id="d650a-189">Not all properties are appropriate for all workflows.</span></span>

## <a name="response"></a><span data-ttu-id="d650a-190">応答</span><span class="sxs-lookup"><span data-stu-id="d650a-190">Response</span></span>
<span data-ttu-id="d650a-191">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="d650a-191">If successful, this method returns a `200 OK` response code and an updated [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d650a-192">例</span><span class="sxs-lookup"><span data-stu-id="d650a-192">Example</span></span>
### <a name="request"></a><span data-ttu-id="d650a-193">要求</span><span class="sxs-lookup"><span data-stu-id="d650a-193">Request</span></span>
<span data-ttu-id="d650a-194">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d650a-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d650a-195">応答</span><span class="sxs-lookup"><span data-stu-id="d650a-195">Response</span></span>
<span data-ttu-id="d650a-196">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d650a-196">Here is an example of the response.</span></span> <span data-ttu-id="d650a-197">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="d650a-197">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d650a-198">実際の呼び出しによって返されるプロパティは、コンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="d650a-198">Properties returned by actual calls vary according to the context.</span></span>
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



