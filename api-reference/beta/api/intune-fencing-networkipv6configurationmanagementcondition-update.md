---
title: NetworkIPv6ConfigurationManagementCondition の更新
description: NetworkIPv6ConfigurationManagementCondition オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f0bc8e40a005322e10bc9929ee847799f058743c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33905302"
---
# <a name="update-networkipv6configurationmanagementcondition"></a><span data-ttu-id="d2396-103">NetworkIPv6ConfigurationManagementCondition の更新</span><span class="sxs-lookup"><span data-stu-id="d2396-103">Update networkIPv6ConfigurationManagementCondition</span></span>

> <span data-ttu-id="d2396-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2396-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2396-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d2396-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2396-106">[NetworkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d2396-106">Update the properties of a [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2396-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d2396-107">Prerequisites</span></span>
<span data-ttu-id="d2396-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d2396-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2396-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d2396-110">Permission type</span></span>|<span data-ttu-id="d2396-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d2396-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2396-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d2396-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d2396-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2396-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d2396-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d2396-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2396-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2396-115">Not supported.</span></span>|
|<span data-ttu-id="d2396-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d2396-116">Application</span></span>|<span data-ttu-id="d2396-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2396-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2396-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d2396-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="d2396-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2396-119">Request headers</span></span>
|<span data-ttu-id="d2396-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2396-120">Header</span></span>|<span data-ttu-id="d2396-121">値</span><span class="sxs-lookup"><span data-stu-id="d2396-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2396-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2396-122">Authorization</span></span>|<span data-ttu-id="d2396-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d2396-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2396-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d2396-124">Accept</span></span>|<span data-ttu-id="d2396-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d2396-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2396-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d2396-126">Request body</span></span>
<span data-ttu-id="d2396-127">要求本文で、 [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d2396-127">In the request body, supply a JSON representation for the [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>

<span data-ttu-id="d2396-128">次の表に、 [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d2396-128">The following table shows the properties that are required when you create the [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md).</span></span>

|<span data-ttu-id="d2396-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d2396-129">Property</span></span>|<span data-ttu-id="d2396-130">型</span><span class="sxs-lookup"><span data-stu-id="d2396-130">Type</span></span>|<span data-ttu-id="d2396-131">説明</span><span class="sxs-lookup"><span data-stu-id="d2396-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2396-132">id</span><span class="sxs-lookup"><span data-stu-id="d2396-132">id</span></span>|<span data-ttu-id="d2396-133">文字列</span><span class="sxs-lookup"><span data-stu-id="d2396-133">String</span></span>|<span data-ttu-id="d2396-134">管理条件の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="d2396-134">Unique identifier for the management condition.</span></span> <span data-ttu-id="d2396-135">作成時に割り当てられたシステム生成値。</span><span class="sxs-lookup"><span data-stu-id="d2396-135">System generated value assigned when created.</span></span> <span data-ttu-id="d2396-136">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="d2396-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d2396-137">uniqueName</span><span class="sxs-lookup"><span data-stu-id="d2396-137">uniqueName</span></span>|<span data-ttu-id="d2396-138">String</span><span class="sxs-lookup"><span data-stu-id="d2396-138">String</span></span>|<span data-ttu-id="d2396-139">管理条件の一意の名前。</span><span class="sxs-lookup"><span data-stu-id="d2396-139">Unique name for the management condition.</span></span> <span data-ttu-id="d2396-140">管理条件式で使用されます。</span><span class="sxs-lookup"><span data-stu-id="d2396-140">Used in management condition expressions.</span></span> <span data-ttu-id="d2396-141">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="d2396-141">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d2396-142">displayName</span><span class="sxs-lookup"><span data-stu-id="d2396-142">displayName</span></span>|<span data-ttu-id="d2396-143">String</span><span class="sxs-lookup"><span data-stu-id="d2396-143">String</span></span>|<span data-ttu-id="d2396-144">管理条件の管理者定義の名前。</span><span class="sxs-lookup"><span data-stu-id="d2396-144">The admin defined name of the management condition.</span></span> <span data-ttu-id="d2396-145">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="d2396-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d2396-146">description</span><span class="sxs-lookup"><span data-stu-id="d2396-146">description</span></span>|<span data-ttu-id="d2396-147">String</span><span class="sxs-lookup"><span data-stu-id="d2396-147">String</span></span>|<span data-ttu-id="d2396-148">管理条件の管理者定義の説明。</span><span class="sxs-lookup"><span data-stu-id="d2396-148">The admin defined description of the management condition.</span></span> <span data-ttu-id="d2396-149">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="d2396-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d2396-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d2396-150">createdDateTime</span></span>|<span data-ttu-id="d2396-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2396-151">DateTimeOffset</span></span>|<span data-ttu-id="d2396-152">管理条件が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="d2396-152">The time the management condition was created.</span></span> <span data-ttu-id="d2396-153">サービス側を生成しました。</span><span class="sxs-lookup"><span data-stu-id="d2396-153">Generated service side.</span></span> <span data-ttu-id="d2396-154">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="d2396-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d2396-155">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d2396-155">modifiedDateTime</span></span>|<span data-ttu-id="d2396-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2396-156">DateTimeOffset</span></span>|<span data-ttu-id="d2396-157">管理条件が最後に変更された時刻。</span><span class="sxs-lookup"><span data-stu-id="d2396-157">The time the management condition was last modified.</span></span> <span data-ttu-id="d2396-158">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="d2396-158">Updated service side.</span></span> <span data-ttu-id="d2396-159">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="d2396-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d2396-160">eTag</span><span class="sxs-lookup"><span data-stu-id="d2396-160">eTag</span></span>|<span data-ttu-id="d2396-161">String</span><span class="sxs-lookup"><span data-stu-id="d2396-161">String</span></span>|<span data-ttu-id="d2396-162">管理条件の ETag。</span><span class="sxs-lookup"><span data-stu-id="d2396-162">ETag of the management condition.</span></span> <span data-ttu-id="d2396-163">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="d2396-163">Updated service side.</span></span> <span data-ttu-id="d2396-164">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="d2396-164">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d2396-165">アプリケーションのプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="d2396-165">applicablePlatforms</span></span>|<span data-ttu-id="d2396-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d2396-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="d2396-167">この管理条件の適用可能なプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="d2396-167">The applicable platforms for this management condition.</span></span> <span data-ttu-id="d2396-168">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="d2396-168">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="d2396-169">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="d2396-169">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="d2396-170">ipV6Prefix</span><span class="sxs-lookup"><span data-stu-id="d2396-170">ipV6Prefix</span></span>|<span data-ttu-id="d2396-171">String</span><span class="sxs-lookup"><span data-stu-id="d2396-171">String</span></span>|<span data-ttu-id="d2396-172">接続先の IPv6 サブネット。</span><span class="sxs-lookup"><span data-stu-id="d2396-172">The IPv6 subnet to be connected to.</span></span> <span data-ttu-id="d2396-173">例: 2001 年: db8::/32</span><span class="sxs-lookup"><span data-stu-id="d2396-173">e.g. 2001:db8::/32</span></span>|
|<span data-ttu-id="d2396-174">ipV6Gateway</span><span class="sxs-lookup"><span data-stu-id="d2396-174">ipV6Gateway</span></span>|<span data-ttu-id="d2396-175">String</span><span class="sxs-lookup"><span data-stu-id="d2396-175">String</span></span>|<span data-ttu-id="d2396-176">IPv6 ゲートウェイアドレス。</span><span class="sxs-lookup"><span data-stu-id="d2396-176">The IPv6 gateway address to.</span></span> <span data-ttu-id="d2396-177">例: 2001 年: db8:: 1</span><span class="sxs-lookup"><span data-stu-id="d2396-177">e.g 2001:db8::1</span></span>|
|<span data-ttu-id="d2396-178">ipV6DNSServerList</span><span class="sxs-lookup"><span data-stu-id="d2396-178">ipV6DNSServerList</span></span>|<span data-ttu-id="d2396-179">String collection</span><span class="sxs-lookup"><span data-stu-id="d2396-179">String collection</span></span>|<span data-ttu-id="d2396-180">アダプターに対して構成された IPv6 DNS サーバー。</span><span class="sxs-lookup"><span data-stu-id="d2396-180">An IPv6 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="d2396-181">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="d2396-181">dnsSuffixList</span></span>|<span data-ttu-id="d2396-182">String collection</span><span class="sxs-lookup"><span data-stu-id="d2396-182">String collection</span></span>|<span data-ttu-id="d2396-183">現在のネットワークの有効な DNS サフィックス。</span><span class="sxs-lookup"><span data-stu-id="d2396-183">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="d2396-184">例: seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="d2396-184">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="d2396-185">応答</span><span class="sxs-lookup"><span data-stu-id="d2396-185">Response</span></span>
<span data-ttu-id="d2396-186">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d2396-186">If successful, this method returns a `200 OK` response code and an updated [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2396-187">例</span><span class="sxs-lookup"><span data-stu-id="d2396-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2396-188">要求</span><span class="sxs-lookup"><span data-stu-id="d2396-188">Request</span></span>
<span data-ttu-id="d2396-189">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d2396-189">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
Content-type: application/json
Content-length: 483

{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV6Prefix": "Ip V6Prefix value",
  "ipV6Gateway": "Ip V6Gateway value",
  "ipV6DNSServerList": [
    "Ip V6DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="d2396-190">応答</span><span class="sxs-lookup"><span data-stu-id="d2396-190">Response</span></span>
<span data-ttu-id="d2396-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d2396-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 651

{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "id": "25811206-1206-2581-0612-812506128125",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV6Prefix": "Ip V6Prefix value",
  "ipV6Gateway": "Ip V6Gateway value",
  "ipV6DNSServerList": [
    "Ip V6DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```




