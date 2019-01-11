---
title: NetworkIPv4ConfigurationManagementCondition を更新します。
description: NetworkIPv4ConfigurationManagementCondition オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fc9662e812909bb78a0a9441c5fd0cb6929d26db
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867824"
---
# <a name="update-networkipv4configurationmanagementcondition"></a><span data-ttu-id="95dd3-103">NetworkIPv4ConfigurationManagementCondition を更新します。</span><span class="sxs-lookup"><span data-stu-id="95dd3-103">Update networkIPv4ConfigurationManagementCondition</span></span>

> <span data-ttu-id="95dd3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="95dd3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="95dd3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95dd3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="95dd3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="95dd3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="95dd3-107">[NetworkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="95dd3-107">Update the properties of a [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="95dd3-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="95dd3-108">Prerequisites</span></span>
<span data-ttu-id="95dd3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="95dd3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95dd3-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="95dd3-111">Permission type</span></span>|<span data-ttu-id="95dd3-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="95dd3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95dd3-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="95dd3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="95dd3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95dd3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="95dd3-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="95dd3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95dd3-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95dd3-116">Not supported.</span></span>|
|<span data-ttu-id="95dd3-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="95dd3-117">Application</span></span>|<span data-ttu-id="95dd3-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95dd3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95dd3-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="95dd3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="95dd3-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95dd3-120">Request headers</span></span>
|<span data-ttu-id="95dd3-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95dd3-121">Header</span></span>|<span data-ttu-id="95dd3-122">値</span><span class="sxs-lookup"><span data-stu-id="95dd3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95dd3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="95dd3-123">Authorization</span></span>|<span data-ttu-id="95dd3-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="95dd3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95dd3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="95dd3-125">Accept</span></span>|<span data-ttu-id="95dd3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="95dd3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95dd3-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="95dd3-127">Request body</span></span>
<span data-ttu-id="95dd3-128">要求の本文に[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="95dd3-128">In the request body, supply a JSON representation for the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

<span data-ttu-id="95dd3-129">[NetworkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="95dd3-129">The following table shows the properties that are required when you create the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md).</span></span>

|<span data-ttu-id="95dd3-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95dd3-130">Property</span></span>|<span data-ttu-id="95dd3-131">種類</span><span class="sxs-lookup"><span data-stu-id="95dd3-131">Type</span></span>|<span data-ttu-id="95dd3-132">説明</span><span class="sxs-lookup"><span data-stu-id="95dd3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95dd3-133">ID</span><span class="sxs-lookup"><span data-stu-id="95dd3-133">id</span></span>|<span data-ttu-id="95dd3-134">String</span><span class="sxs-lookup"><span data-stu-id="95dd3-134">String</span></span>|<span data-ttu-id="95dd3-135">管理条件の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="95dd3-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="95dd3-136">システムでは、作成時に割り当てられた値が生成されます。</span><span class="sxs-lookup"><span data-stu-id="95dd3-136">System generated value assigned when created.</span></span> <span data-ttu-id="95dd3-137">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="95dd3-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="95dd3-138">一意な名前</span><span class="sxs-lookup"><span data-stu-id="95dd3-138">uniqueName</span></span>|<span data-ttu-id="95dd3-139">String</span><span class="sxs-lookup"><span data-stu-id="95dd3-139">String</span></span>|<span data-ttu-id="95dd3-140">管理条件の一意の名前です。</span><span class="sxs-lookup"><span data-stu-id="95dd3-140">Unique name for the management condition.</span></span> <span data-ttu-id="95dd3-141">管理条件式で使用されます。</span><span class="sxs-lookup"><span data-stu-id="95dd3-141">Used in management condition expressions.</span></span> <span data-ttu-id="95dd3-142">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="95dd3-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="95dd3-143">displayName</span><span class="sxs-lookup"><span data-stu-id="95dd3-143">displayName</span></span>|<span data-ttu-id="95dd3-144">String</span><span class="sxs-lookup"><span data-stu-id="95dd3-144">String</span></span>|<span data-ttu-id="95dd3-145">管理者は、管理の条件の名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="95dd3-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="95dd3-146">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="95dd3-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="95dd3-147">説明</span><span class="sxs-lookup"><span data-stu-id="95dd3-147">description</span></span>|<span data-ttu-id="95dd3-148">String</span><span class="sxs-lookup"><span data-stu-id="95dd3-148">String</span></span>|<span data-ttu-id="95dd3-149">管理者は、管理状態の説明を定義します。</span><span class="sxs-lookup"><span data-stu-id="95dd3-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="95dd3-150">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="95dd3-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="95dd3-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95dd3-151">createdDateTime</span></span>|<span data-ttu-id="95dd3-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95dd3-152">DateTimeOffset</span></span>|<span data-ttu-id="95dd3-153">管理条件が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="95dd3-153">The time the management condition was created.</span></span> <span data-ttu-id="95dd3-154">サービス側が生成されます。</span><span class="sxs-lookup"><span data-stu-id="95dd3-154">Generated service side.</span></span> <span data-ttu-id="95dd3-155">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="95dd3-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="95dd3-156">変更された日時</span><span class="sxs-lookup"><span data-stu-id="95dd3-156">modifiedDateTime</span></span>|<span data-ttu-id="95dd3-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95dd3-157">DateTimeOffset</span></span>|<span data-ttu-id="95dd3-158">管理条件が最後に修正された時間です。</span><span class="sxs-lookup"><span data-stu-id="95dd3-158">The time the management condition was last modified.</span></span> <span data-ttu-id="95dd3-159">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="95dd3-159">Updated service side.</span></span> <span data-ttu-id="95dd3-160">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="95dd3-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="95dd3-161">eTag</span><span class="sxs-lookup"><span data-stu-id="95dd3-161">eTag</span></span>|<span data-ttu-id="95dd3-162">String</span><span class="sxs-lookup"><span data-stu-id="95dd3-162">String</span></span>|<span data-ttu-id="95dd3-163">管理条件の ETag。</span><span class="sxs-lookup"><span data-stu-id="95dd3-163">ETag of the management condition.</span></span> <span data-ttu-id="95dd3-164">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="95dd3-164">Updated service side.</span></span> <span data-ttu-id="95dd3-165">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="95dd3-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="95dd3-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="95dd3-166">applicablePlatforms</span></span>|<span data-ttu-id="95dd3-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="95dd3-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="95dd3-168">この管理条件に該当するプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="95dd3-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="95dd3-169">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="95dd3-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="95dd3-170">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile` です。</span><span class="sxs-lookup"><span data-stu-id="95dd3-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="95dd3-171">ipV4Prefix</span><span class="sxs-lookup"><span data-stu-id="95dd3-171">ipV4Prefix</span></span>|<span data-ttu-id="95dd3-172">String</span><span class="sxs-lookup"><span data-stu-id="95dd3-172">String</span></span>|<span data-ttu-id="95dd3-173">接続されている IPv4 サブネットです。</span><span class="sxs-lookup"><span data-stu-id="95dd3-173">The IPv4 subnet to be connected to.</span></span> <span data-ttu-id="95dd3-174">10.0.0.0/8 など</span><span class="sxs-lookup"><span data-stu-id="95dd3-174">e.g. 10.0.0.0/8</span></span>|
|<span data-ttu-id="95dd3-175">ipV4Gateway</span><span class="sxs-lookup"><span data-stu-id="95dd3-175">ipV4Gateway</span></span>|<span data-ttu-id="95dd3-176">String</span><span class="sxs-lookup"><span data-stu-id="95dd3-176">String</span></span>|<span data-ttu-id="95dd3-177">ゲートウェイの IPv4 アドレス。</span><span class="sxs-lookup"><span data-stu-id="95dd3-177">The IPv4 gateway address.</span></span> <span data-ttu-id="95dd3-178">10.0.0.0 など</span><span class="sxs-lookup"><span data-stu-id="95dd3-178">e.g. 10.0.0.0</span></span>|
|<span data-ttu-id="95dd3-179">ipV4DHCPServer</span><span class="sxs-lookup"><span data-stu-id="95dd3-179">ipV4DHCPServer</span></span>|<span data-ttu-id="95dd3-180">String</span><span class="sxs-lookup"><span data-stu-id="95dd3-180">String</span></span>|<span data-ttu-id="95dd3-181">アダプターの DHCP サーバーの IPv4 アドレスです。</span><span class="sxs-lookup"><span data-stu-id="95dd3-181">The IPv4 address of the DHCP server for the adapter.</span></span>|
|<span data-ttu-id="95dd3-182">ipV4DNSServerList</span><span class="sxs-lookup"><span data-stu-id="95dd3-182">ipV4DNSServerList</span></span>|<span data-ttu-id="95dd3-183">String コレクション</span><span class="sxs-lookup"><span data-stu-id="95dd3-183">String collection</span></span>|<span data-ttu-id="95dd3-184">アダプターに対して構成されている IPv4 DNS サーバーです。</span><span class="sxs-lookup"><span data-stu-id="95dd3-184">The IPv4 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="95dd3-185">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="95dd3-185">dnsSuffixList</span></span>|<span data-ttu-id="95dd3-186">String コレクション</span><span class="sxs-lookup"><span data-stu-id="95dd3-186">String collection</span></span>|<span data-ttu-id="95dd3-187">現在のネットワークの有効な DNS サフィックスです。</span><span class="sxs-lookup"><span data-stu-id="95dd3-187">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="95dd3-188">例: seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="95dd3-188">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="95dd3-189">応答</span><span class="sxs-lookup"><span data-stu-id="95dd3-189">Response</span></span>
<span data-ttu-id="95dd3-190">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="95dd3-190">If successful, this method returns a `200 OK` response code and an updated [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95dd3-191">例</span><span class="sxs-lookup"><span data-stu-id="95dd3-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="95dd3-192">要求</span><span class="sxs-lookup"><span data-stu-id="95dd3-192">Request</span></span>
<span data-ttu-id="95dd3-193">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="95dd3-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
Content-type: application/json
Content-length: 447

{
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

### <a name="response"></a><span data-ttu-id="95dd3-194">応答</span><span class="sxs-lookup"><span data-stu-id="95dd3-194">Response</span></span>
<span data-ttu-id="95dd3-p114">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="95dd3-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





