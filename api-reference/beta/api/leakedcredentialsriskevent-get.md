---
title: LeakedCredentialsRiskEvent を取得します。
description: プロパティと、leakedcredentialsriskevent オブジェクトの関係を取得します。
localization_priority: Normal
ms.openlocfilehash: eb7b7ca5ecac02a91c2e9733511cd0a384782bd3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509834"
---
# <a name="get-leakedcredentialsriskevent"></a><span data-ttu-id="73d19-103">LeakedCredentialsRiskEvent を取得します。</span><span class="sxs-lookup"><span data-stu-id="73d19-103">Get leakedCredentialsRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73d19-104">プロパティと、leakedcredentialsriskevent オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="73d19-104">Retrieve the properties and relationships of a leakedcredentialsriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="73d19-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="73d19-105">Permissions</span></span>
<span data-ttu-id="73d19-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="73d19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73d19-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="73d19-108">Permission type</span></span>      | <span data-ttu-id="73d19-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="73d19-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73d19-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="73d19-110">Delegated (work or school account)</span></span> | <span data-ttu-id="73d19-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="73d19-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="73d19-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="73d19-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73d19-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73d19-113">Not supported.</span></span>    |
|<span data-ttu-id="73d19-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="73d19-114">Application</span></span> | <span data-ttu-id="73d19-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="73d19-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="73d19-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="73d19-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /leakedCredentialsRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="73d19-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="73d19-117">Request headers</span></span>
| <span data-ttu-id="73d19-118">名前</span><span class="sxs-lookup"><span data-stu-id="73d19-118">Name</span></span>      |<span data-ttu-id="73d19-119">説明</span><span class="sxs-lookup"><span data-stu-id="73d19-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="73d19-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="73d19-120">Authorization</span></span>  | <span data-ttu-id="73d19-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="73d19-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="73d19-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="73d19-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="73d19-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="73d19-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="73d19-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="73d19-126">Request body</span></span>
<span data-ttu-id="73d19-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="73d19-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73d19-128">応答</span><span class="sxs-lookup"><span data-stu-id="73d19-128">Response</span></span>

<span data-ttu-id="73d19-129">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="73d19-129">If successful, this method returns a `200 OK` response code and [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="73d19-130">例</span><span class="sxs-lookup"><span data-stu-id="73d19-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73d19-131">要求</span><span class="sxs-lookup"><span data-stu-id="73d19-131">Request</span></span>
<span data-ttu-id="73d19-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="73d19-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_leakedcredentialsriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/leakedCredentialsRiskEvents/8c793a18-c86a-b5f9-7d9a-b3d024f33eee-278dc452-4163-dbc6-84eb-a050c37fc931-1a01abd3-b87a-cece-3f4d-c788b055c182
```
##### <a name="response"></a><span data-ttu-id="73d19-133">応答</span><span class="sxs-lookup"><span data-stu-id="73d19-133">Response</span></span>
<span data-ttu-id="73d19-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="73d19-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.leakedCredentialsRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "closedDateTime": null,
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "8c793a18-c86a-b5f9-7d9a-b3d024f33eee-278dc452-4163-dbc6-84eb-a050c37fc931-1a01abd3-b87a-cece-3f4d-c788b055c182",
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "active",
  "riskLevel": "high",
  "riskType": "LeakedCredentialsRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "278dc452-4163-dbc6-84eb-a050c37fc931",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get leakedCredentialsRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/leakedcredentialsriskevent-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
