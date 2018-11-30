---
title: NetworkIPv6ConfigurationManagementCondition を作成します。
description: 新しい networkIPv6ConfigurationManagementCondition オブジェクトを作成します。
ms.openlocfilehash: be69c9a69653bb35413446fe69d36016cb344ced
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070134"
---
# <a name="create-networkipv6configurationmanagementcondition"></a><span data-ttu-id="3e8b1-103">NetworkIPv6ConfigurationManagementCondition を作成します。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-103">Create networkIPv6ConfigurationManagementCondition</span></span>

> <span data-ttu-id="3e8b1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e8b1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3e8b1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3e8b1-107">新しい[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-107">Create a new [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3e8b1-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="3e8b1-108">Prerequisites</span></span>
<span data-ttu-id="3e8b1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e8b1-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3e8b1-111">Permission type</span></span>|<span data-ttu-id="3e8b1-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3e8b1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e8b1-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3e8b1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3e8b1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e8b1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3e8b1-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3e8b1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e8b1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-116">Not supported.</span></span>|
|<span data-ttu-id="3e8b1-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3e8b1-117">Application</span></span>|<span data-ttu-id="3e8b1-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e8b1-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3e8b1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="3e8b1-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3e8b1-120">Request headers</span></span>
|<span data-ttu-id="3e8b1-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3e8b1-121">Header</span></span>|<span data-ttu-id="3e8b1-122">値</span><span class="sxs-lookup"><span data-stu-id="3e8b1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e8b1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e8b1-123">Authorization</span></span>|<span data-ttu-id="3e8b1-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e8b1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3e8b1-125">Accept</span></span>|<span data-ttu-id="3e8b1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3e8b1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e8b1-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3e8b1-127">Request body</span></span>
<span data-ttu-id="3e8b1-128">要求の本文に networkIPv6ConfigurationManagementCondition オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-128">In the request body, supply a JSON representation for the networkIPv6ConfigurationManagementCondition object.</span></span>

<span data-ttu-id="3e8b1-129">次の表は、networkIPv6ConfigurationManagementCondition を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-129">The following table shows the properties that are required when you create the networkIPv6ConfigurationManagementCondition.</span></span>

|<span data-ttu-id="3e8b1-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3e8b1-130">Property</span></span>|<span data-ttu-id="3e8b1-131">型</span><span class="sxs-lookup"><span data-stu-id="3e8b1-131">Type</span></span>|<span data-ttu-id="3e8b1-132">説明</span><span class="sxs-lookup"><span data-stu-id="3e8b1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e8b1-133">id</span><span class="sxs-lookup"><span data-stu-id="3e8b1-133">id</span></span>|<span data-ttu-id="3e8b1-134">String</span><span class="sxs-lookup"><span data-stu-id="3e8b1-134">String</span></span>|<span data-ttu-id="3e8b1-135">管理条件の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="3e8b1-136">システムでは、作成時に割り当てられた値が生成されます。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-136">System generated value assigned when created.</span></span> <span data-ttu-id="3e8b1-137">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="3e8b1-138">一意な名前</span><span class="sxs-lookup"><span data-stu-id="3e8b1-138">uniqueName</span></span>|<span data-ttu-id="3e8b1-139">String</span><span class="sxs-lookup"><span data-stu-id="3e8b1-139">String</span></span>|<span data-ttu-id="3e8b1-140">管理条件の一意の名前です。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-140">Unique name for the management condition.</span></span> <span data-ttu-id="3e8b1-141">管理条件式で使用されます。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-141">Used in management condition expressions.</span></span> <span data-ttu-id="3e8b1-142">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="3e8b1-143">displayName</span><span class="sxs-lookup"><span data-stu-id="3e8b1-143">displayName</span></span>|<span data-ttu-id="3e8b1-144">String</span><span class="sxs-lookup"><span data-stu-id="3e8b1-144">String</span></span>|<span data-ttu-id="3e8b1-145">管理者は、管理の条件の名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="3e8b1-146">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="3e8b1-147">説明</span><span class="sxs-lookup"><span data-stu-id="3e8b1-147">description</span></span>|<span data-ttu-id="3e8b1-148">String</span><span class="sxs-lookup"><span data-stu-id="3e8b1-148">String</span></span>|<span data-ttu-id="3e8b1-149">管理者は、管理状態の説明を定義します。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="3e8b1-150">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="3e8b1-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3e8b1-151">createdDateTime</span></span>|<span data-ttu-id="3e8b1-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e8b1-152">DateTimeOffset</span></span>|<span data-ttu-id="3e8b1-153">管理条件が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-153">The time the management condition was created.</span></span> <span data-ttu-id="3e8b1-154">サービス側が生成されます。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-154">Generated service side.</span></span> <span data-ttu-id="3e8b1-155">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="3e8b1-156">変更された日時</span><span class="sxs-lookup"><span data-stu-id="3e8b1-156">modifiedDateTime</span></span>|<span data-ttu-id="3e8b1-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e8b1-157">DateTimeOffset</span></span>|<span data-ttu-id="3e8b1-158">管理条件が最後に修正された時間です。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-158">The time the management condition was last modified.</span></span> <span data-ttu-id="3e8b1-159">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-159">Updated service side.</span></span> <span data-ttu-id="3e8b1-160">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="3e8b1-161">eTag</span><span class="sxs-lookup"><span data-stu-id="3e8b1-161">eTag</span></span>|<span data-ttu-id="3e8b1-162">String</span><span class="sxs-lookup"><span data-stu-id="3e8b1-162">String</span></span>|<span data-ttu-id="3e8b1-163">管理条件の ETag。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-163">ETag of the management condition.</span></span> <span data-ttu-id="3e8b1-164">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-164">Updated service side.</span></span> <span data-ttu-id="3e8b1-165">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="3e8b1-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="3e8b1-166">applicablePlatforms</span></span>|<span data-ttu-id="3e8b1-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3e8b1-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="3e8b1-168">この管理条件に該当するプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="3e8b1-169">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="3e8b1-170">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile` です。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="3e8b1-171">ipV6Prefix</span><span class="sxs-lookup"><span data-stu-id="3e8b1-171">ipV6Prefix</span></span>|<span data-ttu-id="3e8b1-172">String</span><span class="sxs-lookup"><span data-stu-id="3e8b1-172">String</span></span>|<span data-ttu-id="3e8b1-173">接続されている IPv6 サブネットです。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-173">The IPv6 subnet to be connected to.</span></span> <span data-ttu-id="3e8b1-174">例: 2001:db8::/32</span><span class="sxs-lookup"><span data-stu-id="3e8b1-174">e.g. 2001:db8::/32</span></span>|
|<span data-ttu-id="3e8b1-175">ipV6Gateway</span><span class="sxs-lookup"><span data-stu-id="3e8b1-175">ipV6Gateway</span></span>|<span data-ttu-id="3e8b1-176">String</span><span class="sxs-lookup"><span data-stu-id="3e8b1-176">String</span></span>|<span data-ttu-id="3e8b1-177">IPv6 ゲートウェイ アドレスです。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-177">The IPv6 gateway address to.</span></span> <span data-ttu-id="3e8b1-178">例: 2001:db8::1</span><span class="sxs-lookup"><span data-stu-id="3e8b1-178">e.g 2001:db8::1</span></span>|
|<span data-ttu-id="3e8b1-179">ipV6DNSServerList</span><span class="sxs-lookup"><span data-stu-id="3e8b1-179">ipV6DNSServerList</span></span>|<span data-ttu-id="3e8b1-180">String コレクション</span><span class="sxs-lookup"><span data-stu-id="3e8b1-180">String collection</span></span>|<span data-ttu-id="3e8b1-181">アダプター用に構成された IPv6 の DNS サーバーをします。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-181">An IPv6 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="3e8b1-182">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="3e8b1-182">dnsSuffixList</span></span>|<span data-ttu-id="3e8b1-183">String コレクション</span><span class="sxs-lookup"><span data-stu-id="3e8b1-183">String collection</span></span>|<span data-ttu-id="3e8b1-184">現在のネットワークの有効な DNS サフィックスです。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-184">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="3e8b1-185">例: seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="3e8b1-185">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="3e8b1-186">応答</span><span class="sxs-lookup"><span data-stu-id="3e8b1-186">Response</span></span>
<span data-ttu-id="3e8b1-187">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-187">If successful, this method returns a `201 Created` response code and a [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e8b1-188">例</span><span class="sxs-lookup"><span data-stu-id="3e8b1-188">Example</span></span>
### <a name="request"></a><span data-ttu-id="3e8b1-189">要求</span><span class="sxs-lookup"><span data-stu-id="3e8b1-189">Request</span></span>
<span data-ttu-id="3e8b1-190">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-190">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditions
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

### <a name="response"></a><span data-ttu-id="3e8b1-191">応答</span><span class="sxs-lookup"><span data-stu-id="3e8b1-191">Response</span></span>
<span data-ttu-id="3e8b1-p114">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3e8b1-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





