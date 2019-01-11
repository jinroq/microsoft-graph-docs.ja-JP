---
title: リスト anonymousIpRiskEvents
description: Anonymousipriskevent オブジェクトのリストを取得します。
localization_priority: Normal
ms.openlocfilehash: 83aa906a936d1a33657446f69d512ecd3a0e6e88
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854916"
---
# <a name="list-anonymousipriskevents"></a><span data-ttu-id="dab8f-103">リスト anonymousIpRiskEvents</span><span class="sxs-lookup"><span data-stu-id="dab8f-103">List anonymousIpRiskEvents</span></span>

> <span data-ttu-id="dab8f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dab8f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dab8f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dab8f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dab8f-106">Anonymousipriskevent オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="dab8f-106">Retrieve a list of anonymousipriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="dab8f-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dab8f-107">Permissions</span></span>
<span data-ttu-id="dab8f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dab8f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dab8f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dab8f-110">Permission type</span></span>      | <span data-ttu-id="dab8f-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dab8f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dab8f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dab8f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dab8f-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="dab8f-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="dab8f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dab8f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dab8f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dab8f-115">Not supported.</span></span>    |
|<span data-ttu-id="dab8f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dab8f-116">Application</span></span> | <span data-ttu-id="dab8f-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="dab8f-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dab8f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dab8f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /anonymousIpRiskEvents
```

## <a name="request-headers"></a><span data-ttu-id="dab8f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dab8f-119">Request headers</span></span>
| <span data-ttu-id="dab8f-120">名前</span><span class="sxs-lookup"><span data-stu-id="dab8f-120">Name</span></span>      |<span data-ttu-id="dab8f-121">説明</span><span class="sxs-lookup"><span data-stu-id="dab8f-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dab8f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dab8f-122">Authorization</span></span>  | <span data-ttu-id="dab8f-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="dab8f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dab8f-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dab8f-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="dab8f-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="dab8f-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dab8f-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="dab8f-128">Request body</span></span>
<span data-ttu-id="dab8f-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="dab8f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dab8f-130">応答</span><span class="sxs-lookup"><span data-stu-id="dab8f-130">Response</span></span>

<span data-ttu-id="dab8f-131">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[anonymousIpRiskEvent](../resources/anonymousipriskevent.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="dab8f-131">If successful, this method returns a `200 OK` response code and collection of [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dab8f-132">例</span><span class="sxs-lookup"><span data-stu-id="dab8f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dab8f-133">要求</span><span class="sxs-lookup"><span data-stu-id="dab8f-133">Request</span></span>
<span data-ttu-id="dab8f-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dab8f-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_anonymousipriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/anonymousIpRiskEvents
```
##### <a name="response"></a><span data-ttu-id="dab8f-135">応答</span><span class="sxs-lookup"><span data-stu-id="dab8f-135">Response</span></span>
<span data-ttu-id="dab8f-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dab8f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.anonymousIpRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 290

{
  "value": [
    {
      "closedDateTime": "2016-01-29T20:03:57.7872426Z",
      "createdDateTime": "2016-01-29T00:01:49.126468Z",
      "id": "2016-01-29T00:00:56.22556656a56d0b2-3c51-7c5e-bc1a-1ccdb3bd9c71",
      "ipAddress": null,
      "location": null,
      "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
      "riskEventStatus": "remediated",
      "riskLevel": "medium",
      "riskType": "AnonymousIpRiskEvent",
      "userDisplayName": "Jon Doe",
      "userId": "6a56d0b2-3c51-7c5e-bc1a-1ccdb3bd9c71",
      "userPrincipalName": "jon@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List anonymousIpRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
