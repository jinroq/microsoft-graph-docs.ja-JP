---
title: リスト riskyUsers
description: '**riskyUsers**オブジェクトのプロパティとリレーションシップを取得します。'
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a902daf00f80470e1ac9a83a287eac507d55e171
ms.sourcegitcommit: fd9f62fd9a6d311f98afe2e31afca8b818c402c2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/30/2019
ms.locfileid: "31003728"
---
# <a name="list-riskyusers"></a><span data-ttu-id="2db6d-103">リスト riskyUsers</span><span class="sxs-lookup"><span data-stu-id="2db6d-103">List riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2db6d-104">**riskyUsers**オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="2db6d-104">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>

><span data-ttu-id="2db6d-105">**注:** riskyUsers API を使用するには、Azure AD Premium P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="2db6d-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="2db6d-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2db6d-106">Permissions</span></span>
<span data-ttu-id="2db6d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2db6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2db6d-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2db6d-109">Permission type</span></span>      | <span data-ttu-id="2db6d-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2db6d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2db6d-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2db6d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2db6d-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="2db6d-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="2db6d-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2db6d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2db6d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2db6d-114">Not supported.</span></span>    |
|<span data-ttu-id="2db6d-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2db6d-115">Application</span></span> | <span data-ttu-id="2db6d-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="2db6d-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2db6d-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2db6d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2db6d-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2db6d-118">Optional query parameters</span></span>
<span data-ttu-id="2db6d-119">このメソッドは`$filter` 、クエリ応答をカスタマイズするためにサポートされています。</span><span class="sxs-lookup"><span data-stu-id="2db6d-119">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="2db6d-120">このトピックの後半の例を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2db6d-120">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="2db6d-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2db6d-121">Request headers</span></span>
| <span data-ttu-id="2db6d-122">名前</span><span class="sxs-lookup"><span data-stu-id="2db6d-122">Name</span></span>      |<span data-ttu-id="2db6d-123">説明</span><span class="sxs-lookup"><span data-stu-id="2db6d-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2db6d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2db6d-124">Authorization</span></span>  | <span data-ttu-id="2db6d-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2db6d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2db6d-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2db6d-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="2db6d-128">変更を保存するかどうかを決定するブックセッション ID。</span><span class="sxs-lookup"><span data-stu-id="2db6d-128">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="2db6d-129">省略可能。</span><span class="sxs-lookup"><span data-stu-id="2db6d-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2db6d-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="2db6d-130">Request body</span></span>
<span data-ttu-id="2db6d-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2db6d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2db6d-132">応答</span><span class="sxs-lookup"><span data-stu-id="2db6d-132">Response</span></span>

<span data-ttu-id="2db6d-133">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[identityRiskEvent](../resources/identityriskevent.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2db6d-133">If successful, this method returns a `200 OK` response code and an [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="2db6d-134">例</span><span class="sxs-lookup"><span data-stu-id="2db6d-134">Examples</span></span>
#### <a name="example-1-list-risky-users"></a><span data-ttu-id="2db6d-135">例 1: リスクの高いユーザーの一覧を表示する</span><span class="sxs-lookup"><span data-stu-id="2db6d-135">Example 1: List risky users</span></span>
<span data-ttu-id="2db6d-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2db6d-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers
```

<span data-ttu-id="2db6d-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="2db6d-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUsers"
} -->
```http
HTTP/1.1 200 OK
{
  "id": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
  "riskLastUpdatedDateTime": "2016-01-29T20:03:57.7872426Z",
  "isGuest": "true",
  "isProcessing": true,
  "isDeleted": "true",
  "riskDetail": "adminConfirmedSigninCompromised",
  "riskLevel": "high",
  "riskState": "atRisk"
  "userDisplayName": "Jon Doe",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
#### <a name="example-2-list-risky-users-and-filter-the-results"></a><span data-ttu-id="2db6d-138">例 2: 危険性のあるユーザーを一覧表示し、結果をフィルター処理する</span><span class="sxs-lookup"><span data-stu-id="2db6d-138">Example 2: List risky users and filter the results</span></span>
<span data-ttu-id="2db6d-139">次の例は、を使用`$filter`して、集計リスクレベルが Medium である riskyUser のコレクションを取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="2db6d-139">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
<span data-ttu-id="2db6d-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="2db6d-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUsers"
} -->
```http
HTTP/1.1 200 OK
{
      "id": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
      "riskLastUpdatedDateTime": "2018-09-22T00:04:49.1195968Z",
      "isGuest": false,
      "isProcessing": true,
      "isDeleted": false,
      "riskDetail": "none",
      "riskLevel": "medium",
      "riskState": "atRisk",
      "userDisplayName": "Jon Doe",
      "userPrincipalName": "jon@contoso.com",
      }
    }
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
