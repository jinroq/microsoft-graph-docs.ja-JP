---
title: リスト riskyUsers
description: プロパティと、 **riskyUsers**オブジェクトの関係を取得します。
localization_priority: Normal
ms.openlocfilehash: bc5023df014e2abc1e7b510bc10a051f6b725e3b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835239"
---
# <a name="list-riskyusers"></a><span data-ttu-id="78bc9-103">リスト riskyUsers</span><span class="sxs-lookup"><span data-stu-id="78bc9-103">List riskyUsers</span></span>

> <span data-ttu-id="78bc9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="78bc9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78bc9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78bc9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="78bc9-106">プロパティと、 **riskyUsers**オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="78bc9-106">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>

> <span data-ttu-id="78bc9-107">**注:** この API には、Azure AD プレミアム P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="78bc9-107">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="78bc9-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="78bc9-108">Permissions</span></span>
<span data-ttu-id="78bc9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="78bc9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78bc9-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="78bc9-111">Permission type</span></span>      | <span data-ttu-id="78bc9-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="78bc9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78bc9-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="78bc9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="78bc9-114">IdentityriskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="78bc9-114">IdentityriskyUser.Read.All</span></span>    |
|<span data-ttu-id="78bc9-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="78bc9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78bc9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78bc9-116">Not supported.</span></span>    |
|<span data-ttu-id="78bc9-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="78bc9-117">Application</span></span> | <span data-ttu-id="78bc9-118">IdentityriskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="78bc9-118">IdentityriskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="78bc9-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="78bc9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="78bc9-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="78bc9-120">Optional query parameters</span></span>
<span data-ttu-id="78bc9-121">このメソッドをサポートしています`$filter`クエリの応答をカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="78bc9-121">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="78bc9-122">このトピックで後述する例を参照してください。</span><span class="sxs-lookup"><span data-stu-id="78bc9-122">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="78bc9-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="78bc9-123">Request headers</span></span>
| <span data-ttu-id="78bc9-124">名前</span><span class="sxs-lookup"><span data-stu-id="78bc9-124">Name</span></span>      |<span data-ttu-id="78bc9-125">説明</span><span class="sxs-lookup"><span data-stu-id="78bc9-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="78bc9-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="78bc9-126">Authorization</span></span>  | <span data-ttu-id="78bc9-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="78bc9-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="78bc9-129">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="78bc9-129">Workbook-Session-Id</span></span>  | <span data-ttu-id="78bc9-p105">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="78bc9-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="78bc9-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="78bc9-132">Request body</span></span>
<span data-ttu-id="78bc9-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="78bc9-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78bc9-134">応答</span><span class="sxs-lookup"><span data-stu-id="78bc9-134">Response</span></span>

<span data-ttu-id="78bc9-135">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[identityRiskEvent](../resources/identityriskevent.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="78bc9-135">If successful, this method returns a `200 OK` response code and [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="78bc9-136">例</span><span class="sxs-lookup"><span data-stu-id="78bc9-136">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="78bc9-137">要求 1</span><span class="sxs-lookup"><span data-stu-id="78bc9-137">Request 1</span></span>
<span data-ttu-id="78bc9-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="78bc9-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers
```
##### <a name="response-1"></a><span data-ttu-id="78bc9-139">応答 1</span><span class="sxs-lookup"><span data-stu-id="78bc9-139">Response 1</span></span>
<span data-ttu-id="78bc9-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="78bc9-140">Here is an example of the response.</span></span>
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
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
##### <a name="request-2"></a><span data-ttu-id="78bc9-141">要求 2</span><span class="sxs-lookup"><span data-stu-id="78bc9-141">Request 2</span></span>
<span data-ttu-id="78bc9-142">次の例を使用する方法を示しています`$filter`コレクションを取得する、riskyUser の集計が危険度は中です。</span><span class="sxs-lookup"><span data-stu-id="78bc9-142">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
##### <a name="response-2"></a><span data-ttu-id="78bc9-143">応答 2</span><span class="sxs-lookup"><span data-stu-id="78bc9-143">Response 2</span></span>
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
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
