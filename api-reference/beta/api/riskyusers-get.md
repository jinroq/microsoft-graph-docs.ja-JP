---
title: RiskyUsers を取得します。
description: プロパティと、 **riskyUsers**オブジェクトの関係を取得します。
ms.openlocfilehash: f0a6ac24bf66184d0547e9284f5a35b84b9358b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067466"
---
# <a name="get-riskyusers"></a><span data-ttu-id="face2-103">RiskyUsers を取得します。</span><span class="sxs-lookup"><span data-stu-id="face2-103">Get riskyUsers</span></span>

> <span data-ttu-id="face2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="face2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="face2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="face2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="face2-106">プロパティと、 **riskyUsers**オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="face2-106">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="face2-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="face2-107">Permissions</span></span>
<span data-ttu-id="face2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="face2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="face2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="face2-110">Permission type</span></span>      | <span data-ttu-id="face2-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="face2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="face2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="face2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="face2-113">IdentityrRskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="face2-113">IdentityrRskyUser.Read.All</span></span>    |
|<span data-ttu-id="face2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="face2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="face2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="face2-115">Not supported.</span></span>    |
|<span data-ttu-id="face2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="face2-116">Application</span></span> | <span data-ttu-id="face2-117">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="face2-117">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="face2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="face2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```


## <a name="request-headers"></a><span data-ttu-id="face2-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="face2-119">Request headers</span></span>
| <span data-ttu-id="face2-120">名前</span><span class="sxs-lookup"><span data-stu-id="face2-120">Name</span></span>      |<span data-ttu-id="face2-121">説明</span><span class="sxs-lookup"><span data-stu-id="face2-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="face2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="face2-122">Authorization</span></span>  | <span data-ttu-id="face2-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="face2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="face2-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="face2-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="face2-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="face2-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="face2-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="face2-128">Request body</span></span>
<span data-ttu-id="face2-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="face2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="face2-130">応答</span><span class="sxs-lookup"><span data-stu-id="face2-130">Response</span></span>

<span data-ttu-id="face2-131">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[riskyUser](../resources/riskyuser.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="face2-131">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="face2-132">例</span><span class="sxs-lookup"><span data-stu-id="face2-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="face2-133">要求</span><span class="sxs-lookup"><span data-stu-id="face2-133">Request</span></span>
<span data-ttu-id="face2-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="face2-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/{id}
```
##### <a name="response"></a><span data-ttu-id="face2-135">応答</span><span class="sxs-lookup"><span data-stu-id="face2-135">Response</span></span>
<span data-ttu-id="face2-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="face2-136">Here is an example of the response.</span></span>
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
