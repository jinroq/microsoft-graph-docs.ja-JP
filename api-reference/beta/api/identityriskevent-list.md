---
title: リスト identityRiskEvents
description: Identityriskevent オブジェクトのリストを取得します。
author: cloudhandler
localization_priority: Normal
ms.openlocfilehash: fbd5e739986ded9fa6f5346e35808f4018bff625
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894251"
---
# <a name="list-identityriskevents"></a><span data-ttu-id="e59b2-103">リスト identityRiskEvents</span><span class="sxs-lookup"><span data-stu-id="e59b2-103">List identityRiskEvents</span></span>

> <span data-ttu-id="e59b2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e59b2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e59b2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e59b2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e59b2-106">Identityriskevent オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="e59b2-106">Retrieve a list of identityriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="e59b2-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e59b2-107">Permissions</span></span>
<span data-ttu-id="e59b2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e59b2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e59b2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e59b2-110">Permission type</span></span>      | <span data-ttu-id="e59b2-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e59b2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e59b2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e59b2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e59b2-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="e59b2-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="e59b2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e59b2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e59b2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e59b2-115">Not supported.</span></span>    |
|<span data-ttu-id="e59b2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e59b2-116">Application</span></span> | <span data-ttu-id="e59b2-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="e59b2-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e59b2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e59b2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="e59b2-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e59b2-119">Request headers</span></span>
| <span data-ttu-id="e59b2-120">名前</span><span class="sxs-lookup"><span data-stu-id="e59b2-120">Name</span></span>      |<span data-ttu-id="e59b2-121">説明</span><span class="sxs-lookup"><span data-stu-id="e59b2-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e59b2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e59b2-122">Authorization</span></span>  | <span data-ttu-id="e59b2-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e59b2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e59b2-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e59b2-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="e59b2-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="e59b2-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e59b2-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="e59b2-128">Request body</span></span>
<span data-ttu-id="e59b2-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e59b2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e59b2-130">応答</span><span class="sxs-lookup"><span data-stu-id="e59b2-130">Response</span></span>

<span data-ttu-id="e59b2-131">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[identityRiskEvent](../resources/identityriskevent.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="e59b2-131">If successful, this method returns a `200 OK` response code and collection of [identityRiskEvent](../resources/identityriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e59b2-132">例</span><span class="sxs-lookup"><span data-stu-id="e59b2-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e59b2-133">要求</span><span class="sxs-lookup"><span data-stu-id="e59b2-133">Request</span></span>
<span data-ttu-id="e59b2-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e59b2-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityRiskEvents
```
##### <a name="response"></a><span data-ttu-id="e59b2-135">応答</span><span class="sxs-lookup"><span data-stu-id="e59b2-135">Response</span></span>
<span data-ttu-id="e59b2-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e59b2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List identityRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
