---
title: 警告の一覧表示
description: オブジェクトのアラートの一覧を取得します。
ms.openlocfilehash: c25784f62d37722fc997e57b9f15c9857133b964
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022977"
---
# <a name="list-alerts"></a><span data-ttu-id="ec3c1-103">警告の一覧表示</span><span class="sxs-lookup"><span data-stu-id="ec3c1-103">List alerts</span></span>

<span data-ttu-id="ec3c1-104">オブジェクトの[アラート](../resources/alert.md)の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="ec3c1-104">Retrieve a list of [alert](../resources/alert.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec3c1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ec3c1-105">Permissions</span></span>

<span data-ttu-id="ec3c1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ec3c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec3c1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ec3c1-108">Permission type</span></span>      | <span data-ttu-id="ec3c1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ec3c1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec3c1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ec3c1-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="ec3c1-111">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec3c1-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="ec3c1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ec3c1-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ec3c1-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ec3c1-113">Not supported.</span></span>  |
|<span data-ttu-id="ec3c1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ec3c1-114">Application</span></span> | <span data-ttu-id="ec3c1-115">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec3c1-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec3c1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ec3c1-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ec3c1-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ec3c1-117">Optional query parameters</span></span>

<span data-ttu-id="ec3c1-118">このメソッドは、応答をカスタマイズするために次の[OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ec3c1-118">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- <span data-ttu-id="ec3c1-119">`$top`セキュリティ API の各プロバイダーから集計の上位の結果を返します。</span><span class="sxs-lookup"><span data-stu-id="ec3c1-119">`$top` will return the aggregated top results from each security API provider.</span></span>  

<span data-ttu-id="ec3c1-120">OData を使用する別のプロパティ セットを返すには、`$select`する**警告**のプロパティのセットを指定するパラメーター クエリを実行します。</span><span class="sxs-lookup"><span data-stu-id="ec3c1-120">To return an alternative property set, use the OData `$select` query parameter to specify the set of **alert** properties that you want.</span></span>  <span data-ttu-id="ec3c1-121">たとえば、**担当者**、**カテゴリ**、および**重要度**のプロパティを返す、クエリに次を追加: `$select=assignedTo,category,severity`。</span><span class="sxs-lookup"><span data-stu-id="ec3c1-121">For example, to return the **assignedTo**, **category**, and **severity** properties, add the following to your query: `$select=assignedTo,category,severity`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ec3c1-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ec3c1-122">Request headers</span></span>

| <span data-ttu-id="ec3c1-123">名前</span><span class="sxs-lookup"><span data-stu-id="ec3c1-123">Name</span></span>      |<span data-ttu-id="ec3c1-124">説明</span><span class="sxs-lookup"><span data-stu-id="ec3c1-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ec3c1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec3c1-125">Authorization</span></span>  | <span data-ttu-id="ec3c1-p103">Bearer {code}。必須。</span><span class="sxs-lookup"><span data-stu-id="ec3c1-p103">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec3c1-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="ec3c1-128">Request body</span></span>

<span data-ttu-id="ec3c1-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ec3c1-129">Do not supply a request body for this method.</span></span> <span data-ttu-id="ec3c1-130">要求の本体は無視されます。</span><span class="sxs-lookup"><span data-stu-id="ec3c1-130">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="ec3c1-131">応答</span><span class="sxs-lookup"><span data-stu-id="ec3c1-131">Response</span></span>

<span data-ttu-id="ec3c1-132">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の**通知**オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="ec3c1-132">If successful, this method returns a `200 OK` response code and collection of **alert** objects in the response body.</span></span> <span data-ttu-id="ec3c1-133">2 xx または 404 以外のステータス コードは、プロバイダーから返された場合、またはプロバイダーがタイムアウトすると、応答がある場合、`206 Partial Content`警告ヘッダー内のプロバイダーの応答のステータス コード。</span><span class="sxs-lookup"><span data-stu-id="ec3c1-133">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the providers response in a warning header.</span></span> <span data-ttu-id="ec3c1-134">詳細については、 [Microsoft グラフ セキュリティ API のエラー応答](../resources/security-error-codes.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ec3c1-134">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="ec3c1-135">例</span><span class="sxs-lookup"><span data-stu-id="ec3c1-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec3c1-136">要求</span><span class="sxs-lookup"><span data-stu-id="ec3c1-136">Request</span></span>

<span data-ttu-id="ec3c1-137">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ec3c1-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/alerts
```

### <a name="response"></a><span data-ttu-id="ec3c1-138">応答</span><span class="sxs-lookup"><span data-stu-id="ec3c1-138">Response</span></span>

<span data-ttu-id="ec3c1-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ec3c1-139">The following is an example of the response.</span></span>

><span data-ttu-id="ec3c1-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ec3c1-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
