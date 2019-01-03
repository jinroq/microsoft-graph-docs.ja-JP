---
title: リスト networkIPv6ConfigurationManagementConditions
description: NetworkIPv6ConfigurationManagementCondition オブジェクトのプロパティと関係を一覧表示します。
author: tfitzmac
ms.openlocfilehash: ad138f098413cc09c06bc25e48d603d43f3d45a0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305615"
---
# <a name="list-networkipv6configurationmanagementconditions"></a><span data-ttu-id="6af93-103">リスト networkIPv6ConfigurationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="6af93-103">List networkIPv6ConfigurationManagementConditions</span></span>

> <span data-ttu-id="6af93-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6af93-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6af93-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6af93-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6af93-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6af93-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6af93-107">[NetworkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="6af93-107">List properties and relationships of the [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6af93-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="6af93-108">Prerequisites</span></span>
<span data-ttu-id="6af93-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6af93-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6af93-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6af93-111">Permission type</span></span>|<span data-ttu-id="6af93-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6af93-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6af93-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6af93-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6af93-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6af93-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6af93-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6af93-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6af93-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6af93-116">Not supported.</span></span>|
|<span data-ttu-id="6af93-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6af93-117">Application</span></span>|<span data-ttu-id="6af93-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6af93-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6af93-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6af93-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="6af93-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6af93-120">Request headers</span></span>
|<span data-ttu-id="6af93-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6af93-121">Header</span></span>|<span data-ttu-id="6af93-122">値</span><span class="sxs-lookup"><span data-stu-id="6af93-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6af93-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6af93-123">Authorization</span></span>|<span data-ttu-id="6af93-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="6af93-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6af93-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6af93-125">Accept</span></span>|<span data-ttu-id="6af93-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6af93-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6af93-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="6af93-127">Request body</span></span>
<span data-ttu-id="6af93-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6af93-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6af93-129">応答</span><span class="sxs-lookup"><span data-stu-id="6af93-129">Response</span></span>
<span data-ttu-id="6af93-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="6af93-130">If successful, this method returns a `200 OK` response code and a collection of [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6af93-131">例</span><span class="sxs-lookup"><span data-stu-id="6af93-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6af93-132">要求</span><span class="sxs-lookup"><span data-stu-id="6af93-132">Request</span></span>
<span data-ttu-id="6af93-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6af93-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="6af93-134">応答</span><span class="sxs-lookup"><span data-stu-id="6af93-134">Response</span></span>
<span data-ttu-id="6af93-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6af93-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 760

{
  "value": [
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
  ]
}
```




