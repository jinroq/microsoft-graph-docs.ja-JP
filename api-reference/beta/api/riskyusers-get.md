---
title: RiskyUser を取得する
description: '**RiskyUser**オブジェクトのプロパティとリレーションシップを取得します。'
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b268804444ad4693d06728568c5a2439883a8f95
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536463"
---
# <a name="get-riskyuser"></a><span data-ttu-id="a05ed-103">RiskyUser を取得する</span><span class="sxs-lookup"><span data-stu-id="a05ed-103">Get riskyUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a05ed-104">**RiskyUser**オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="a05ed-104">Retrieve the properties and relationships of a **riskyUser** object.</span></span>

><span data-ttu-id="a05ed-105">**注:** RiskyUsers API を使用するには、Azure AD Premium P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="a05ed-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="a05ed-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a05ed-106">Permissions</span></span>
<span data-ttu-id="a05ed-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a05ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a05ed-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a05ed-109">Permission type</span></span>      | <span data-ttu-id="a05ed-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a05ed-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a05ed-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a05ed-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a05ed-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="a05ed-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="a05ed-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a05ed-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a05ed-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a05ed-114">Not supported.</span></span>    |
|<span data-ttu-id="a05ed-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a05ed-115">Application</span></span> | <span data-ttu-id="a05ed-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="a05ed-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a05ed-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a05ed-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{id}
```


## <a name="request-headers"></a><span data-ttu-id="a05ed-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a05ed-118">Request headers</span></span>
| <span data-ttu-id="a05ed-119">名前</span><span class="sxs-lookup"><span data-stu-id="a05ed-119">Name</span></span>      |<span data-ttu-id="a05ed-120">説明</span><span class="sxs-lookup"><span data-stu-id="a05ed-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a05ed-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a05ed-121">Authorization</span></span>  | <span data-ttu-id="a05ed-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a05ed-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a05ed-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a05ed-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="a05ed-125">変更を保存するかどうかを決定するブックセッション ID。</span><span class="sxs-lookup"><span data-stu-id="a05ed-125">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="a05ed-126">省略可能。</span><span class="sxs-lookup"><span data-stu-id="a05ed-126">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a05ed-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a05ed-127">Request body</span></span>
<span data-ttu-id="a05ed-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a05ed-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a05ed-129">応答</span><span class="sxs-lookup"><span data-stu-id="a05ed-129">Response</span></span>

<span data-ttu-id="a05ed-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[riskyUser](../resources/riskyuser.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a05ed-130">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a05ed-131">例</span><span class="sxs-lookup"><span data-stu-id="a05ed-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a05ed-132">要求</span><span class="sxs-lookup"><span data-stu-id="a05ed-132">Request</span></span>
<span data-ttu-id="a05ed-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a05ed-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuser",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
##### <a name="response"></a><span data-ttu-id="a05ed-134">応答</span><span class="sxs-lookup"><span data-stu-id="a05ed-134">Response</span></span>
<span data-ttu-id="a05ed-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="a05ed-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
  "riskLastUpdatedDateTime": "2016-01-29T20:03:57.7872426Z",
  "isGuest": true,
  "isProcessing": true,
  "isDeleted": true,
  "riskDetail": "adminConfirmedSigninCompromised",
  "riskLevel": "high",
  "riskState": "atRisk",
  "userDisplayName": "Alex Wilbur",
  "userPrincipalName": "alexw@contoso.com"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a05ed-136">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="a05ed-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a05ed-137">C#</span><span class="sxs-lookup"><span data-stu-id="a05ed-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_riskyuser-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a05ed-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="a05ed-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_riskyuser-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/riskyusers-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/riskyusers-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

