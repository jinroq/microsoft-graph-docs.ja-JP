---
title: リスト suspiciousIpRiskEvents
description: Suspiciousipriskevent オブジェクトのリストを取得します。
ms.openlocfilehash: fe6d14b4f1c7fc1d65b6293de156a63ed2bd15a4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073971"
---
# <a name="list-suspiciousipriskevents"></a><span data-ttu-id="9a77b-103">リスト suspiciousIpRiskEvents</span><span class="sxs-lookup"><span data-stu-id="9a77b-103">List suspiciousIpRiskEvents</span></span>

> <span data-ttu-id="9a77b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9a77b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9a77b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a77b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9a77b-106">Suspiciousipriskevent オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="9a77b-106">Retrieve a list of suspiciousipriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="9a77b-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9a77b-107">Permissions</span></span>
<span data-ttu-id="9a77b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a77b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a77b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9a77b-110">Permission type</span></span>      | <span data-ttu-id="9a77b-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9a77b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a77b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9a77b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9a77b-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a77b-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="9a77b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9a77b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a77b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a77b-115">Not supported.</span></span>    |
|<span data-ttu-id="9a77b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9a77b-116">Application</span></span> | <span data-ttu-id="9a77b-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a77b-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a77b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9a77b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /suspiciousIpRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="9a77b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a77b-119">Request headers</span></span>
| <span data-ttu-id="9a77b-120">名前</span><span class="sxs-lookup"><span data-stu-id="9a77b-120">Name</span></span>      |<span data-ttu-id="9a77b-121">説明</span><span class="sxs-lookup"><span data-stu-id="9a77b-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9a77b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a77b-122">Authorization</span></span>  | <span data-ttu-id="9a77b-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9a77b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9a77b-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9a77b-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="9a77b-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="9a77b-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a77b-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="9a77b-128">Request body</span></span>
<span data-ttu-id="9a77b-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9a77b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a77b-130">応答</span><span class="sxs-lookup"><span data-stu-id="9a77b-130">Response</span></span>

<span data-ttu-id="9a77b-131">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="9a77b-131">If successful, this method returns a `200 OK` response code and collection of [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9a77b-132">例</span><span class="sxs-lookup"><span data-stu-id="9a77b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a77b-133">要求</span><span class="sxs-lookup"><span data-stu-id="9a77b-133">Request</span></span>
<span data-ttu-id="9a77b-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9a77b-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_suspiciousipriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/suspiciousIpRiskEvents
```
##### <a name="response"></a><span data-ttu-id="9a77b-135">応答</span><span class="sxs-lookup"><span data-stu-id="9a77b-135">Response</span></span>
<span data-ttu-id="9a77b-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9a77b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.suspiciousIpRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 290

{
  "value": [
    {
      "closedDateTime": null,
      "createdDateTime": "2016-02-03T06:08:35.123512Z",
      "id": "02e8bfd1-5231-1006-01cc-434f84e0859e-97b7301f-bc05-8e2c-fdfa-2004eb66ff70-287e7b9b-1d60-aa96-6ddb-65c81ee31475",
      "ipAddress": "95.31.18.119",
      "location": "Moskva, Russia, RU",
      "riskEventDateTime": "2016-02-03T05:33:49.9516789Z",
      "riskEventStatus": "active",
      "riskLevel": "low",
      "riskType": "SuspiciousIpRiskEvent",
      "userDisplayName": "Jon Doe",
      "userId": "97b7301f-bc05-8e2c-fdfa-2004eb66ff70",
      "userPrincipalName": "jon@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List suspiciousIpRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->