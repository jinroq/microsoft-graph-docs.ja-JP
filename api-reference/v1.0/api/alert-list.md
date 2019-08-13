---
title: アラートを一覧表示する
description: alert オブジェクトのリストを取得する。
author: preetikr
localization_priority: Priority
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 44fd601cf004237d7cabda967bb99657d4f4bd25
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374000"
---
# <a name="list-alerts"></a><span data-ttu-id="14dcc-103">アラートを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="14dcc-103">List alerts</span></span>

<span data-ttu-id="14dcc-104">[alert](../resources/alert.md) オブジェクトのリストを取得する。</span><span class="sxs-lookup"><span data-stu-id="14dcc-104">Retrieve a list of [alert](../resources/alert.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="14dcc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="14dcc-105">Permissions</span></span>

<span data-ttu-id="14dcc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="14dcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14dcc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="14dcc-108">Permission type</span></span>      | <span data-ttu-id="14dcc-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="14dcc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14dcc-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="14dcc-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="14dcc-111">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14dcc-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="14dcc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="14dcc-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="14dcc-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14dcc-113">Not supported.</span></span>  |
|<span data-ttu-id="14dcc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="14dcc-114">Application</span></span> | <span data-ttu-id="14dcc-115">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14dcc-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="14dcc-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="14dcc-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}' and {property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="14dcc-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="14dcc-117">Optional query parameters</span></span>

<span data-ttu-id="14dcc-118">このメソッドは、応答をカスタマイズするために次の [OData クエリ パラメーター](/graph/query-parameters)をサポートします:</span><span class="sxs-lookup"><span data-stu-id="14dcc-118">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- <span data-ttu-id="14dcc-119">`$top` は、各セキュリティ API プロバイダーから集計された上位の結果を返します。</span><span class="sxs-lookup"><span data-stu-id="14dcc-119">`$top` will return the aggregated top results from each security API provider.</span></span>  

<span data-ttu-id="14dcc-120">別のプロパティ セットを返すには、OData `$select` クエリ パラメーターを使用し、目的の **alert** プロパティのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="14dcc-120">To return an alternative property set, use the OData `$select` query parameter to specify the set of **alert** properties that you want.</span></span>  <span data-ttu-id="14dcc-121">例えば、**assignedTo**、**category**、および **severity** プロパティを返すには、以下をクエリに追加します: `$select=assignedTo,category,severity`。</span><span class="sxs-lookup"><span data-stu-id="14dcc-121">For example, to return the **assignedTo**, **category**, and **severity** properties, add the following to your query: `$select=assignedTo,category,severity`.</span></span>

> <span data-ttu-id="14dcc-122">**注:** `$top` ではアラート数が 1000件に制限され、`$top`  +  `$skip` の組み合わせでのアラート数は 6000 件に制限されます。</span><span class="sxs-lookup"><span data-stu-id="14dcc-122">**Note:** `$top` has a limit of 1000 alerts, and a combination of `$top` + `$skip` cannot exceed 6000 alerts.</span></span> <span data-ttu-id="14dcc-123">例えば、`/security/alerts?$top=10&$skip=5990` は応答コード `200 OK` を返しますが、`/security/alerts?$top=10&$skip=5991` は応答コード `400 Bad Request` を返します。</span><span class="sxs-lookup"><span data-stu-id="14dcc-123">For example, `/security/alerts?$top=10&$skip=5990` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=5991` will return a `400 Bad Request` response code.</span></span>  <span data-ttu-id="14dcc-124">詳細については、「[Microsoft グラフ セキュリティ API のエラー応答](../resources/security-error-codes.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="14dcc-124">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="14dcc-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="14dcc-125">Request headers</span></span>

| <span data-ttu-id="14dcc-126">名前</span><span class="sxs-lookup"><span data-stu-id="14dcc-126">Name</span></span>      |<span data-ttu-id="14dcc-127">説明</span><span class="sxs-lookup"><span data-stu-id="14dcc-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="14dcc-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="14dcc-128">Authorization</span></span>  | <span data-ttu-id="14dcc-129">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="14dcc-129">Bearer {code}.</span></span> <span data-ttu-id="14dcc-130">必須です。</span><span class="sxs-lookup"><span data-stu-id="14dcc-130">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="14dcc-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="14dcc-131">Request body</span></span>

<span data-ttu-id="14dcc-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="14dcc-132">Do not supply a request body for this method.</span></span> <span data-ttu-id="14dcc-133">要求本文は無視されます。</span><span class="sxs-lookup"><span data-stu-id="14dcc-133">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="14dcc-134">応答</span><span class="sxs-lookup"><span data-stu-id="14dcc-134">Response</span></span>

<span data-ttu-id="14dcc-135">成功した場合、このメソッドは応答コード `200 OK` と **alert** オブジェクトのコレクションを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="14dcc-135">If successful, this method returns a `200 OK` response code and collection of **alert** objects in the response body.</span></span> <span data-ttu-id="14dcc-136">プロバイダーから 2xx または 404 以外の状態コードが返されるか、プロバイダーがタイムアウトした場合、応答は、警告ヘッダー内のプロバイダーの応答と共に状態コード `206 Partial Content` になります。</span><span class="sxs-lookup"><span data-stu-id="14dcc-136">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="14dcc-137">詳細については、「[Microsoft グラフ セキュリティ API のエラー応答](../resources/security-error-codes.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="14dcc-137">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="14dcc-138">例</span><span class="sxs-lookup"><span data-stu-id="14dcc-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="14dcc-139">要求</span><span class="sxs-lookup"><span data-stu-id="14dcc-139">Request</span></span>

<span data-ttu-id="14dcc-140">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="14dcc-140">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="14dcc-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="14dcc-141">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/alerts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="14dcc-142">C#</span><span class="sxs-lookup"><span data-stu-id="14dcc-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-alerts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="14dcc-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14dcc-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-alerts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="14dcc-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14dcc-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-alerts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="14dcc-145">Java</span><span class="sxs-lookup"><span data-stu-id="14dcc-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-alerts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="14dcc-146">応答</span><span class="sxs-lookup"><span data-stu-id="14dcc-146">Response</span></span>

<span data-ttu-id="14dcc-147">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="14dcc-147">The following is an example of the response.</span></span>

><span data-ttu-id="14dcc-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="14dcc-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
