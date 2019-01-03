---
title: リスト leakedCredentialsRiskEvents
description: Leakedcredentialsriskevent オブジェクトのリストを取得します。
ms.openlocfilehash: 49cfd54c580634e43cff50aa7c125ffc79116ea3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071653"
---
# <a name="list-leakedcredentialsriskevents"></a><span data-ttu-id="5f116-103">リスト leakedCredentialsRiskEvents</span><span class="sxs-lookup"><span data-stu-id="5f116-103">List leakedCredentialsRiskEvents</span></span>

> <span data-ttu-id="5f116-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5f116-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f116-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f116-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5f116-106">Leakedcredentialsriskevent オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="5f116-106">Retrieve a list of leakedcredentialsriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="5f116-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5f116-107">Permissions</span></span>
<span data-ttu-id="5f116-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5f116-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f116-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5f116-110">Permission type</span></span>      | <span data-ttu-id="5f116-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5f116-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f116-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5f116-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5f116-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f116-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="5f116-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5f116-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f116-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f116-115">Not supported.</span></span>    |
|<span data-ttu-id="5f116-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5f116-116">Application</span></span> | <span data-ttu-id="5f116-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f116-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f116-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5f116-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /leakedCredentialsRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="5f116-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5f116-119">Request headers</span></span>
| <span data-ttu-id="5f116-120">名前</span><span class="sxs-lookup"><span data-stu-id="5f116-120">Name</span></span>      |<span data-ttu-id="5f116-121">説明</span><span class="sxs-lookup"><span data-stu-id="5f116-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5f116-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f116-122">Authorization</span></span>  | <span data-ttu-id="5f116-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5f116-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5f116-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5f116-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="5f116-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="5f116-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f116-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="5f116-128">Request body</span></span>
<span data-ttu-id="5f116-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5f116-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f116-130">応答</span><span class="sxs-lookup"><span data-stu-id="5f116-130">Response</span></span>

<span data-ttu-id="5f116-131">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="5f116-131">If successful, this method returns a `200 OK` response code and collection of [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5f116-132">例</span><span class="sxs-lookup"><span data-stu-id="5f116-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5f116-133">要求</span><span class="sxs-lookup"><span data-stu-id="5f116-133">Request</span></span>
<span data-ttu-id="5f116-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5f116-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_leakedcredentialsriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/leakedCredentialsRiskEvents
```
##### <a name="response"></a><span data-ttu-id="5f116-135">応答</span><span class="sxs-lookup"><span data-stu-id="5f116-135">Response</span></span>
<span data-ttu-id="5f116-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5f116-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List leakedCredentialsRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->