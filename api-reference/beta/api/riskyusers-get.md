---
title: RiskyUser を取得する
description: '**RiskyUser**オブジェクトのプロパティとリレーションシップを取得します。'
localization_priority: Normal
author: cloudhandler
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 61e11b933cd2a7f284920d144da7e022486bdb1e
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410816"
---
# <a name="get-riskyuser"></a><span data-ttu-id="0bafe-103">RiskyUser を取得する</span><span class="sxs-lookup"><span data-stu-id="0bafe-103">Get riskyUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0bafe-104">**RiskyUser**オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="0bafe-104">Retrieve the properties and relationships of a **riskyUser** object.</span></span>

><span data-ttu-id="0bafe-105">**注:** RiskyUsers API を使用するには、Azure AD Premium P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="0bafe-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="0bafe-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0bafe-106">Permissions</span></span>
<span data-ttu-id="0bafe-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0bafe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bafe-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0bafe-109">Permission type</span></span>      | <span data-ttu-id="0bafe-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0bafe-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0bafe-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0bafe-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0bafe-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="0bafe-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="0bafe-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0bafe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0bafe-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0bafe-114">Not supported.</span></span>    |
|<span data-ttu-id="0bafe-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0bafe-115">Application</span></span> | <span data-ttu-id="0bafe-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="0bafe-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0bafe-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0bafe-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{id}
```


## <a name="request-headers"></a><span data-ttu-id="0bafe-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0bafe-118">Request headers</span></span>
| <span data-ttu-id="0bafe-119">名前</span><span class="sxs-lookup"><span data-stu-id="0bafe-119">Name</span></span>      |<span data-ttu-id="0bafe-120">説明</span><span class="sxs-lookup"><span data-stu-id="0bafe-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0bafe-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0bafe-121">Authorization</span></span>  | <span data-ttu-id="0bafe-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0bafe-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0bafe-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0bafe-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="0bafe-125">変更を保存するかどうかを決定するブックセッション ID。</span><span class="sxs-lookup"><span data-stu-id="0bafe-125">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="0bafe-126">省略可能。</span><span class="sxs-lookup"><span data-stu-id="0bafe-126">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bafe-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0bafe-127">Request body</span></span>
<span data-ttu-id="0bafe-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0bafe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0bafe-129">応答</span><span class="sxs-lookup"><span data-stu-id="0bafe-129">Response</span></span>

<span data-ttu-id="0bafe-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[riskyUser](../resources/riskyuser.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0bafe-130">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0bafe-131">例</span><span class="sxs-lookup"><span data-stu-id="0bafe-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0bafe-132">要求</span><span class="sxs-lookup"><span data-stu-id="0bafe-132">Request</span></span>
<span data-ttu-id="0bafe-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0bafe-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0bafe-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="0bafe-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0bafe-135">C#</span><span class="sxs-lookup"><span data-stu-id="0bafe-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0bafe-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0bafe-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0bafe-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="0bafe-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0bafe-138">応答</span><span class="sxs-lookup"><span data-stu-id="0bafe-138">Response</span></span>
<span data-ttu-id="0bafe-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="0bafe-139">Here is an example of the response.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

