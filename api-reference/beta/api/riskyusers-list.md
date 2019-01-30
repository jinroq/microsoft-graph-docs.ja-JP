---
title: リスト riskyUsers
description: プロパティと、 **riskyUsers**オブジェクトの関係を取得します。
localization_priority: Normal
author: cloudhandler
ms.prod: security
ms.openlocfilehash: 5c0c0557a5cd84312ef9d6381d8cf3018ab8ce7d
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640939"
---
# <a name="list-riskyusers"></a><span data-ttu-id="92000-103">リスト riskyUsers</span><span class="sxs-lookup"><span data-stu-id="92000-103">List riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92000-104">プロパティと、 **riskyUsers**オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="92000-104">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>

> <span data-ttu-id="92000-105">**注:** この API には、Azure AD プレミアム P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="92000-105">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="92000-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="92000-106">Permissions</span></span>
<span data-ttu-id="92000-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="92000-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92000-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="92000-109">Permission type</span></span>      | <span data-ttu-id="92000-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="92000-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92000-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="92000-111">Delegated (work or school account)</span></span> | <span data-ttu-id="92000-112">IdentityriskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="92000-112">IdentityriskyUser.Read.All</span></span>    |
|<span data-ttu-id="92000-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="92000-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92000-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92000-114">Not supported.</span></span>    |
|<span data-ttu-id="92000-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="92000-115">Application</span></span> | <span data-ttu-id="92000-116">IdentityriskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="92000-116">IdentityriskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="92000-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="92000-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="92000-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="92000-118">Optional query parameters</span></span>
<span data-ttu-id="92000-119">このメソッドをサポートしています`$filter`クエリの応答をカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="92000-119">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="92000-120">このトピックで後述する例を参照してください。</span><span class="sxs-lookup"><span data-stu-id="92000-120">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="92000-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="92000-121">Request headers</span></span>
| <span data-ttu-id="92000-122">名前</span><span class="sxs-lookup"><span data-stu-id="92000-122">Name</span></span>      |<span data-ttu-id="92000-123">説明</span><span class="sxs-lookup"><span data-stu-id="92000-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="92000-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="92000-124">Authorization</span></span>  | <span data-ttu-id="92000-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="92000-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="92000-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="92000-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="92000-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="92000-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="92000-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="92000-130">Request body</span></span>
<span data-ttu-id="92000-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="92000-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92000-132">応答</span><span class="sxs-lookup"><span data-stu-id="92000-132">Response</span></span>

<span data-ttu-id="92000-133">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[identityRiskEvent](../resources/identityriskevent.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="92000-133">If successful, this method returns a `200 OK` response code and [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="92000-134">例</span><span class="sxs-lookup"><span data-stu-id="92000-134">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="92000-135">要求 1</span><span class="sxs-lookup"><span data-stu-id="92000-135">Request 1</span></span>
<span data-ttu-id="92000-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="92000-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers
```
##### <a name="response-1"></a><span data-ttu-id="92000-137">応答 1</span><span class="sxs-lookup"><span data-stu-id="92000-137">Response 1</span></span>
<span data-ttu-id="92000-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="92000-138">Here is an example of the response.</span></span>
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
##### <a name="request-2"></a><span data-ttu-id="92000-139">要求 2</span><span class="sxs-lookup"><span data-stu-id="92000-139">Request 2</span></span>
<span data-ttu-id="92000-140">次の例を使用する方法を示しています`$filter`コレクションを取得する、riskyUser の集計が危険度は中です。</span><span class="sxs-lookup"><span data-stu-id="92000-140">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
##### <a name="response-2"></a><span data-ttu-id="92000-141">応答 2</span><span class="sxs-lookup"><span data-stu-id="92000-141">Response 2</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/riskyusers-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
