---
title: ImpossibleTravelRiskEvent を取得します。
description: プロパティと impossibletravelriskevent オブジェクトの関係を取得します。
ms.openlocfilehash: 3bb5b052cca79e90c26e7e26f2b9cb798e97680f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069494"
---
# <a name="get-impossibletravelriskevent"></a><span data-ttu-id="08ca7-103">ImpossibleTravelRiskEvent を取得します。</span><span class="sxs-lookup"><span data-stu-id="08ca7-103">Get impossibleTravelRiskEvent</span></span>

> <span data-ttu-id="08ca7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="08ca7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08ca7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="08ca7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="08ca7-106">プロパティと impossibletravelriskevent オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="08ca7-106">Retrieve the properties and relationships of an impossibletravelriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="08ca7-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="08ca7-107">Permissions</span></span>
<span data-ttu-id="08ca7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="08ca7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08ca7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="08ca7-110">Permission type</span></span>      | <span data-ttu-id="08ca7-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="08ca7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08ca7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="08ca7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="08ca7-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="08ca7-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="08ca7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="08ca7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08ca7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="08ca7-115">Not supported.</span></span>    |
|<span data-ttu-id="08ca7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="08ca7-116">Application</span></span> | <span data-ttu-id="08ca7-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="08ca7-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="08ca7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="08ca7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /impossibleTravelRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="08ca7-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="08ca7-119">Request headers</span></span>
| <span data-ttu-id="08ca7-120">名前</span><span class="sxs-lookup"><span data-stu-id="08ca7-120">Name</span></span>      |<span data-ttu-id="08ca7-121">説明</span><span class="sxs-lookup"><span data-stu-id="08ca7-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="08ca7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="08ca7-122">Authorization</span></span>  | <span data-ttu-id="08ca7-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="08ca7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="08ca7-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="08ca7-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="08ca7-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="08ca7-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="08ca7-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="08ca7-128">Request body</span></span>
<span data-ttu-id="08ca7-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="08ca7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08ca7-130">応答</span><span class="sxs-lookup"><span data-stu-id="08ca7-130">Response</span></span>

<span data-ttu-id="08ca7-131">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="08ca7-131">If successful, this method returns a `200 OK` response code and [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="08ca7-132">例</span><span class="sxs-lookup"><span data-stu-id="08ca7-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="08ca7-133">要求</span><span class="sxs-lookup"><span data-stu-id="08ca7-133">Request</span></span>
<span data-ttu-id="08ca7-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="08ca7-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_impossibletravelriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/impossibleTravelRiskEvents/22e65c1f-909a-42b5-c0d2-075f30e27887-0bfdc7a8-6a16-c33e-7de9-a60a28ae533b-15475553-dbc1-8879-5079-23b1edd25bab
```
##### <a name="response"></a><span data-ttu-id="08ca7-135">応答</span><span class="sxs-lookup"><span data-stu-id="08ca7-135">Response</span></span>
<span data-ttu-id="08ca7-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="08ca7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.impossibleTravelRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 260

{
  "@odata.type": "#microsoft.graph.impossibleTravelRiskEvent",
  "closedDateTime": "2016-01-29T20:03:57.7872426Z",
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "22e65c1f-909a-42b5-c0d2-075f30e27887-0bfdc7a8-6a16-c33e-7de9-a60a28ae533b-15475553-dbc1-8879-5079-23b1edd25bab",
  "ipAddress": "176.10.104.240",
  "isAtypicalLocation": true,
  "location": "Bern, CH",
  "previousIPAddress": "95.31.18.119",
  "previousLocation": "Moskva, Russia, RU",
  "previousSigninDateTime": "2016-01-29T00:00:55.3859274Z",
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "remediated",
  "riskLevel": "medium",
  "riskType": "ImpossibleTravelRiskEvent",
  "userAgent": "Firefox 42.0.0.1",
  "userDisplayName": "Jon Doe",
  "userId": "0bfdc7a8-6a16-c33e-7de9-a60a28ae533b",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get impossibleTravelRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
