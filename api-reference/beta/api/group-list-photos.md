---
title: 写真の一覧表示
description: profilePhoto オブジェクトのリストを取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d90e92b58dc85629d86c8527e835c4a5520256a6
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420702"
---
# <a name="list-photos"></a><span data-ttu-id="ce535-103">写真の一覧表示</span><span class="sxs-lookup"><span data-stu-id="ce535-103">List photos</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce535-104">[profilePhoto](../resources/profilephoto.md) オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="ce535-104">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce535-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ce535-105">Permissions</span></span>
<span data-ttu-id="ce535-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce535-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce535-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ce535-108">Permission type</span></span>      | <span data-ttu-id="ce535-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ce535-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce535-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ce535-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ce535-111">Group.ReadBasic.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce535-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ce535-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ce535-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce535-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce535-113">Not supported.</span></span>    |
|<span data-ttu-id="ce535-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ce535-114">Application</span></span> | <span data-ttu-id="ce535-115">Group.ReadBasic.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce535-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce535-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ce535-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ce535-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ce535-117">Optional query parameters</span></span>
<span data-ttu-id="ce535-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ce535-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce535-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce535-119">Request headers</span></span>
| <span data-ttu-id="ce535-120">名前</span><span class="sxs-lookup"><span data-stu-id="ce535-120">Name</span></span>       | <span data-ttu-id="ce535-121">型</span><span class="sxs-lookup"><span data-stu-id="ce535-121">Type</span></span> | <span data-ttu-id="ce535-122">説明</span><span class="sxs-lookup"><span data-stu-id="ce535-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ce535-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce535-123">Authorization</span></span>  | <span data-ttu-id="ce535-124">string</span><span class="sxs-lookup"><span data-stu-id="ce535-124">string</span></span>  | <span data-ttu-id="ce535-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ce535-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce535-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ce535-127">Request body</span></span>
<span data-ttu-id="ce535-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ce535-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce535-129">応答</span><span class="sxs-lookup"><span data-stu-id="ce535-129">Response</span></span>
<span data-ttu-id="ce535-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [profilePhoto](../resources/profilephoto.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ce535-130">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce535-131">例</span><span class="sxs-lookup"><span data-stu-id="ce535-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ce535-132">要求</span><span class="sxs-lookup"><span data-stu-id="ce535-132">Request</span></span>
<span data-ttu-id="ce535-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ce535-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ce535-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ce535-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/photos
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ce535-135">C#</span><span class="sxs-lookup"><span data-stu-id="ce535-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-photos-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ce535-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce535-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-photos-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ce535-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="ce535-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-photos-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ce535-138">応答</span><span class="sxs-lookup"><span data-stu-id="ce535-138">Response</span></span>
<span data-ttu-id="ce535-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ce535-139">The following is an example of the response.</span></span>
><span data-ttu-id="ce535-140">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="ce535-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ce535-141">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ce535-141">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profilePhoto",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 94

{
  "value": [
    {
      "height": 99,
      "width": 99,
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
  "description": "List photos",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
