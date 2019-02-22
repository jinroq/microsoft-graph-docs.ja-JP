---
title: networkIPv6ConfigurationManagementCondition を作成する
description: 新しい networkIPv6ConfigurationManagementCondition オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5cce69f184ad9e3a67248ee5b388a1606b7a37b6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154643"
---
# <a name="create-networkipv6configurationmanagementcondition"></a><span data-ttu-id="6dc24-103">networkIPv6ConfigurationManagementCondition を作成する</span><span class="sxs-lookup"><span data-stu-id="6dc24-103">Create networkIPv6ConfigurationManagementCondition</span></span>

> <span data-ttu-id="6dc24-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6dc24-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6dc24-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6dc24-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6dc24-106">新しい[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6dc24-106">Create a new [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6dc24-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="6dc24-107">Prerequisites</span></span>
<span data-ttu-id="6dc24-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6dc24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6dc24-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6dc24-110">Permission type</span></span>|<span data-ttu-id="6dc24-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6dc24-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6dc24-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6dc24-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6dc24-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dc24-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6dc24-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6dc24-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6dc24-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6dc24-115">Not supported.</span></span>|
|<span data-ttu-id="6dc24-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6dc24-116">Application</span></span>|<span data-ttu-id="6dc24-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6dc24-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6dc24-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6dc24-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="6dc24-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6dc24-119">Request headers</span></span>
|<span data-ttu-id="6dc24-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6dc24-120">Header</span></span>|<span data-ttu-id="6dc24-121">値</span><span class="sxs-lookup"><span data-stu-id="6dc24-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6dc24-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6dc24-122">Authorization</span></span>|<span data-ttu-id="6dc24-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="6dc24-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6dc24-124">承諾</span><span class="sxs-lookup"><span data-stu-id="6dc24-124">Accept</span></span>|<span data-ttu-id="6dc24-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6dc24-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dc24-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6dc24-126">Request body</span></span>
<span data-ttu-id="6dc24-127">要求本文で、networkIPv6ConfigurationManagementCondition オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6dc24-127">In the request body, supply a JSON representation for the networkIPv6ConfigurationManagementCondition object.</span></span>

<span data-ttu-id="6dc24-128">次の表に、networkIPv6ConfigurationManagementCondition の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6dc24-128">The following table shows the properties that are required when you create the networkIPv6ConfigurationManagementCondition.</span></span>

|<span data-ttu-id="6dc24-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6dc24-129">Property</span></span>|<span data-ttu-id="6dc24-130">型</span><span class="sxs-lookup"><span data-stu-id="6dc24-130">Type</span></span>|<span data-ttu-id="6dc24-131">説明</span><span class="sxs-lookup"><span data-stu-id="6dc24-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6dc24-132">id</span><span class="sxs-lookup"><span data-stu-id="6dc24-132">id</span></span>|<span data-ttu-id="6dc24-133">文字列</span><span class="sxs-lookup"><span data-stu-id="6dc24-133">String</span></span>|<span data-ttu-id="6dc24-134">管理条件の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="6dc24-134">Unique identifier for the management condition.</span></span> <span data-ttu-id="6dc24-135">作成時に割り当てられたシステム生成値。</span><span class="sxs-lookup"><span data-stu-id="6dc24-135">System generated value assigned when created.</span></span> <span data-ttu-id="6dc24-136">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="6dc24-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="6dc24-137">uniqueName</span><span class="sxs-lookup"><span data-stu-id="6dc24-137">uniqueName</span></span>|<span data-ttu-id="6dc24-138">String</span><span class="sxs-lookup"><span data-stu-id="6dc24-138">String</span></span>|<span data-ttu-id="6dc24-139">管理条件の一意の名前。</span><span class="sxs-lookup"><span data-stu-id="6dc24-139">Unique name for the management condition.</span></span> <span data-ttu-id="6dc24-140">管理条件式で使用されます。</span><span class="sxs-lookup"><span data-stu-id="6dc24-140">Used in management condition expressions.</span></span> <span data-ttu-id="6dc24-141">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="6dc24-141">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="6dc24-142">displayName</span><span class="sxs-lookup"><span data-stu-id="6dc24-142">displayName</span></span>|<span data-ttu-id="6dc24-143">String</span><span class="sxs-lookup"><span data-stu-id="6dc24-143">String</span></span>|<span data-ttu-id="6dc24-144">管理条件の管理者定義の名前。</span><span class="sxs-lookup"><span data-stu-id="6dc24-144">The admin defined name of the management condition.</span></span> <span data-ttu-id="6dc24-145">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="6dc24-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="6dc24-146">説明</span><span class="sxs-lookup"><span data-stu-id="6dc24-146">description</span></span>|<span data-ttu-id="6dc24-147">String</span><span class="sxs-lookup"><span data-stu-id="6dc24-147">String</span></span>|<span data-ttu-id="6dc24-148">管理条件の管理者定義の説明。</span><span class="sxs-lookup"><span data-stu-id="6dc24-148">The admin defined description of the management condition.</span></span> <span data-ttu-id="6dc24-149">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="6dc24-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="6dc24-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6dc24-150">createdDateTime</span></span>|<span data-ttu-id="6dc24-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6dc24-151">DateTimeOffset</span></span>|<span data-ttu-id="6dc24-152">管理条件が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="6dc24-152">The time the management condition was created.</span></span> <span data-ttu-id="6dc24-153">サービス側を生成しました。</span><span class="sxs-lookup"><span data-stu-id="6dc24-153">Generated service side.</span></span> <span data-ttu-id="6dc24-154">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="6dc24-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="6dc24-155">変更された日時</span><span class="sxs-lookup"><span data-stu-id="6dc24-155">modifiedDateTime</span></span>|<span data-ttu-id="6dc24-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6dc24-156">DateTimeOffset</span></span>|<span data-ttu-id="6dc24-157">管理条件が最後に変更された時刻。</span><span class="sxs-lookup"><span data-stu-id="6dc24-157">The time the management condition was last modified.</span></span> <span data-ttu-id="6dc24-158">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="6dc24-158">Updated service side.</span></span> <span data-ttu-id="6dc24-159">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="6dc24-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="6dc24-160">eTag</span><span class="sxs-lookup"><span data-stu-id="6dc24-160">eTag</span></span>|<span data-ttu-id="6dc24-161">String</span><span class="sxs-lookup"><span data-stu-id="6dc24-161">String</span></span>|<span data-ttu-id="6dc24-162">管理条件の ETag。</span><span class="sxs-lookup"><span data-stu-id="6dc24-162">ETag of the management condition.</span></span> <span data-ttu-id="6dc24-163">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="6dc24-163">Updated service side.</span></span> <span data-ttu-id="6dc24-164">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="6dc24-164">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="6dc24-165">アプリケーションのプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="6dc24-165">applicablePlatforms</span></span>|<span data-ttu-id="6dc24-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6dc24-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="6dc24-167">この管理条件の適用可能なプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="6dc24-167">The applicable platforms for this management condition.</span></span> <span data-ttu-id="6dc24-168">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="6dc24-168">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="6dc24-169">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile` です。</span><span class="sxs-lookup"><span data-stu-id="6dc24-169">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="6dc24-170">ipV6Prefix</span><span class="sxs-lookup"><span data-stu-id="6dc24-170">ipV6Prefix</span></span>|<span data-ttu-id="6dc24-171">String</span><span class="sxs-lookup"><span data-stu-id="6dc24-171">String</span></span>|<span data-ttu-id="6dc24-172">接続先の IPv6 サブネット。</span><span class="sxs-lookup"><span data-stu-id="6dc24-172">The IPv6 subnet to be connected to.</span></span> <span data-ttu-id="6dc24-173">例: 2001 年: db8::/32</span><span class="sxs-lookup"><span data-stu-id="6dc24-173">e.g. 2001:db8::/32</span></span>|
|<span data-ttu-id="6dc24-174">ipV6Gateway</span><span class="sxs-lookup"><span data-stu-id="6dc24-174">ipV6Gateway</span></span>|<span data-ttu-id="6dc24-175">String</span><span class="sxs-lookup"><span data-stu-id="6dc24-175">String</span></span>|<span data-ttu-id="6dc24-176">IPv6 ゲートウェイアドレス。</span><span class="sxs-lookup"><span data-stu-id="6dc24-176">The IPv6 gateway address to.</span></span> <span data-ttu-id="6dc24-177">例: 2001 年: db8:: 1</span><span class="sxs-lookup"><span data-stu-id="6dc24-177">e.g 2001:db8::1</span></span>|
|<span data-ttu-id="6dc24-178">ipV6DNSServerList</span><span class="sxs-lookup"><span data-stu-id="6dc24-178">ipV6DNSServerList</span></span>|<span data-ttu-id="6dc24-179">String collection</span><span class="sxs-lookup"><span data-stu-id="6dc24-179">String collection</span></span>|<span data-ttu-id="6dc24-180">アダプターに対して構成された IPv6 DNS サーバー。</span><span class="sxs-lookup"><span data-stu-id="6dc24-180">An IPv6 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="6dc24-181">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="6dc24-181">dnsSuffixList</span></span>|<span data-ttu-id="6dc24-182">String collection</span><span class="sxs-lookup"><span data-stu-id="6dc24-182">String collection</span></span>|<span data-ttu-id="6dc24-183">現在のネットワークの有効な DNS サフィックス。</span><span class="sxs-lookup"><span data-stu-id="6dc24-183">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="6dc24-184">例: seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="6dc24-184">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="6dc24-185">応答</span><span class="sxs-lookup"><span data-stu-id="6dc24-185">Response</span></span>
<span data-ttu-id="6dc24-186">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6dc24-186">If successful, this method returns a `201 Created` response code and a [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6dc24-187">例</span><span class="sxs-lookup"><span data-stu-id="6dc24-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="6dc24-188">要求</span><span class="sxs-lookup"><span data-stu-id="6dc24-188">Request</span></span>
<span data-ttu-id="6dc24-189">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6dc24-189">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6dc24-190">応答</span><span class="sxs-lookup"><span data-stu-id="6dc24-190">Response</span></span>
<span data-ttu-id="6dc24-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6dc24-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




