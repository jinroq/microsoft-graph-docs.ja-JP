---
title: IdentityRiskEvent を取得します。
description: プロパティと identityriskevent オブジェクトの関係を取得します。
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: e86ec77450a1b661311ba9e53b3b3591776323a4
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575703"
---
# <a name="get-identityriskevent"></a><span data-ttu-id="d8821-103">IdentityRiskEvent を取得します。</span><span class="sxs-lookup"><span data-stu-id="d8821-103">Get identityRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8821-104">プロパティと identityriskevent オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="d8821-104">Retrieve the properties and relationships of identityriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d8821-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d8821-105">Permissions</span></span>
<span data-ttu-id="d8821-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d8821-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8821-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d8821-108">Permission type</span></span>      | <span data-ttu-id="d8821-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d8821-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8821-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d8821-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d8821-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8821-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="d8821-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d8821-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8821-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8821-113">Not supported.</span></span>    |
|<span data-ttu-id="d8821-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d8821-114">Application</span></span> | <span data-ttu-id="d8821-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8821-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8821-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d8821-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d8821-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d8821-117">Request headers</span></span>
| <span data-ttu-id="d8821-118">名前</span><span class="sxs-lookup"><span data-stu-id="d8821-118">Name</span></span>      |<span data-ttu-id="d8821-119">説明</span><span class="sxs-lookup"><span data-stu-id="d8821-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d8821-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8821-120">Authorization</span></span>  | <span data-ttu-id="d8821-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d8821-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d8821-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d8821-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d8821-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="d8821-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8821-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d8821-126">Request body</span></span>
<span data-ttu-id="d8821-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d8821-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8821-128">応答</span><span class="sxs-lookup"><span data-stu-id="d8821-128">Response</span></span>

<span data-ttu-id="d8821-129">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[identityRiskEvent](../resources/identityriskevent.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="d8821-129">If successful, this method returns a `200 OK` response code and [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d8821-130">例</span><span class="sxs-lookup"><span data-stu-id="d8821-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d8821-131">要求</span><span class="sxs-lookup"><span data-stu-id="d8821-131">Request</span></span>
<span data-ttu-id="d8821-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d8821-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/identityRiskEvents/ec50e9fb-9da1-215b-e18c-b7e2a716b2a6
```
##### <a name="response"></a><span data-ttu-id="d8821-133">応答</span><span class="sxs-lookup"><span data-stu-id="d8821-133">Response</span></span>
<span data-ttu-id="d8821-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d8821-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": "ec50e9fb-9da1-215b-e18c-b7e2a716b2a6",
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
<!--
{
  "type": "#page.annotation",
  "description": "Get identityRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/identityriskevent-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
