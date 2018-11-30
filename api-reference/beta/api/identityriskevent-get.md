---
title: IdentityRiskEvent を取得します。
description: プロパティと identityriskevent オブジェクトの関係を取得します。
ms.openlocfilehash: 3e00f93fc80f68799687ba6e9b1ec25d803779dd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069179"
---
# <a name="get-identityriskevent"></a><span data-ttu-id="3b630-103">IdentityRiskEvent を取得します。</span><span class="sxs-lookup"><span data-stu-id="3b630-103">Get identityRiskEvent</span></span>

> <span data-ttu-id="3b630-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3b630-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b630-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b630-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3b630-106">プロパティと identityriskevent オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="3b630-106">Retrieve the properties and relationships of identityriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3b630-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3b630-107">Permissions</span></span>
<span data-ttu-id="3b630-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3b630-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b630-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3b630-110">Permission type</span></span>      | <span data-ttu-id="3b630-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3b630-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b630-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3b630-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3b630-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b630-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="3b630-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3b630-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b630-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b630-115">Not supported.</span></span>    |
|<span data-ttu-id="3b630-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3b630-116">Application</span></span> | <span data-ttu-id="3b630-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b630-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b630-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3b630-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3b630-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3b630-119">Request headers</span></span>
| <span data-ttu-id="3b630-120">名前</span><span class="sxs-lookup"><span data-stu-id="3b630-120">Name</span></span>      |<span data-ttu-id="3b630-121">説明</span><span class="sxs-lookup"><span data-stu-id="3b630-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3b630-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b630-122">Authorization</span></span>  | <span data-ttu-id="3b630-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3b630-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3b630-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3b630-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="3b630-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="3b630-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b630-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="3b630-128">Request body</span></span>
<span data-ttu-id="3b630-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3b630-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b630-130">応答</span><span class="sxs-lookup"><span data-stu-id="3b630-130">Response</span></span>

<span data-ttu-id="3b630-131">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[identityRiskEvent](../resources/identityriskevent.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="3b630-131">If successful, this method returns a `200 OK` response code and [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3b630-132">例</span><span class="sxs-lookup"><span data-stu-id="3b630-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3b630-133">要求</span><span class="sxs-lookup"><span data-stu-id="3b630-133">Request</span></span>
<span data-ttu-id="3b630-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3b630-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/identityRiskEvents/ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-c2b6c2b9-dddc-acd0-2b39-d519d803dbc3-db69711e-9324-ec99-f010-6e63fb972e98
```
##### <a name="response"></a><span data-ttu-id="3b630-135">応答</span><span class="sxs-lookup"><span data-stu-id="3b630-135">Response</span></span>
<span data-ttu-id="3b630-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3b630-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get identityRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
