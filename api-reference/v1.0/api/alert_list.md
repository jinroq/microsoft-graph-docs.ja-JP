# <a name="list-alerts"></a><span data-ttu-id="7110e-101">警告の一覧表示</span><span class="sxs-lookup"><span data-stu-id="7110e-101">List alerts</span></span>

<span data-ttu-id="7110e-102">オブジェクトの[アラート](../resources/alert.md)の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="7110e-102">Retrieve a list of [alert](../resources/alert.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="7110e-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7110e-103">Permissions</span></span>

<span data-ttu-id="7110e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7110e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7110e-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7110e-106">Permission type</span></span>      | <span data-ttu-id="7110e-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7110e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7110e-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7110e-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="7110e-109">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7110e-109">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="7110e-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7110e-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7110e-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7110e-111">Not supported.</span></span>  |
|<span data-ttu-id="7110e-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7110e-112">Application</span></span> | <span data-ttu-id="7110e-113">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7110e-113">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7110e-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7110e-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7110e-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7110e-115">Optional query parameters</span></span>

<span data-ttu-id="7110e-116">このメソッドは、応答をカスタマイズするために次の[OData クエリ パラメーター](../../../concepts/query_parameters.md)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7110e-116">This method supports the following [OData query parameters](../../../concepts/query_parameters.md) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- <span data-ttu-id="7110e-117">`$top`セキュリティ API の各プロバイダーから集計の上位の結果を返します。</span><span class="sxs-lookup"><span data-stu-id="7110e-117">`$top` will return the aggregated top results from each security API provider.</span></span>  

<span data-ttu-id="7110e-118">OData を使用する別のプロパティ セットを返すには、`$select`する**警告**のプロパティのセットを指定するパラメーター クエリを実行します。</span><span class="sxs-lookup"><span data-stu-id="7110e-118">To return an alternative property set, use the OData `$select` query parameter to specify the set of **alert** properties that you want.</span></span>  <span data-ttu-id="7110e-119">たとえば、**担当者**、**カテゴリ**、および**重要度**のプロパティを返す、クエリに次を追加: `$select=assignedTo,category,severity`。</span><span class="sxs-lookup"><span data-stu-id="7110e-119">For example, to return the **assignedTo**, **category**, and **severity** properties, add the following to your query: `$select=assignedTo,category,severity`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7110e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7110e-120">Request headers</span></span>

| <span data-ttu-id="7110e-121">名前</span><span class="sxs-lookup"><span data-stu-id="7110e-121">Name</span></span>      |<span data-ttu-id="7110e-122">説明</span><span class="sxs-lookup"><span data-stu-id="7110e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7110e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7110e-123">Authorization</span></span>  | <span data-ttu-id="7110e-p103">Bearer {code}。必須。</span><span class="sxs-lookup"><span data-stu-id="7110e-p103">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7110e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7110e-126">Request body</span></span>

<span data-ttu-id="7110e-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7110e-127">Do not supply a request body for this method.</span></span> <span data-ttu-id="7110e-128">要求の本体は無視されます。</span><span class="sxs-lookup"><span data-stu-id="7110e-128">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="7110e-129">応答</span><span class="sxs-lookup"><span data-stu-id="7110e-129">Response</span></span>

<span data-ttu-id="7110e-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の**通知**オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="7110e-130">If successful, this method returns a `200 OK` response code and collection of **alert** objects in the response body.</span></span> <span data-ttu-id="7110e-131">2 xx または 404 以外のステータス コードは、プロバイダーから返された場合、またはプロバイダーがタイムアウトすると、応答がある場合、`206 Partial Content`警告ヘッダー内のプロバイダーの応答のステータス コード。</span><span class="sxs-lookup"><span data-stu-id="7110e-131">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the providers response in a warning header.</span></span> <span data-ttu-id="7110e-132">詳細については、 [Microsoft グラフ セキュリティ API のエラー応答](../resources/security-error-codes.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7110e-132">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="7110e-133">例</span><span class="sxs-lookup"><span data-stu-id="7110e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="7110e-134">要求</span><span class="sxs-lookup"><span data-stu-id="7110e-134">Request</span></span>

<span data-ttu-id="7110e-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7110e-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/alerts
```

### <a name="response"></a><span data-ttu-id="7110e-136">応答</span><span class="sxs-lookup"><span data-stu-id="7110e-136">Response</span></span>

<span data-ttu-id="7110e-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7110e-137">The following is an example of the response.</span></span>

><span data-ttu-id="7110e-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7110e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "activityGroupName": "activityGroupName-value",
      "assignedTo": "assignedTo-value",
      "azureSubscriptionId": "azureSubscriptionId-value",
      "azureTenantId": "azureTenantId-value",
      "category": "category-value",
      "closedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List alerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
