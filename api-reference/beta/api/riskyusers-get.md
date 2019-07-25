---
title: RiskyUser を取得する
description: '**RiskyUser**オブジェクトのプロパティとリレーションシップを取得します。'
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 12932e22e88271a11f35f5e28dc52cfca78e407c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871013"
---
# <a name="get-riskyuser"></a><span data-ttu-id="1bc09-103">RiskyUser を取得する</span><span class="sxs-lookup"><span data-stu-id="1bc09-103">Get riskyUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bc09-104">**RiskyUser**オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="1bc09-104">Retrieve the properties and relationships of a **riskyUser** object.</span></span>

><span data-ttu-id="1bc09-105">**注:** RiskyUsers API を使用するには、Azure AD Premium P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="1bc09-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="1bc09-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1bc09-106">Permissions</span></span>
<span data-ttu-id="1bc09-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1bc09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bc09-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1bc09-109">Permission type</span></span>      | <span data-ttu-id="1bc09-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1bc09-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1bc09-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1bc09-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1bc09-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="1bc09-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="1bc09-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1bc09-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bc09-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1bc09-114">Not supported.</span></span>    |
|<span data-ttu-id="1bc09-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1bc09-115">Application</span></span> | <span data-ttu-id="1bc09-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="1bc09-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1bc09-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1bc09-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{id}
```


## <a name="request-headers"></a><span data-ttu-id="1bc09-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1bc09-118">Request headers</span></span>
| <span data-ttu-id="1bc09-119">名前</span><span class="sxs-lookup"><span data-stu-id="1bc09-119">Name</span></span>      |<span data-ttu-id="1bc09-120">説明</span><span class="sxs-lookup"><span data-stu-id="1bc09-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1bc09-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bc09-121">Authorization</span></span>  | <span data-ttu-id="1bc09-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1bc09-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1bc09-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1bc09-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="1bc09-125">変更を保存するかどうかを決定するブックセッション ID。</span><span class="sxs-lookup"><span data-stu-id="1bc09-125">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="1bc09-126">省略可能。</span><span class="sxs-lookup"><span data-stu-id="1bc09-126">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bc09-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1bc09-127">Request body</span></span>
<span data-ttu-id="1bc09-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1bc09-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bc09-129">応答</span><span class="sxs-lookup"><span data-stu-id="1bc09-129">Response</span></span>

<span data-ttu-id="1bc09-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[riskyUser](../resources/riskyuser.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1bc09-130">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1bc09-131">例</span><span class="sxs-lookup"><span data-stu-id="1bc09-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1bc09-132">要求</span><span class="sxs-lookup"><span data-stu-id="1bc09-132">Request</span></span>
<span data-ttu-id="1bc09-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1bc09-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1bc09-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1bc09-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1bc09-135">C#</span><span class="sxs-lookup"><span data-stu-id="1bc09-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1bc09-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="1bc09-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1bc09-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="1bc09-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1bc09-138">Java</span><span class="sxs-lookup"><span data-stu-id="1bc09-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-riskyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1bc09-139">応答</span><span class="sxs-lookup"><span data-stu-id="1bc09-139">Response</span></span>
<span data-ttu-id="1bc09-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="1bc09-140">Here is an example of the response.</span></span>
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

