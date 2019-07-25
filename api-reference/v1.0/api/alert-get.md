---
title: アラートを取得する
description: " Alert オブジェクトのプロパティと関係を取得します。"
author: preetikr
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 573519edb0346c5d4b6145b7df6a88524737ae8e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882657"
---
# <a name="get-alert"></a><span data-ttu-id="a1235-103">アラートを取得する</span><span class="sxs-lookup"><span data-stu-id="a1235-103">Get alert</span></span>

 <span data-ttu-id="a1235-104">[Alert](../resources/alert.md)オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="a1235-104">Retrieve the properties and relationships of an [alert](../resources/alert.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1235-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a1235-105">Permissions</span></span>

<span data-ttu-id="a1235-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a1235-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1235-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a1235-108">Permission type</span></span>      | <span data-ttu-id="a1235-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a1235-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1235-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a1235-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a1235-111">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1235-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="a1235-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a1235-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a1235-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1235-113">Not supported.</span></span>  |
|<span data-ttu-id="a1235-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a1235-114">Application</span></span> | <span data-ttu-id="a1235-115">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1235-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1235-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a1235-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="a1235-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a1235-117">Request headers</span></span>

| <span data-ttu-id="a1235-118">名前</span><span class="sxs-lookup"><span data-stu-id="a1235-118">Name</span></span>      |<span data-ttu-id="a1235-119">説明</span><span class="sxs-lookup"><span data-stu-id="a1235-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a1235-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1235-120">Authorization</span></span>  | <span data-ttu-id="a1235-121">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="a1235-121">Bearer {code}.</span></span> <span data-ttu-id="a1235-122">必須です。</span><span class="sxs-lookup"><span data-stu-id="a1235-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1235-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="a1235-123">Request body</span></span>

<span data-ttu-id="a1235-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a1235-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1235-125">応答</span><span class="sxs-lookup"><span data-stu-id="a1235-125">Response</span></span>

<span data-ttu-id="a1235-126">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**alert**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a1235-126">If successful, this method returns a `200 OK` response code and an **alert** object in the response body.</span></span> <span data-ttu-id="a1235-127">プロバイダーから 2xx または 404 以外の状態コードが返されるか、プロバイダーがタイムアウトした場合、応答は、警告ヘッダー内のプロバイダーの応答と共に状態コード `206 Partial Content` になります。</span><span class="sxs-lookup"><span data-stu-id="a1235-127">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="a1235-128">詳細については、「[Microsoft グラフ セキュリティ API のエラー応答](../resources/security-error-codes.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a1235-128">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="a1235-129">例</span><span class="sxs-lookup"><span data-stu-id="a1235-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1235-130">要求</span><span class="sxs-lookup"><span data-stu-id="a1235-130">Request</span></span>

<span data-ttu-id="a1235-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a1235-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a1235-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="a1235-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_alert"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a1235-133">C#</span><span class="sxs-lookup"><span data-stu-id="a1235-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-alert-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a1235-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="a1235-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-alert-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a1235-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="a1235-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-alert-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a1235-136">Java</span><span class="sxs-lookup"><span data-stu-id="a1235-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-alert-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a1235-137">応答</span><span class="sxs-lookup"><span data-stu-id="a1235-137">Response</span></span>

<span data-ttu-id="a1235-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a1235-138">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "activityGroupName": "String",
  "assignedTo": "String",
  "azureSubscriptionId": "String",
  "azureTenantId": "String",
  "category": "String",
  "closedDateTime": "String (timestamp)",
  "cloudAppStates": [
    {
      "destinationServiceIp": "String",
      "destinationServiceName": "String",
      "riskScore": "String"
    }
  ],
  "comments": ["String"],
  "confidence": 1024,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "detectionIds": ["String"],
  "eventDateTime": "String (timestamp)",
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "fileStates": [
    {
      "fileHash": {
        "hashType": "@odata.type: microsoft.graph.fileHashType",
        "hashValue": "String"
      },
      "name": "String",
      "path": "String",
      "riskScore": "String"
    }
  ],
  "hostStates": [
    {
      "fqdn": "String",
      "isAzureAadJoined": true,
      "isAzureAadRegistered": true,
      "isHybridAzureDomainJoined": true,
      "netBiosName": "String",
      "os": "String",
      "privateIpAddress": "String",
      "publicIpAddress": "String",
      "riskScore": "String"
    }
  ],
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "malwareStates": [
    {
      "category": "String",
      "family": "String",
      "name": "String",
      "severity": "String",
      "wasRunning": true
    }
  ],
  "networkConnections": [
    {
      "applicationName": "String",
      "destinationAddress": "String",
      "destinationDomain": "String",
      "destinationPort": "String",
      "destinationUrl": "String",
      "direction": "@odata.type: microsoft.graph.connectionDirection",
      "domainRegisteredDateTime": "String (timestamp)",
      "localDnsName": "String",
      "natDestinationAddress": "String",
      "natDestinationPort": "String",
      "natSourceAddress": "String",
      "natSourcePort": "String",
      "protocol": "@odata.type: microsoft.graph.securityNetworkProtocol",
      "riskScore": "String",
      "sourceAddress": "String",
      "sourcePort": "String",
      "status": "@odata.type: microsoft.graph.connectionStatus",
      "urlParameters": "String"
    }
  ],
  "processes": [
    {
      "accountName": "String",
      "commandLine": "String",
      "createdDateTime": "String (timestamp)",
      "fileHash": {
        "hashType": "@odata.type: microsoft.graph.fileHashType",
        "hashValue": "String"
      },
      "integrityLevel": "@odata.type: microsoft.graph.processIntegrityLevel",
      "isElevated": true,
      "name": "String",
      "parentProcessCreatedDateTime": "String (timestamp)",
      "parentProcessId": 1024,
      "parentProcessName": "String",
      "path": "String",
      "processId": 1024
    }
  ],
  "recommendedActions": ["String"],
  "registryKeyStates": [
    {
      "hive": "@odata.type: microsoft.graph.registryHive",
      "key": "String",
      "oldKey": "String",
      "oldValueData": "String",
      "oldValueName": "String",
      "operation": "@odata.type: microsoft.graph.registryOperation",
      "processId": 1024,
      "valueData": "String",
      "valueName": "String",
      "valueType": "@odata.type: microsoft.graph.registryValueType"
    }
  ],
  "severity": "@odata.type: microsoft.graph.alertSeverity",
  "sourceMaterials": ["String"],
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "title": "String",
  "triggers": [
    {
      "name": "String",
      "type": "String",
      "value": "String"
    }
  ],
  "userStates": [
    {
      "aadUserId": "String",
      "accountName": "String",
      "domainName": "String",
      "emailRole": "@odata.type: microsoft.graph.emailRole",
      "isVpn": true,
      "logonDateTime": "String (timestamp)",
      "logonId": "String",
      "logonIp": "String",
      "logonLocation": "String",
      "logonType": "@odata.type: microsoft.graph.logonType",
      "onPremisesSecurityIdentifier": "String",
      "riskScore": "String",
      "userAccountType": "@odata.type: microsoft.graph.userAccountSecurityType",
      "userPrincipalName": "String"
    }
  ],
  "vendorInformation": {
    "provider": "String",
    "providerVersion": "String",
    "subProvider": "String",
    "vendor": "String"
  },
  "vulnerabilityStates": [
    {
      "cve": "String",
      "severity": "String",
      "wasRunning": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get glert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
