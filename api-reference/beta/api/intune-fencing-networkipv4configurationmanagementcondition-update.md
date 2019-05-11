---
title: NetworkIPv4ConfigurationManagementCondition の更新
description: NetworkIPv4ConfigurationManagementCondition オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b19f29064e0fe5bd673c0ffbc0677959b9be844c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33905274"
---
# <a name="update-networkipv4configurationmanagementcondition"></a><span data-ttu-id="e2b21-103">NetworkIPv4ConfigurationManagementCondition の更新</span><span class="sxs-lookup"><span data-stu-id="e2b21-103">Update networkIPv4ConfigurationManagementCondition</span></span>

> <span data-ttu-id="e2b21-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2b21-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2b21-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e2b21-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2b21-106">[NetworkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e2b21-106">Update the properties of a [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2b21-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e2b21-107">Prerequisites</span></span>
<span data-ttu-id="e2b21-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e2b21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2b21-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e2b21-110">Permission type</span></span>|<span data-ttu-id="e2b21-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e2b21-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2b21-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e2b21-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e2b21-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2b21-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e2b21-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e2b21-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2b21-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2b21-115">Not supported.</span></span>|
|<span data-ttu-id="e2b21-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e2b21-116">Application</span></span>|<span data-ttu-id="e2b21-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2b21-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2b21-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e2b21-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="e2b21-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e2b21-119">Request headers</span></span>
|<span data-ttu-id="e2b21-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e2b21-120">Header</span></span>|<span data-ttu-id="e2b21-121">値</span><span class="sxs-lookup"><span data-stu-id="e2b21-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2b21-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2b21-122">Authorization</span></span>|<span data-ttu-id="e2b21-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e2b21-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2b21-124">承諾</span><span class="sxs-lookup"><span data-stu-id="e2b21-124">Accept</span></span>|<span data-ttu-id="e2b21-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e2b21-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2b21-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e2b21-126">Request body</span></span>
<span data-ttu-id="e2b21-127">要求本文で、 [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e2b21-127">In the request body, supply a JSON representation for the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

<span data-ttu-id="e2b21-128">次の表に、 [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e2b21-128">The following table shows the properties that are required when you create the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md).</span></span>

|<span data-ttu-id="e2b21-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2b21-129">Property</span></span>|<span data-ttu-id="e2b21-130">型</span><span class="sxs-lookup"><span data-stu-id="e2b21-130">Type</span></span>|<span data-ttu-id="e2b21-131">説明</span><span class="sxs-lookup"><span data-stu-id="e2b21-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2b21-132">id</span><span class="sxs-lookup"><span data-stu-id="e2b21-132">id</span></span>|<span data-ttu-id="e2b21-133">文字列</span><span class="sxs-lookup"><span data-stu-id="e2b21-133">String</span></span>|<span data-ttu-id="e2b21-134">管理条件の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="e2b21-134">Unique identifier for the management condition.</span></span> <span data-ttu-id="e2b21-135">作成時に割り当てられたシステム生成値。</span><span class="sxs-lookup"><span data-stu-id="e2b21-135">System generated value assigned when created.</span></span> <span data-ttu-id="e2b21-136">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="e2b21-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="e2b21-137">uniqueName</span><span class="sxs-lookup"><span data-stu-id="e2b21-137">uniqueName</span></span>|<span data-ttu-id="e2b21-138">String</span><span class="sxs-lookup"><span data-stu-id="e2b21-138">String</span></span>|<span data-ttu-id="e2b21-139">管理条件の一意の名前。</span><span class="sxs-lookup"><span data-stu-id="e2b21-139">Unique name for the management condition.</span></span> <span data-ttu-id="e2b21-140">管理条件式で使用されます。</span><span class="sxs-lookup"><span data-stu-id="e2b21-140">Used in management condition expressions.</span></span> <span data-ttu-id="e2b21-141">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="e2b21-141">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="e2b21-142">displayName</span><span class="sxs-lookup"><span data-stu-id="e2b21-142">displayName</span></span>|<span data-ttu-id="e2b21-143">String</span><span class="sxs-lookup"><span data-stu-id="e2b21-143">String</span></span>|<span data-ttu-id="e2b21-144">管理条件の管理者定義の名前。</span><span class="sxs-lookup"><span data-stu-id="e2b21-144">The admin defined name of the management condition.</span></span> <span data-ttu-id="e2b21-145">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="e2b21-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="e2b21-146">description</span><span class="sxs-lookup"><span data-stu-id="e2b21-146">description</span></span>|<span data-ttu-id="e2b21-147">String</span><span class="sxs-lookup"><span data-stu-id="e2b21-147">String</span></span>|<span data-ttu-id="e2b21-148">管理条件の管理者定義の説明。</span><span class="sxs-lookup"><span data-stu-id="e2b21-148">The admin defined description of the management condition.</span></span> <span data-ttu-id="e2b21-149">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="e2b21-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="e2b21-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e2b21-150">createdDateTime</span></span>|<span data-ttu-id="e2b21-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2b21-151">DateTimeOffset</span></span>|<span data-ttu-id="e2b21-152">管理条件が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="e2b21-152">The time the management condition was created.</span></span> <span data-ttu-id="e2b21-153">サービス側を生成しました。</span><span class="sxs-lookup"><span data-stu-id="e2b21-153">Generated service side.</span></span> <span data-ttu-id="e2b21-154">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="e2b21-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="e2b21-155">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2b21-155">modifiedDateTime</span></span>|<span data-ttu-id="e2b21-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2b21-156">DateTimeOffset</span></span>|<span data-ttu-id="e2b21-157">管理条件が最後に変更された時刻。</span><span class="sxs-lookup"><span data-stu-id="e2b21-157">The time the management condition was last modified.</span></span> <span data-ttu-id="e2b21-158">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="e2b21-158">Updated service side.</span></span> <span data-ttu-id="e2b21-159">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="e2b21-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="e2b21-160">eTag</span><span class="sxs-lookup"><span data-stu-id="e2b21-160">eTag</span></span>|<span data-ttu-id="e2b21-161">String</span><span class="sxs-lookup"><span data-stu-id="e2b21-161">String</span></span>|<span data-ttu-id="e2b21-162">管理条件の ETag。</span><span class="sxs-lookup"><span data-stu-id="e2b21-162">ETag of the management condition.</span></span> <span data-ttu-id="e2b21-163">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="e2b21-163">Updated service side.</span></span> <span data-ttu-id="e2b21-164">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="e2b21-164">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="e2b21-165">アプリケーションのプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="e2b21-165">applicablePlatforms</span></span>|<span data-ttu-id="e2b21-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e2b21-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="e2b21-167">この管理条件の適用可能なプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="e2b21-167">The applicable platforms for this management condition.</span></span> <span data-ttu-id="e2b21-168">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="e2b21-168">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="e2b21-169">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="e2b21-169">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="e2b21-170">ipV4Prefix</span><span class="sxs-lookup"><span data-stu-id="e2b21-170">ipV4Prefix</span></span>|<span data-ttu-id="e2b21-171">String</span><span class="sxs-lookup"><span data-stu-id="e2b21-171">String</span></span>|<span data-ttu-id="e2b21-172">接続先の IPv4 サブネット。</span><span class="sxs-lookup"><span data-stu-id="e2b21-172">The IPv4 subnet to be connected to.</span></span> <span data-ttu-id="e2b21-173">例: 10.0.0.0/8</span><span class="sxs-lookup"><span data-stu-id="e2b21-173">e.g. 10.0.0.0/8</span></span>|
|<span data-ttu-id="e2b21-174">ipV4Gateway</span><span class="sxs-lookup"><span data-stu-id="e2b21-174">ipV4Gateway</span></span>|<span data-ttu-id="e2b21-175">String</span><span class="sxs-lookup"><span data-stu-id="e2b21-175">String</span></span>|<span data-ttu-id="e2b21-176">IPv4 ゲートウェイアドレス。</span><span class="sxs-lookup"><span data-stu-id="e2b21-176">The IPv4 gateway address.</span></span> <span data-ttu-id="e2b21-177">例: 10.0.0.0</span><span class="sxs-lookup"><span data-stu-id="e2b21-177">e.g. 10.0.0.0</span></span>|
|<span data-ttu-id="e2b21-178">ipV4DHCPServer</span><span class="sxs-lookup"><span data-stu-id="e2b21-178">ipV4DHCPServer</span></span>|<span data-ttu-id="e2b21-179">String</span><span class="sxs-lookup"><span data-stu-id="e2b21-179">String</span></span>|<span data-ttu-id="e2b21-180">アダプターの DHCP サーバーの IPv4 アドレス。</span><span class="sxs-lookup"><span data-stu-id="e2b21-180">The IPv4 address of the DHCP server for the adapter.</span></span>|
|<span data-ttu-id="e2b21-181">ipV4DNSServerList</span><span class="sxs-lookup"><span data-stu-id="e2b21-181">ipV4DNSServerList</span></span>|<span data-ttu-id="e2b21-182">String collection</span><span class="sxs-lookup"><span data-stu-id="e2b21-182">String collection</span></span>|<span data-ttu-id="e2b21-183">アダプターに対して構成されている IPv4 DNS サーバー。</span><span class="sxs-lookup"><span data-stu-id="e2b21-183">The IPv4 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="e2b21-184">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="e2b21-184">dnsSuffixList</span></span>|<span data-ttu-id="e2b21-185">String collection</span><span class="sxs-lookup"><span data-stu-id="e2b21-185">String collection</span></span>|<span data-ttu-id="e2b21-186">現在のネットワークの有効な DNS サフィックス。</span><span class="sxs-lookup"><span data-stu-id="e2b21-186">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="e2b21-187">例: seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="e2b21-187">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="e2b21-188">応答</span><span class="sxs-lookup"><span data-stu-id="e2b21-188">Response</span></span>
<span data-ttu-id="e2b21-189">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e2b21-189">If successful, this method returns a `200 OK` response code and an updated [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2b21-190">例</span><span class="sxs-lookup"><span data-stu-id="e2b21-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2b21-191">要求</span><span class="sxs-lookup"><span data-stu-id="e2b21-191">Request</span></span>
<span data-ttu-id="e2b21-192">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e2b21-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
Content-type: application/json
Content-length: 529

{
  "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV4Prefix": "Ip V4Prefix value",
  "ipV4Gateway": "Ip V4Gateway value",
  "ipV4DHCPServer": "Ip V4DHCPServer value",
  "ipV4DNSServerList": [
    "Ip V4DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="e2b21-193">応答</span><span class="sxs-lookup"><span data-stu-id="e2b21-193">Response</span></span>
<span data-ttu-id="e2b21-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e2b21-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 697

{
  "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
  "id": "5e4a8284-8284-5e4a-8482-4a5e84824a5e",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV4Prefix": "Ip V4Prefix value",
  "ipV4Gateway": "Ip V4Gateway value",
  "ipV4DHCPServer": "Ip V4DHCPServer value",
  "ipV4DNSServerList": [
    "Ip V4DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```




