---
title: impossibleTravelRiskEvent を取得する
description: Impossibletravelriskevent オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 81487cf62230708d151f67250b9980e18bcbb7c7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35953144"
---
# <a name="get-impossibletravelriskevent"></a><span data-ttu-id="01f4a-103">impossibleTravelRiskEvent を取得する</span><span class="sxs-lookup"><span data-stu-id="01f4a-103">Get impossibleTravelRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01f4a-104">Impossibletravelriskevent オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="01f4a-104">Retrieve the properties and relationships of an impossibletravelriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="01f4a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="01f4a-105">Permissions</span></span>
<span data-ttu-id="01f4a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="01f4a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01f4a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="01f4a-108">Permission type</span></span>      | <span data-ttu-id="01f4a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="01f4a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01f4a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="01f4a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="01f4a-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="01f4a-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="01f4a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="01f4a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01f4a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="01f4a-113">Not supported.</span></span>    |
|<span data-ttu-id="01f4a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="01f4a-114">Application</span></span> | <span data-ttu-id="01f4a-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="01f4a-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01f4a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="01f4a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /impossibleTravelRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="01f4a-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="01f4a-117">Request headers</span></span>
| <span data-ttu-id="01f4a-118">名前</span><span class="sxs-lookup"><span data-stu-id="01f4a-118">Name</span></span>      |<span data-ttu-id="01f4a-119">説明</span><span class="sxs-lookup"><span data-stu-id="01f4a-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="01f4a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="01f4a-120">Authorization</span></span>  | <span data-ttu-id="01f4a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="01f4a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="01f4a-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="01f4a-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="01f4a-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="01f4a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="01f4a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="01f4a-126">Request body</span></span>
<span data-ttu-id="01f4a-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="01f4a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01f4a-128">応答</span><span class="sxs-lookup"><span data-stu-id="01f4a-128">Response</span></span>

<span data-ttu-id="01f4a-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="01f4a-129">If successful, this method returns a `200 OK` response code and [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="01f4a-130">例</span><span class="sxs-lookup"><span data-stu-id="01f4a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01f4a-131">要求</span><span class="sxs-lookup"><span data-stu-id="01f4a-131">Request</span></span>
<span data-ttu-id="01f4a-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="01f4a-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_impossibletravelriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/impossibleTravelRiskEvents/22e65c1f-909a-42b5-c0d2-075f30e27887-0bfdc7a8-6a16-c33e-7de9-a60a28ae533b-15475553-dbc1-8879-5079-23b1edd25bab
```
##### <a name="response"></a><span data-ttu-id="01f4a-133">応答</span><span class="sxs-lookup"><span data-stu-id="01f4a-133">Response</span></span>
<span data-ttu-id="01f4a-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="01f4a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get impossibleTravelRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
