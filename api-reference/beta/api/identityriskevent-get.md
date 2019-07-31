---
title: identityRiskEvent を取得する
description: Identityriskevent オブジェクトのプロパティとリレーションシップを取得します。
author: cloudhandler
localization_priority: Normal
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 60749f5b4932ece77a4db6e6bf6c66e47d55e60f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35953165"
---
# <a name="get-identityriskevent"></a><span data-ttu-id="cedf1-103">identityRiskEvent を取得する</span><span class="sxs-lookup"><span data-stu-id="cedf1-103">Get identityRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cedf1-104">Identityriskevent オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="cedf1-104">Retrieve the properties and relationships of identityriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="cedf1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cedf1-105">Permissions</span></span>
<span data-ttu-id="cedf1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cedf1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cedf1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cedf1-108">Permission type</span></span>      | <span data-ttu-id="cedf1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cedf1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cedf1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cedf1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cedf1-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="cedf1-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="cedf1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cedf1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cedf1-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cedf1-113">Not supported.</span></span>    |
|<span data-ttu-id="cedf1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cedf1-114">Application</span></span> | <span data-ttu-id="cedf1-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="cedf1-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cedf1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cedf1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="cedf1-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cedf1-117">Request headers</span></span>
| <span data-ttu-id="cedf1-118">名前</span><span class="sxs-lookup"><span data-stu-id="cedf1-118">Name</span></span>      |<span data-ttu-id="cedf1-119">説明</span><span class="sxs-lookup"><span data-stu-id="cedf1-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cedf1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cedf1-120">Authorization</span></span>  | <span data-ttu-id="cedf1-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cedf1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cedf1-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cedf1-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="cedf1-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="cedf1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cedf1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="cedf1-126">Request body</span></span>
<span data-ttu-id="cedf1-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cedf1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cedf1-128">応答</span><span class="sxs-lookup"><span data-stu-id="cedf1-128">Response</span></span>

<span data-ttu-id="cedf1-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[identityRiskEvent](../resources/identityriskevent.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cedf1-129">If successful, this method returns a `200 OK` response code and [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cedf1-130">例</span><span class="sxs-lookup"><span data-stu-id="cedf1-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cedf1-131">要求</span><span class="sxs-lookup"><span data-stu-id="cedf1-131">Request</span></span>
<span data-ttu-id="cedf1-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cedf1-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cedf1-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="cedf1-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/identityRiskEvents/ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-c2b6c2b9-dddc-acd0-2b39-d519d803dbc3-db69711e-9324-ec99-f010-6e63fb972e98
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cedf1-134">C#</span><span class="sxs-lookup"><span data-stu-id="cedf1-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityriskevent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cedf1-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="cedf1-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityriskevent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cedf1-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="cedf1-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityriskevent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cedf1-137">Java</span><span class="sxs-lookup"><span data-stu-id="cedf1-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityriskevent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cedf1-138">応答</span><span class="sxs-lookup"><span data-stu-id="cedf1-138">Response</span></span>
<span data-ttu-id="cedf1-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cedf1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "@odata.type": "#microsoft.graph.unfamiliarLocationRiskEvent",
  "closedDateTime": "2016-01-29T20:03:57.7872426Z",
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-c2b6c2b9-dddc-acd0-2b39-d519d803dbc3-db69711e-9324-ec99-f010-6e63fb972e98",
  "ipAddress": "176.10.104.240",
  "location": "Bern, CH",
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "remediated",
  "riskLevel": "medium",
  "riskType": "UnfamiliarLocationRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get identityRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
