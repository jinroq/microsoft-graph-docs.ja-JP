# <a name="get-alert"></a><span data-ttu-id="d17d0-101">警告の取得</span><span class="sxs-lookup"><span data-stu-id="d17d0-101">Get alert</span></span>

 <span data-ttu-id="d17d0-102">プロパティと[通知](../resources/alert.md)オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="d17d0-102">Retrieve the properties and relationships of an [alert](../resources/alert.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d17d0-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d17d0-103">Permissions</span></span>

<span data-ttu-id="d17d0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d17d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d17d0-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d17d0-106">Permission type</span></span>      | <span data-ttu-id="d17d0-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d17d0-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d17d0-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d17d0-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="d17d0-109">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d17d0-109">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="d17d0-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d17d0-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d17d0-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d17d0-111">Not supported.</span></span>  |
|<span data-ttu-id="d17d0-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d17d0-112">Application</span></span> | <span data-ttu-id="d17d0-113">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d17d0-113">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d17d0-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d17d0-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="d17d0-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d17d0-115">Request headers</span></span>

| <span data-ttu-id="d17d0-116">名前</span><span class="sxs-lookup"><span data-stu-id="d17d0-116">Name</span></span>      |<span data-ttu-id="d17d0-117">説明</span><span class="sxs-lookup"><span data-stu-id="d17d0-117">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d17d0-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="d17d0-118">Authorization</span></span>  | <span data-ttu-id="d17d0-p102">Bearer {code}。必須。</span><span class="sxs-lookup"><span data-stu-id="d17d0-p102">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d17d0-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="d17d0-121">Request body</span></span>

<span data-ttu-id="d17d0-122">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d17d0-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d17d0-123">応答</span><span class="sxs-lookup"><span data-stu-id="d17d0-123">Response</span></span>

<span data-ttu-id="d17d0-124">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**通知**オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="d17d0-124">If successful, this method returns a `200 OK` response code and an **alert** object in the response body.</span></span> <span data-ttu-id="d17d0-125">2 xx または 404 以外のステータス コードは、プロバイダーから返された場合、またはプロバイダーがタイムアウトすると、応答がある場合、`206 Partial Content`警告ヘッダー内のプロバイダーの応答のステータス コード。</span><span class="sxs-lookup"><span data-stu-id="d17d0-125">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the providers response in a warning header.</span></span> <span data-ttu-id="d17d0-126">詳細については、 [Microsoft グラフ セキュリティ API のエラー応答](../resources/security-error-codes.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d17d0-126">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="d17d0-127">例</span><span class="sxs-lookup"><span data-stu-id="d17d0-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="d17d0-128">要求</span><span class="sxs-lookup"><span data-stu-id="d17d0-128">Request</span></span>

<span data-ttu-id="d17d0-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d17d0-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alert"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
```

### <a name="response"></a><span data-ttu-id="d17d0-130">応答</span><span class="sxs-lookup"><span data-stu-id="d17d0-130">Response</span></span>

<span data-ttu-id="d17d0-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d17d0-131">The following is an example of the response.</span></span>
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
  "tocPath": ""
}-->
