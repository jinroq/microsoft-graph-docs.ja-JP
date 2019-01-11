---
title: 警告の一覧表示
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
ms.openlocfilehash: 6036514c2aeabe287fd019ce69157d4b7897af60
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860208"
---
# <a name="list-alerts"></a><span data-ttu-id="fbb02-104">警告の一覧表示</span><span class="sxs-lookup"><span data-stu-id="fbb02-104">List alerts</span></span>

 > <span data-ttu-id="fbb02-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fbb02-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fbb02-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fbb02-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fbb02-107">オブジェクトの[アラート](../resources/alert.md)の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="fbb02-107">Retrieve a list of [alert](../resources/alert.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="fbb02-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fbb02-108">Permissions</span></span>

<span data-ttu-id="fbb02-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fbb02-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbb02-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fbb02-111">Permission type</span></span>      | <span data-ttu-id="fbb02-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fbb02-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fbb02-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fbb02-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="fbb02-114">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbb02-114">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="fbb02-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fbb02-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="fbb02-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fbb02-116">Not supported.</span></span>  |
|<span data-ttu-id="fbb02-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fbb02-117">Application</span></span> | <span data-ttu-id="fbb02-118">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbb02-118">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fbb02-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fbb02-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fbb02-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="fbb02-120">Optional query parameters</span></span>

<span data-ttu-id="fbb02-121">このメソッドは、応答をカスタマイズするために次の[OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="fbb02-121">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- <span data-ttu-id="fbb02-122">`$top`セキュリティ API の各プロバイダーから集計の上位の結果を返します。</span><span class="sxs-lookup"><span data-stu-id="fbb02-122">`$top` will return the aggregated top results from each security API provider.</span></span>  

<span data-ttu-id="fbb02-123">OData を使用する別のプロパティ セットを返すには、`$select`する**警告**のプロパティのセットを指定するパラメーター クエリを実行します。</span><span class="sxs-lookup"><span data-stu-id="fbb02-123">To return an alternative property set, use the OData `$select` query parameter to specify the set of **alert** properties that you want.</span></span>  <span data-ttu-id="fbb02-124">たとえば、**担当者**、**カテゴリ**、および**重要度**のプロパティを返す、クエリに次を追加: `$select=assignedTo,category,severity`。</span><span class="sxs-lookup"><span data-stu-id="fbb02-124">For example, to return the **assignedTo**, **category**, and **severity** properties, add the following to your query: `$select=assignedTo,category,severity`.</span></span>

> <span data-ttu-id="fbb02-125">**注:**`$top` 1000 の警告との組み合わせの制限が`$top`  +  `$skip` 6000 のアラートを超えることはできません。</span><span class="sxs-lookup"><span data-stu-id="fbb02-125">**Note:** `$top` has a limit of 1000 alerts, and a combination of `$top` + `$skip` cannot exceed 6000 alerts.</span></span> <span data-ttu-id="fbb02-126">などの`/security/alerts?$top=10&$skip=5990`を返します、`200 OK`応答コードの場合が、`/security/alerts?$top=10&$skip=5991`を返します、`400 Bad Request`応答コード。</span><span class="sxs-lookup"><span data-stu-id="fbb02-126">For example, `/security/alerts?$top=10&$skip=5990` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=5991` will return a `400 Bad Request` response code.</span></span>  <span data-ttu-id="fbb02-127">詳細については、 [Microsoft グラフ セキュリティ API のエラー応答](../resources/security-error-codes.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fbb02-127">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fbb02-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fbb02-128">Request headers</span></span>

| <span data-ttu-id="fbb02-129">名前</span><span class="sxs-lookup"><span data-stu-id="fbb02-129">Name</span></span>      |<span data-ttu-id="fbb02-130">説明</span><span class="sxs-lookup"><span data-stu-id="fbb02-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fbb02-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbb02-131">Authorization</span></span>  | <span data-ttu-id="fbb02-p106">Bearer {code}。必須。</span><span class="sxs-lookup"><span data-stu-id="fbb02-p106">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbb02-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="fbb02-134">Request body</span></span>

<span data-ttu-id="fbb02-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fbb02-135">Do not supply a request body for this method.</span></span> <span data-ttu-id="fbb02-136">要求の本体は無視されます。</span><span class="sxs-lookup"><span data-stu-id="fbb02-136">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="fbb02-137">応答</span><span class="sxs-lookup"><span data-stu-id="fbb02-137">Response</span></span>

<span data-ttu-id="fbb02-138">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の**通知**オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="fbb02-138">If successful, this method returns a `200 OK` response code and collection of **alert** objects in the response body.</span></span> <span data-ttu-id="fbb02-139">2 xx または 404 以外のステータス コードは、プロバイダーから返された場合、またはプロバイダーがタイムアウトすると、応答がある場合、`206 Partial Content`警告ヘッダー内のプロバイダーの応答のステータス コード。</span><span class="sxs-lookup"><span data-stu-id="fbb02-139">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="fbb02-140">詳細については、 [Microsoft グラフ セキュリティ API のエラー応答](../resources/security-error-codes.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fbb02-140">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="fbb02-141">例</span><span class="sxs-lookup"><span data-stu-id="fbb02-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbb02-142">要求</span><span class="sxs-lookup"><span data-stu-id="fbb02-142">Request</span></span>

<span data-ttu-id="fbb02-143">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fbb02-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```http
GET https://graph.microsoft.com/beta/security/alerts
```

### <a name="response"></a><span data-ttu-id="fbb02-144">応答</span><span class="sxs-lookup"><span data-stu-id="fbb02-144">Response</span></span>

<span data-ttu-id="fbb02-145">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fbb02-145">The following is an example of the response.</span></span>

><span data-ttu-id="fbb02-p109">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="fbb02-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
