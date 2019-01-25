---
title: UnfamiliarLocationRiskEvent を取得します。
description: プロパティと unfamiliarlocationriskevent オブジェクトの関係を取得します。
localization_priority: Normal
ms.openlocfilehash: 99a7578cf9ebe183483c9d09a83696a4bc2ffbef
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515483"
---
# <a name="get-unfamiliarlocationriskevent"></a><span data-ttu-id="c4fb5-103">UnfamiliarLocationRiskEvent を取得します。</span><span class="sxs-lookup"><span data-stu-id="c4fb5-103">Get unfamiliarLocationRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4fb5-104">プロパティと unfamiliarlocationriskevent オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="c4fb5-104">Retrieve the properties and relationships of an unfamiliarlocationriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c4fb5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c4fb5-105">Permissions</span></span>
<span data-ttu-id="c4fb5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c4fb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4fb5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c4fb5-108">Permission type</span></span>      | <span data-ttu-id="c4fb5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c4fb5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4fb5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c4fb5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c4fb5-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4fb5-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="c4fb5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c4fb5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4fb5-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4fb5-113">Not supported.</span></span>    |
|<span data-ttu-id="c4fb5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c4fb5-114">Application</span></span> | <span data-ttu-id="c4fb5-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4fb5-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4fb5-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c4fb5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /unfamiliarLocationRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c4fb5-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c4fb5-117">Request headers</span></span>
| <span data-ttu-id="c4fb5-118">名前</span><span class="sxs-lookup"><span data-stu-id="c4fb5-118">Name</span></span>      |<span data-ttu-id="c4fb5-119">説明</span><span class="sxs-lookup"><span data-stu-id="c4fb5-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c4fb5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4fb5-120">Authorization</span></span>  | <span data-ttu-id="c4fb5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c4fb5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c4fb5-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c4fb5-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c4fb5-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="c4fb5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4fb5-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c4fb5-126">Request body</span></span>
<span data-ttu-id="c4fb5-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c4fb5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4fb5-128">応答</span><span class="sxs-lookup"><span data-stu-id="c4fb5-128">Response</span></span>

<span data-ttu-id="c4fb5-129">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c4fb5-129">If successful, this method returns a `200 OK` response code and [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c4fb5-130">例</span><span class="sxs-lookup"><span data-stu-id="c4fb5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c4fb5-131">要求</span><span class="sxs-lookup"><span data-stu-id="c4fb5-131">Request</span></span>
<span data-ttu-id="c4fb5-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c4fb5-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unfamiliarlocationriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/unfamiliarLocationRiskEvents/700b6476-8138-4c14-4962-c43614958301-8dce9c6b-21f1-2e3b-2c3b-5164f751e7ad-4e5591fd-2ac1-4e9d-96a9-aca8339e2604
```
##### <a name="response"></a><span data-ttu-id="c4fb5-133">応答</span><span class="sxs-lookup"><span data-stu-id="c4fb5-133">Response</span></span>
<span data-ttu-id="c4fb5-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c4fb5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unfamiliarLocationRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "closedDateTime": "2016-01-29T20:03:57.7872426Z",
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "700b6476-8138-4c14-4962-c43614958301-8dce9c6b-21f1-2e3b-2c3b-5164f751e7ad-4e5591fd-2ac1-4e9d-96a9-aca8339e2604",
  "ipAddress": "176.10.104.240",
  "location": "Bern, CH",
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "remediated",
  "riskLevel": "medium",
  "riskType": "UnfamiliarLocationRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "8dce9c6b-21f1-2e3b-2c3b-5164f751e7ad",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get unfamiliarLocationRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/unfamiliarlocationriskevent-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
