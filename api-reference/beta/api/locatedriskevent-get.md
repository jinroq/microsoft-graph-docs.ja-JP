---
title: locatedRiskEvent を取得する
description: locatedriskevent オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
ms.openlocfilehash: aee63e3f9cbb90f839d3eaebf5ec37b2f5b53042
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540892"
---
# <a name="get-locatedriskevent"></a><span data-ttu-id="77db7-103">locatedRiskEvent を取得する</span><span class="sxs-lookup"><span data-stu-id="77db7-103">Get locatedRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77db7-104">locatedriskevent オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="77db7-104">Retrieve the properties and relationships of a locatedriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="77db7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="77db7-105">Permissions</span></span>
<span data-ttu-id="77db7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="77db7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77db7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="77db7-108">Permission type</span></span>      | <span data-ttu-id="77db7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="77db7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77db7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="77db7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="77db7-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="77db7-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="77db7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="77db7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77db7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77db7-113">Not supported.</span></span>    |
|<span data-ttu-id="77db7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="77db7-114">Application</span></span> | <span data-ttu-id="77db7-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="77db7-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="77db7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="77db7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /locatedRiskEvents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="77db7-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="77db7-117">Request headers</span></span>
| <span data-ttu-id="77db7-118">名前</span><span class="sxs-lookup"><span data-stu-id="77db7-118">Name</span></span>      |<span data-ttu-id="77db7-119">説明</span><span class="sxs-lookup"><span data-stu-id="77db7-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="77db7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="77db7-120">Authorization</span></span>  | <span data-ttu-id="77db7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="77db7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="77db7-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="77db7-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="77db7-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="77db7-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="77db7-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="77db7-126">Request body</span></span>
<span data-ttu-id="77db7-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="77db7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77db7-128">応答</span><span class="sxs-lookup"><span data-stu-id="77db7-128">Response</span></span>

<span data-ttu-id="77db7-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[locatedRiskEvent](../resources/locatedriskevent.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="77db7-129">If successful, this method returns a `200 OK` response code and [locatedRiskEvent](../resources/locatedriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="77db7-130">例</span><span class="sxs-lookup"><span data-stu-id="77db7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="77db7-131">要求</span><span class="sxs-lookup"><span data-stu-id="77db7-131">Request</span></span>
<span data-ttu-id="77db7-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="77db7-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_locatedriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/locatedRiskEvents/27b91217-a6ca-edff-da2b-c46feaf0228f-a6653179-3c7b-4e99-bb4c-dddeb18adfc1-42445d4d-fe22-9840-cf9d-72f6ce8cd056
```
##### <a name="response"></a><span data-ttu-id="77db7-133">応答</span><span class="sxs-lookup"><span data-stu-id="77db7-133">Response</span></span>
<span data-ttu-id="77db7-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="77db7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/locatedriskevent-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
