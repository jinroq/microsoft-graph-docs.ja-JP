---
title: リスト anonymousIpRiskEvents
description: Anonymousipriskevent オブジェクトのリストを取得します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7935b5bcb98d5f7122f3967aeed1313315259a29
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945572"
---
# <a name="list-anonymousipriskevents"></a><span data-ttu-id="143b3-103">リスト anonymousIpRiskEvents</span><span class="sxs-lookup"><span data-stu-id="143b3-103">List anonymousIpRiskEvents</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="143b3-104">Anonymousipriskevent オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="143b3-104">Retrieve a list of anonymousipriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="143b3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="143b3-105">Permissions</span></span>
<span data-ttu-id="143b3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="143b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="143b3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="143b3-108">Permission type</span></span>      | <span data-ttu-id="143b3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="143b3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="143b3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="143b3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="143b3-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="143b3-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="143b3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="143b3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="143b3-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="143b3-113">Not supported.</span></span>    |
|<span data-ttu-id="143b3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="143b3-114">Application</span></span> | <span data-ttu-id="143b3-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="143b3-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="143b3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="143b3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /anonymousIpRiskEvents
```

## <a name="request-headers"></a><span data-ttu-id="143b3-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="143b3-117">Request headers</span></span>
| <span data-ttu-id="143b3-118">名前</span><span class="sxs-lookup"><span data-stu-id="143b3-118">Name</span></span>      |<span data-ttu-id="143b3-119">説明</span><span class="sxs-lookup"><span data-stu-id="143b3-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="143b3-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="143b3-120">Authorization</span></span>  | <span data-ttu-id="143b3-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="143b3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="143b3-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="143b3-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="143b3-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="143b3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="143b3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="143b3-126">Request body</span></span>
<span data-ttu-id="143b3-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="143b3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="143b3-128">応答</span><span class="sxs-lookup"><span data-stu-id="143b3-128">Response</span></span>

<span data-ttu-id="143b3-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[anonymousIpRiskEvent](../resources/anonymousipriskevent.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="143b3-129">If successful, this method returns a `200 OK` response code and collection of [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="143b3-130">例</span><span class="sxs-lookup"><span data-stu-id="143b3-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="143b3-131">要求</span><span class="sxs-lookup"><span data-stu-id="143b3-131">Request</span></span>
<span data-ttu-id="143b3-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="143b3-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_anonymousipriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/anonymousIpRiskEvents
```
##### <a name="response"></a><span data-ttu-id="143b3-133">応答</span><span class="sxs-lookup"><span data-stu-id="143b3-133">Response</span></span>
<span data-ttu-id="143b3-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="143b3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List anonymousIpRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
