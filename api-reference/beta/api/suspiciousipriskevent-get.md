---
title: suspiciousIpRiskEvent を取得する
description: Suspiciousipriskevent オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7f874b4f5bc4e20d162d56a757596789b581ed1e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991108"
---
# <a name="get-suspiciousipriskevent"></a><span data-ttu-id="ae263-103">suspiciousIpRiskEvent を取得する</span><span class="sxs-lookup"><span data-stu-id="ae263-103">Get suspiciousIpRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae263-104">Suspiciousipriskevent オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="ae263-104">Retrieve the properties and relationships of a suspiciousipriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ae263-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ae263-105">Permissions</span></span>
<span data-ttu-id="ae263-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae263-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae263-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ae263-108">Permission type</span></span>      | <span data-ttu-id="ae263-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ae263-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae263-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ae263-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ae263-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae263-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="ae263-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ae263-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae263-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae263-113">Not supported.</span></span>    |
|<span data-ttu-id="ae263-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ae263-114">Application</span></span> | <span data-ttu-id="ae263-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae263-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae263-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ae263-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /suspiciousIpRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ae263-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae263-117">Request headers</span></span>
| <span data-ttu-id="ae263-118">名前</span><span class="sxs-lookup"><span data-stu-id="ae263-118">Name</span></span>      |<span data-ttu-id="ae263-119">説明</span><span class="sxs-lookup"><span data-stu-id="ae263-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ae263-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae263-120">Authorization</span></span>  | <span data-ttu-id="ae263-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ae263-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ae263-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ae263-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="ae263-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="ae263-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae263-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ae263-126">Request body</span></span>
<span data-ttu-id="ae263-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ae263-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae263-128">応答</span><span class="sxs-lookup"><span data-stu-id="ae263-128">Response</span></span>

<span data-ttu-id="ae263-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ae263-129">If successful, this method returns a `200 OK` response code and [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ae263-130">例</span><span class="sxs-lookup"><span data-stu-id="ae263-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae263-131">要求</span><span class="sxs-lookup"><span data-stu-id="ae263-131">Request</span></span>
<span data-ttu-id="ae263-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ae263-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_suspiciousipriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/suspiciousIpRiskEvents/02e8bfd1-5231-1006-01cc-434f84e0859e-97b7301f-bc05-8e2c-fdfa-2004eb66ff70-287e7b9b-1d60-aa96-6ddb-65c81ee31475
```
##### <a name="response"></a><span data-ttu-id="ae263-133">応答</span><span class="sxs-lookup"><span data-stu-id="ae263-133">Response</span></span>
<span data-ttu-id="ae263-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ae263-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.suspiciousIpRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get suspiciousIpRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
