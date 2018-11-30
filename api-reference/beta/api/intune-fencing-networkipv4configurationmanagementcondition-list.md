---
title: リスト networkIPv4ConfigurationManagementConditions
description: NetworkIPv4ConfigurationManagementCondition オブジェクトのプロパティと関係を一覧表示します。
ms.openlocfilehash: e217a3d9e2c0cd7b3358d6380f92450fb3aa3864
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072320"
---
# <a name="list-networkipv4configurationmanagementconditions"></a><span data-ttu-id="77518-103">リスト networkIPv4ConfigurationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="77518-103">List networkIPv4ConfigurationManagementConditions</span></span>

> <span data-ttu-id="77518-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="77518-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77518-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77518-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="77518-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="77518-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="77518-107">[NetworkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="77518-107">List properties and relationships of the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="77518-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="77518-108">Prerequisites</span></span>
<span data-ttu-id="77518-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="77518-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77518-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="77518-111">Permission type</span></span>|<span data-ttu-id="77518-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="77518-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77518-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="77518-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77518-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="77518-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="77518-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="77518-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77518-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77518-116">Not supported.</span></span>|
|<span data-ttu-id="77518-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="77518-117">Application</span></span>|<span data-ttu-id="77518-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77518-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77518-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="77518-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="77518-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="77518-120">Request headers</span></span>
|<span data-ttu-id="77518-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="77518-121">Header</span></span>|<span data-ttu-id="77518-122">値</span><span class="sxs-lookup"><span data-stu-id="77518-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77518-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="77518-123">Authorization</span></span>|<span data-ttu-id="77518-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="77518-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77518-125">Accept</span><span class="sxs-lookup"><span data-stu-id="77518-125">Accept</span></span>|<span data-ttu-id="77518-126">application/json</span><span class="sxs-lookup"><span data-stu-id="77518-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77518-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="77518-127">Request body</span></span>
<span data-ttu-id="77518-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="77518-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77518-129">応答</span><span class="sxs-lookup"><span data-stu-id="77518-129">Response</span></span>
<span data-ttu-id="77518-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="77518-130">If successful, this method returns a `200 OK` response code and a collection of [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77518-131">例</span><span class="sxs-lookup"><span data-stu-id="77518-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="77518-132">要求</span><span class="sxs-lookup"><span data-stu-id="77518-132">Request</span></span>
<span data-ttu-id="77518-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="77518-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="77518-134">応答</span><span class="sxs-lookup"><span data-stu-id="77518-134">Response</span></span>
<span data-ttu-id="77518-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="77518-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 810

{
  "value": [
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
  ]
}
```





