---
title: directReports を一覧表示する　
description: ユーザーの直属の部下を取得します。 このユーザーがマネージャーとして割り当てられているユーザーと連絡先を返します。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 40b81284650955da317cfb90729a5e0cbcd45db1
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408956"
---
# <a name="list-directreports"></a><span data-ttu-id="b5620-104">directReports を一覧表示する　</span><span class="sxs-lookup"><span data-stu-id="b5620-104">List directReports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5620-105">ユーザーの直属の部下を取得します。</span><span class="sxs-lookup"><span data-stu-id="b5620-105">Get user's direct reports.</span></span> <span data-ttu-id="b5620-106">このユーザーがマネージャーとして割り当てられているユーザーと連絡先を返します。</span><span class="sxs-lookup"><span data-stu-id="b5620-106">Returns the users and contacts for whom this user is assigned as manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="b5620-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b5620-107">Permissions</span></span>
<span data-ttu-id="b5620-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b5620-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5620-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b5620-110">Permission type</span></span>      | <span data-ttu-id="b5620-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b5620-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5620-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b5620-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b5620-113">User.Read、User.ReadWrite、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b5620-113">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b5620-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b5620-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5620-115">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5620-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="b5620-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b5620-116">Application</span></span> | <span data-ttu-id="b5620-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5620-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5620-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b5620-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/directReports
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b5620-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b5620-119">Optional query parameters</span></span>
<span data-ttu-id="b5620-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b5620-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b5620-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b5620-121">Request headers</span></span>
| <span data-ttu-id="b5620-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b5620-122">Header</span></span>       | <span data-ttu-id="b5620-123">値</span><span class="sxs-lookup"><span data-stu-id="b5620-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="b5620-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5620-124">Authorization</span></span>  | <span data-ttu-id="b5620-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b5620-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b5620-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b5620-127">Content-Type</span></span>   | <span data-ttu-id="b5620-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b5620-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b5620-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="b5620-129">Request body</span></span>
<span data-ttu-id="b5620-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b5620-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5620-131">応答</span><span class="sxs-lookup"><span data-stu-id="b5620-131">Response</span></span>

<span data-ttu-id="b5620-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b5620-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b5620-133">例</span><span class="sxs-lookup"><span data-stu-id="b5620-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5620-134">要求</span><span class="sxs-lookup"><span data-stu-id="b5620-134">Request</span></span>
<span data-ttu-id="b5620-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b5620-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b5620-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b5620-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```http
GET https://graph.microsoft.com/beta/me/directReports
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b5620-137">C#</span><span class="sxs-lookup"><span data-stu-id="b5620-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directreports-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b5620-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5620-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directreports-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b5620-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="b5620-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directreports-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b5620-140">応答</span><span class="sxs-lookup"><span data-stu-id="b5620-140">Response</span></span>
<span data-ttu-id="b5620-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b5620-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
