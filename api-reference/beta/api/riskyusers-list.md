---
title: リスト riskyUsers
description: '**RiskyUser**オブジェクトのコレクションのプロパティとリレーションシップを取得します。'
localization_priority: Normal
author: cloudhandler
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cb29c5845c8243a046a563351d4b1e486d38c029
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358203"
---
# <a name="list-riskyusers"></a><span data-ttu-id="bbb39-103">リスト riskyUsers</span><span class="sxs-lookup"><span data-stu-id="bbb39-103">List riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbb39-104">**RiskyUser**オブジェクトのコレクションのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="bbb39-104">Retrieve the properties and relationships of a collection of **riskyUser** objects.</span></span>

><span data-ttu-id="bbb39-105">**注:** RiskyUsers API を使用するには、Azure AD Premium P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="bbb39-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbb39-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bbb39-106">Permissions</span></span>
<span data-ttu-id="bbb39-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bbb39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbb39-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bbb39-109">Permission type</span></span>      | <span data-ttu-id="bbb39-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bbb39-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bbb39-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bbb39-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bbb39-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbb39-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="bbb39-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bbb39-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbb39-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bbb39-114">Not supported.</span></span>    |
|<span data-ttu-id="bbb39-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bbb39-115">Application</span></span> | <span data-ttu-id="bbb39-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbb39-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bbb39-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bbb39-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bbb39-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="bbb39-118">Optional query parameters</span></span>
<span data-ttu-id="bbb39-119">このメソッドは`$filter` 、クエリ応答をカスタマイズするためにサポートされています。</span><span class="sxs-lookup"><span data-stu-id="bbb39-119">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="bbb39-120">このトピックの後半の例を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bbb39-120">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="bbb39-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bbb39-121">Request headers</span></span>
| <span data-ttu-id="bbb39-122">名前</span><span class="sxs-lookup"><span data-stu-id="bbb39-122">Name</span></span>      |<span data-ttu-id="bbb39-123">説明</span><span class="sxs-lookup"><span data-stu-id="bbb39-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bbb39-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbb39-124">Authorization</span></span>  | <span data-ttu-id="bbb39-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bbb39-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bbb39-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bbb39-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="bbb39-128">変更を保存するかどうかを決定するブックセッション ID。</span><span class="sxs-lookup"><span data-stu-id="bbb39-128">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="bbb39-129">省略可能。</span><span class="sxs-lookup"><span data-stu-id="bbb39-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbb39-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="bbb39-130">Request body</span></span>
<span data-ttu-id="bbb39-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bbb39-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbb39-132">応答</span><span class="sxs-lookup"><span data-stu-id="bbb39-132">Response</span></span>
<span data-ttu-id="bbb39-133">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[riskyUser](../resources/riskyuser.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="bbb39-133">If successful, this method returns a `200 OK` response code and a collection of [riskyUser](../resources/riskyuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bbb39-134">例</span><span class="sxs-lookup"><span data-stu-id="bbb39-134">Examples</span></span>
### <a name="example-1-list-risky-users"></a><span data-ttu-id="bbb39-135">例 1: リスクの高いユーザーの一覧を表示する</span><span class="sxs-lookup"><span data-stu-id="bbb39-135">Example 1: List risky users</span></span>
#### <a name="request"></a><span data-ttu-id="bbb39-136">要求</span><span class="sxs-lookup"><span data-stu-id="bbb39-136">Request</span></span>
<span data-ttu-id="bbb39-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bbb39-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bbb39-138">プロトコル</span><span class="sxs-lookup"><span data-stu-id="bbb39-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bbb39-139">C#</span><span class="sxs-lookup"><span data-stu-id="bbb39-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-riskyusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bbb39-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bbb39-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-riskyusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bbb39-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="bbb39-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-riskyusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bbb39-142">Java</span><span class="sxs-lookup"><span data-stu-id="bbb39-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-riskyusers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="bbb39-143">応答</span><span class="sxs-lookup"><span data-stu-id="bbb39-143">Response</span></span>
<span data-ttu-id="bbb39-144">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="bbb39-144">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.riskyUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
        {
            "id": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
            "riskLastUpdatedDateTime": "2016-01-29T20:03:57.7872426Z",
            "isGuest": true,
            "isProcessing": true,
            "isDeleted": true,
            "riskDetail": "adminConfirmedSigninCompromised",
            "riskLevel": "high",
            "riskState": "atRisk",
            "userDisplayName": "Alex Wilbur",
            "userPrincipalName": "alexw@contoso.com"
        }
    ]
}
```

### <a name="example-2-list-risky-users-and-filter-the-results"></a><span data-ttu-id="bbb39-145">例 2: 危険性のあるユーザーを一覧表示し、結果をフィルター処理する</span><span class="sxs-lookup"><span data-stu-id="bbb39-145">Example 2: List risky users and filter the results</span></span>
#### <a name="request"></a><span data-ttu-id="bbb39-146">要求</span><span class="sxs-lookup"><span data-stu-id="bbb39-146">Request</span></span>
<span data-ttu-id="bbb39-147">次の例は、を使用`$filter`して、集計リスクレベルが Medium である riskyUser のコレクションを取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="bbb39-147">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bbb39-148">プロトコル</span><span class="sxs-lookup"><span data-stu-id="bbb39-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_filter_riskyusers"
} -->
```http
GET https://graph.microsoft.com/beta/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bbb39-149">C#</span><span class="sxs-lookup"><span data-stu-id="bbb39-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-filter-riskyusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bbb39-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bbb39-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-filter-riskyusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bbb39-151">目的-C</span><span class="sxs-lookup"><span data-stu-id="bbb39-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-filter-riskyusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bbb39-152">Java</span><span class="sxs-lookup"><span data-stu-id="bbb39-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-filter-riskyusers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bbb39-153">応答</span><span class="sxs-lookup"><span data-stu-id="bbb39-153">Response</span></span>
<span data-ttu-id="bbb39-154">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="bbb39-154">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.riskyUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
            "riskLastUpdatedDateTime": "2018-09-22T00:04:49.1195968Z",
            "isGuest": false,
            "isProcessing": true,
            "isDeleted": false,
            "riskDetail": "none",
            "riskLevel": "medium",
            "riskState": "atRisk",
            "userDisplayName": "Alex Wilbur",
            "userPrincipalName": "alexw@contoso.com",
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
