---
title: リスト leakedCredentialsRiskEvents
description: leakedcredentialsriskevent オブジェクトのリストを取得します。
localization_priority: Normal
ms.openlocfilehash: 4846c9f27ded5beee29f8cfb3212551613190092
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338827"
---
# <a name="list-leakedcredentialsriskevents"></a><span data-ttu-id="29ca0-103">リスト leakedCredentialsRiskEvents</span><span class="sxs-lookup"><span data-stu-id="29ca0-103">List leakedCredentialsRiskEvents</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29ca0-104">leakedcredentialsriskevent オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="29ca0-104">Retrieve a list of leakedcredentialsriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="29ca0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="29ca0-105">Permissions</span></span>
<span data-ttu-id="29ca0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="29ca0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29ca0-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="29ca0-108">Permission type</span></span>      | <span data-ttu-id="29ca0-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="29ca0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29ca0-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="29ca0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="29ca0-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="29ca0-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="29ca0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="29ca0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29ca0-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29ca0-113">Not supported.</span></span>    |
|<span data-ttu-id="29ca0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="29ca0-114">Application</span></span> | <span data-ttu-id="29ca0-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="29ca0-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="29ca0-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="29ca0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /leakedCredentialsRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="29ca0-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="29ca0-117">Request headers</span></span>
| <span data-ttu-id="29ca0-118">名前</span><span class="sxs-lookup"><span data-stu-id="29ca0-118">Name</span></span>      |<span data-ttu-id="29ca0-119">説明</span><span class="sxs-lookup"><span data-stu-id="29ca0-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="29ca0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="29ca0-120">Authorization</span></span>  | <span data-ttu-id="29ca0-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="29ca0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="29ca0-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="29ca0-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="29ca0-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="29ca0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="29ca0-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="29ca0-126">Request body</span></span>
<span data-ttu-id="29ca0-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="29ca0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29ca0-128">応答</span><span class="sxs-lookup"><span data-stu-id="29ca0-128">Response</span></span>

<span data-ttu-id="29ca0-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="29ca0-129">If successful, this method returns a `200 OK` response code and collection of [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="29ca0-130">例</span><span class="sxs-lookup"><span data-stu-id="29ca0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="29ca0-131">要求</span><span class="sxs-lookup"><span data-stu-id="29ca0-131">Request</span></span>
<span data-ttu-id="29ca0-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="29ca0-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_leakedcredentialsriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/leakedCredentialsRiskEvents
```
##### <a name="response"></a><span data-ttu-id="29ca0-133">応答</span><span class="sxs-lookup"><span data-stu-id="29ca0-133">Response</span></span>
<span data-ttu-id="29ca0-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="29ca0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.leakedCredentialsRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
  "value":
  [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List leakedCredentialsRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
