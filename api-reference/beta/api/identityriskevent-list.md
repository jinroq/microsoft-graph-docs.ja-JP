---
title: リスト identityRiskEvents
description: identityriskevent オブジェクトのリストを取得します。
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 3f26b52f988a02e3a3f9f97ca9f78f7d5c8a6cc0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328467"
---
# <a name="list-identityriskevents"></a><span data-ttu-id="af713-103">リスト identityRiskEvents</span><span class="sxs-lookup"><span data-stu-id="af713-103">List identityRiskEvents</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af713-104">identityriskevent オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="af713-104">Retrieve a list of identityriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="af713-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="af713-105">Permissions</span></span>
<span data-ttu-id="af713-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="af713-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af713-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="af713-108">Permission type</span></span>      | <span data-ttu-id="af713-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="af713-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af713-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="af713-110">Delegated (work or school account)</span></span> | <span data-ttu-id="af713-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="af713-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="af713-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="af713-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af713-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af713-113">Not supported.</span></span>    |
|<span data-ttu-id="af713-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="af713-114">Application</span></span> | <span data-ttu-id="af713-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="af713-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="af713-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="af713-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="af713-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="af713-117">Request headers</span></span>
| <span data-ttu-id="af713-118">名前</span><span class="sxs-lookup"><span data-stu-id="af713-118">Name</span></span>      |<span data-ttu-id="af713-119">説明</span><span class="sxs-lookup"><span data-stu-id="af713-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="af713-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="af713-120">Authorization</span></span>  | <span data-ttu-id="af713-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="af713-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="af713-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="af713-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="af713-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="af713-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="af713-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="af713-126">Request body</span></span>
<span data-ttu-id="af713-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="af713-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af713-128">応答</span><span class="sxs-lookup"><span data-stu-id="af713-128">Response</span></span>

<span data-ttu-id="af713-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[identityRiskEvent](../resources/identityriskevent.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="af713-129">If successful, this method returns a `200 OK` response code and collection of [identityRiskEvent](../resources/identityriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="af713-130">例</span><span class="sxs-lookup"><span data-stu-id="af713-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="af713-131">要求</span><span class="sxs-lookup"><span data-stu-id="af713-131">Request</span></span>
<span data-ttu-id="af713-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="af713-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityRiskEvents
```
##### <a name="response"></a><span data-ttu-id="af713-133">応答</span><span class="sxs-lookup"><span data-stu-id="af713-133">Response</span></span>
<span data-ttu-id="af713-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="af713-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.malwareRiskEvent",
      "malwareName": "CONFICKER",
      "closedDateTime": null,
      "createdDateTime": "2016-02-03T06:06:01.940814Z",
      "deviceInformation": "B62XYZ13OX",
      "id": "74ceb0af-2271-9167-ffa0-b6ac3b4e8781-9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89-0fdc2304-ba4c-ac0c-bdd7-da2d10e93849",
      "ipAddress": "95.31.18.119",
      "location": "Moskva, Russia, RU",
      "riskEventDateTime": "2016-02-03T05:20:33.7208156Z",
      "riskEventStatus": "active",
      "riskLevel": "low",
      "riskType": "MalwareRiskEvent",
      "userDisplayName": "Jon Doe",
      "userId": "9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89",
      "userPrincipalName": "jon@contoso.com"
    },
    {
      "@odata.type": "#microsoft.graph.unfamiliarLocationRiskEvent",
      "closedDateTime": "2016-01-29T20:03:57.7872426Z",
      "createdDateTime": "2016-01-29T00:01:49.126468Z",
      "id": "ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89-db69711e-9324-ec99-f010-6e63fb972e98",
      "ipAddress": "176.10.104.240",
      "location": "Bern, CH",
      "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
      "riskEventStatus": "remediated",
      "riskLevel": "medium",
      "riskType": "UnfamiliarLocationRiskEvent",
      "userDisplayName": "Jon Doe",
      "userId": "9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89",
      "userPrincipalName": "jon@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List identityRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
