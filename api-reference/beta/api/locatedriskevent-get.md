---
title: LocatedRiskEvent を取得します。
description: プロパティと、locatedriskevent オブジェクトの関係を取得します。
localization_priority: Normal
ms.openlocfilehash: 428c0cdac81fffc7cfca085922e23beccea82b90
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829149"
---
# <a name="get-locatedriskevent"></a><span data-ttu-id="21343-103">LocatedRiskEvent を取得します。</span><span class="sxs-lookup"><span data-stu-id="21343-103">Get locatedRiskEvent</span></span>

> <span data-ttu-id="21343-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="21343-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21343-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="21343-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="21343-106">プロパティと、locatedriskevent オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="21343-106">Retrieve the properties and relationships of a locatedriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="21343-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="21343-107">Permissions</span></span>
<span data-ttu-id="21343-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="21343-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21343-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="21343-110">Permission type</span></span>      | <span data-ttu-id="21343-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="21343-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21343-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="21343-112">Delegated (work or school account)</span></span> | <span data-ttu-id="21343-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="21343-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="21343-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="21343-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21343-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="21343-115">Not supported.</span></span>    |
|<span data-ttu-id="21343-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="21343-116">Application</span></span> | <span data-ttu-id="21343-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="21343-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="21343-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="21343-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /locatedRiskEvents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="21343-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="21343-119">Request headers</span></span>
| <span data-ttu-id="21343-120">名前</span><span class="sxs-lookup"><span data-stu-id="21343-120">Name</span></span>      |<span data-ttu-id="21343-121">説明</span><span class="sxs-lookup"><span data-stu-id="21343-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="21343-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="21343-122">Authorization</span></span>  | <span data-ttu-id="21343-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="21343-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="21343-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="21343-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="21343-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="21343-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="21343-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="21343-128">Request body</span></span>
<span data-ttu-id="21343-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="21343-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21343-130">応答</span><span class="sxs-lookup"><span data-stu-id="21343-130">Response</span></span>

<span data-ttu-id="21343-131">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[locatedRiskEvent](../resources/locatedriskevent.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="21343-131">If successful, this method returns a `200 OK` response code and [locatedRiskEvent](../resources/locatedriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="21343-132">例</span><span class="sxs-lookup"><span data-stu-id="21343-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="21343-133">要求</span><span class="sxs-lookup"><span data-stu-id="21343-133">Request</span></span>
<span data-ttu-id="21343-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="21343-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_locatedriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/locatedRiskEvents/27b91217-a6ca-edff-da2b-c46feaf0228f-a6653179-3c7b-4e99-bb4c-dddeb18adfc1-42445d4d-fe22-9840-cf9d-72f6ce8cd056
```
##### <a name="response"></a><span data-ttu-id="21343-135">応答</span><span class="sxs-lookup"><span data-stu-id="21343-135">Response</span></span>
<span data-ttu-id="21343-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="21343-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.locatedRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "closedDateTime": "2016-01-29T20:03:57.7872426Z",
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "27b91217-a6ca-edff-da2b-c46feaf0228f-a6653179-3c7b-4e99-bb4c-dddeb18adfc1-42445d4d-fe22-9840-cf9d-72f6ce8cd056",
  "ipAddress": "176.10.104.240",
  "location": "Bern, CH",
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "remediated",
  "riskLevel": "medium",
  "riskType": "UnfamiliarLocationRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "a6653179-3c7b-4e99-bb4c-dddeb18adfc1",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get locatedRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
