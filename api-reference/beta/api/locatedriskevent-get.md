---
title: LocatedRiskEvent を取得する
description: Locatedriskevent オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: a90ecf29119a74e3d102e61ca1f2987683d5c54d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35984095"
---
# <a name="get-locatedriskevent"></a><span data-ttu-id="bf556-103">LocatedRiskEvent を取得する</span><span class="sxs-lookup"><span data-stu-id="bf556-103">Get locatedRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf556-104">Locatedriskevent オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="bf556-104">Retrieve the properties and relationships of a locatedriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bf556-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bf556-105">Permissions</span></span>
<span data-ttu-id="bf556-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bf556-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf556-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bf556-108">Permission type</span></span>      | <span data-ttu-id="bf556-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bf556-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf556-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bf556-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bf556-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf556-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="bf556-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bf556-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf556-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bf556-113">Not supported.</span></span>    |
|<span data-ttu-id="bf556-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bf556-114">Application</span></span> | <span data-ttu-id="bf556-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf556-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf556-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bf556-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /locatedRiskEvents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bf556-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bf556-117">Request headers</span></span>
| <span data-ttu-id="bf556-118">名前</span><span class="sxs-lookup"><span data-stu-id="bf556-118">Name</span></span>      |<span data-ttu-id="bf556-119">説明</span><span class="sxs-lookup"><span data-stu-id="bf556-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bf556-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf556-120">Authorization</span></span>  | <span data-ttu-id="bf556-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bf556-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bf556-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bf556-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="bf556-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="bf556-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf556-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="bf556-126">Request body</span></span>
<span data-ttu-id="bf556-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bf556-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf556-128">応答</span><span class="sxs-lookup"><span data-stu-id="bf556-128">Response</span></span>

<span data-ttu-id="bf556-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[locatedRiskEvent](../resources/locatedriskevent.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bf556-129">If successful, this method returns a `200 OK` response code and [locatedRiskEvent](../resources/locatedriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bf556-130">例</span><span class="sxs-lookup"><span data-stu-id="bf556-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bf556-131">要求</span><span class="sxs-lookup"><span data-stu-id="bf556-131">Request</span></span>
<span data-ttu-id="bf556-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bf556-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_locatedriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/locatedRiskEvents/27b91217-a6ca-edff-da2b-c46feaf0228f-a6653179-3c7b-4e99-bb4c-dddeb18adfc1-42445d4d-fe22-9840-cf9d-72f6ce8cd056
```
##### <a name="response"></a><span data-ttu-id="bf556-133">応答</span><span class="sxs-lookup"><span data-stu-id="bf556-133">Response</span></span>
<span data-ttu-id="bf556-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bf556-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get locatedRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
