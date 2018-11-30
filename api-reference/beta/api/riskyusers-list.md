---
title: リスト riskyUsers
description: プロパティと、 **riskyUsers**オブジェクトの関係を取得します。
ms.openlocfilehash: 152171ff098bb58e8cbb247ca687841e77594ead
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074464"
---
# <a name="list-riskyusers"></a><span data-ttu-id="40fc0-103">リスト riskyUsers</span><span class="sxs-lookup"><span data-stu-id="40fc0-103">List riskyUsers</span></span>

> <span data-ttu-id="40fc0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="40fc0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40fc0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40fc0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="40fc0-106">プロパティと、 **riskyUsers**オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="40fc0-106">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="40fc0-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="40fc0-107">Permissions</span></span>
<span data-ttu-id="40fc0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="40fc0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40fc0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="40fc0-110">Permission type</span></span>      | <span data-ttu-id="40fc0-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="40fc0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40fc0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="40fc0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="40fc0-113">IdentityriskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="40fc0-113">IdentityriskyUser.Read.All</span></span>    |
|<span data-ttu-id="40fc0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="40fc0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40fc0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40fc0-115">Not supported.</span></span>    |
|<span data-ttu-id="40fc0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="40fc0-116">Application</span></span> | <span data-ttu-id="40fc0-117">IdentityriskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="40fc0-117">IdentityriskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="40fc0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="40fc0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="40fc0-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="40fc0-119">Optional query parameters</span></span>
<span data-ttu-id="40fc0-120">このメソッドをサポートしています`$filter`クエリの応答をカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="40fc0-120">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="40fc0-121">このトピックで後述する例を参照してください。</span><span class="sxs-lookup"><span data-stu-id="40fc0-121">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="40fc0-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40fc0-122">Request headers</span></span>
| <span data-ttu-id="40fc0-123">名前</span><span class="sxs-lookup"><span data-stu-id="40fc0-123">Name</span></span>      |<span data-ttu-id="40fc0-124">説明</span><span class="sxs-lookup"><span data-stu-id="40fc0-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="40fc0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="40fc0-125">Authorization</span></span>  | <span data-ttu-id="40fc0-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="40fc0-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="40fc0-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="40fc0-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="40fc0-p105">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="40fc0-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="40fc0-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="40fc0-131">Request body</span></span>
<span data-ttu-id="40fc0-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="40fc0-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40fc0-133">応答</span><span class="sxs-lookup"><span data-stu-id="40fc0-133">Response</span></span>

<span data-ttu-id="40fc0-134">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[identityRiskEvent](../resources/identityriskevent.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="40fc0-134">If successful, this method returns a `200 OK` response code and [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="40fc0-135">例</span><span class="sxs-lookup"><span data-stu-id="40fc0-135">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="40fc0-136">要求 1</span><span class="sxs-lookup"><span data-stu-id="40fc0-136">Request 1</span></span>
<span data-ttu-id="40fc0-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="40fc0-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers
```
##### <a name="response-1"></a><span data-ttu-id="40fc0-138">応答 1</span><span class="sxs-lookup"><span data-stu-id="40fc0-138">Response 1</span></span>
<span data-ttu-id="40fc0-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="40fc0-139">Here is an example of the response.</span></span>
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
##### <a name="request-2"></a><span data-ttu-id="40fc0-140">要求 2</span><span class="sxs-lookup"><span data-stu-id="40fc0-140">Request 2</span></span>
<span data-ttu-id="40fc0-141">次の例を使用する方法を示しています`$filter`コレクションを取得する、riskyUser の集計が危険度は中です。</span><span class="sxs-lookup"><span data-stu-id="40fc0-141">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
##### <a name="response-2"></a><span data-ttu-id="40fc0-142">応答 2</span><span class="sxs-lookup"><span data-stu-id="40fc0-142">Response 2</span></span>
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
