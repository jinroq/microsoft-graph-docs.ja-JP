---
title: identityRiskEvent を取得する
description: Identityriskevent オブジェクトのプロパティとリレーションシップを取得します。
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: bf951b88e61077e606586b24e4ea24f45b47df59
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33592142"
---
# <a name="get-identityriskevent"></a><span data-ttu-id="3d1be-103">identityRiskEvent を取得する</span><span class="sxs-lookup"><span data-stu-id="3d1be-103">Get identityRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d1be-104">Identityriskevent オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="3d1be-104">Retrieve the properties and relationships of identityriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3d1be-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3d1be-105">Permissions</span></span>
<span data-ttu-id="3d1be-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3d1be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d1be-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3d1be-108">Permission type</span></span>      | <span data-ttu-id="3d1be-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3d1be-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d1be-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3d1be-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3d1be-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d1be-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="3d1be-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3d1be-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d1be-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3d1be-113">Not supported.</span></span>    |
|<span data-ttu-id="3d1be-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3d1be-114">Application</span></span> | <span data-ttu-id="3d1be-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d1be-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d1be-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3d1be-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3d1be-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3d1be-117">Request headers</span></span>
| <span data-ttu-id="3d1be-118">名前</span><span class="sxs-lookup"><span data-stu-id="3d1be-118">Name</span></span>      |<span data-ttu-id="3d1be-119">説明</span><span class="sxs-lookup"><span data-stu-id="3d1be-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3d1be-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d1be-120">Authorization</span></span>  | <span data-ttu-id="3d1be-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3d1be-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3d1be-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3d1be-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="3d1be-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="3d1be-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d1be-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3d1be-126">Request body</span></span>
<span data-ttu-id="3d1be-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3d1be-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d1be-128">応答</span><span class="sxs-lookup"><span data-stu-id="3d1be-128">Response</span></span>

<span data-ttu-id="3d1be-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[identityRiskEvent](../resources/identityriskevent.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3d1be-129">If successful, this method returns a `200 OK` response code and [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3d1be-130">例</span><span class="sxs-lookup"><span data-stu-id="3d1be-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3d1be-131">要求</span><span class="sxs-lookup"><span data-stu-id="3d1be-131">Request</span></span>
<span data-ttu-id="3d1be-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3d1be-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/identityRiskEvents/ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-c2b6c2b9-dddc-acd0-2b39-d519d803dbc3-db69711e-9324-ec99-f010-6e63fb972e98
```
##### <a name="response"></a><span data-ttu-id="3d1be-133">応答</span><span class="sxs-lookup"><span data-stu-id="3d1be-133">Response</span></span>
<span data-ttu-id="3d1be-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3d1be-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="3d1be-137">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="3d1be-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3d1be-138">Visual</span><span class="sxs-lookup"><span data-stu-id="3d1be-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_identityriskevent-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3d1be-139">Java</span><span class="sxs-lookup"><span data-stu-id="3d1be-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_identityriskevent-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/identityriskevent-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/identityriskevent-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
