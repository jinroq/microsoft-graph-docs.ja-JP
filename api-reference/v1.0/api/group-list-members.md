---
title: メンバーを一覧表示する
description: グループの直接メンバーの一覧を取得します。 グループは、ユーザー、連絡先、および他のグループをメンバーとして持つことができます。
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: f70ca44404e0a5fb72f6e347e8a6ffa6fa2d1727
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889120"
---
# <a name="list-members"></a><span data-ttu-id="f2ea0-104">メンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f2ea0-104">List members</span></span>
<span data-ttu-id="f2ea0-p102">グループの直接メンバーの一覧を取得します。グループは、ユーザー、連絡先、および他のグループをメンバーとして持つことができます。この操作は推移的ではありません。</span><span class="sxs-lookup"><span data-stu-id="f2ea0-p102">Get a list of the group's direct members. A group can have users, contacts, and other groups as members. This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2ea0-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f2ea0-108">Permissions</span></span>
<span data-ttu-id="f2ea0-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f2ea0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2ea0-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f2ea0-111">Permission type</span></span>      | <span data-ttu-id="f2ea0-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f2ea0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2ea0-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f2ea0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f2ea0-114">User.ReadBasic.All、User.Read.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f2ea0-114">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="f2ea0-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f2ea0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2ea0-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2ea0-116">Not supported.</span></span>    |
|<span data-ttu-id="f2ea0-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f2ea0-117">Application</span></span> | <span data-ttu-id="f2ea0-118">User.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2ea0-118">User.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2ea0-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f2ea0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2ea0-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f2ea0-120">Optional query parameters</span></span>
<span data-ttu-id="f2ea0-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f2ea0-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2ea0-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f2ea0-122">Request headers</span></span>
| <span data-ttu-id="f2ea0-123">名前</span><span class="sxs-lookup"><span data-stu-id="f2ea0-123">Name</span></span>       | <span data-ttu-id="f2ea0-124">型</span><span class="sxs-lookup"><span data-stu-id="f2ea0-124">Type</span></span> | <span data-ttu-id="f2ea0-125">説明</span><span class="sxs-lookup"><span data-stu-id="f2ea0-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f2ea0-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2ea0-126">Authorization</span></span>  | <span data-ttu-id="f2ea0-127">string</span><span class="sxs-lookup"><span data-stu-id="f2ea0-127">string</span></span>  | <span data-ttu-id="f2ea0-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f2ea0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2ea0-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="f2ea0-130">Request body</span></span>
<span data-ttu-id="f2ea0-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f2ea0-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2ea0-132">応答</span><span class="sxs-lookup"><span data-stu-id="f2ea0-132">Response</span></span>
<span data-ttu-id="f2ea0-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f2ea0-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2ea0-134">例</span><span class="sxs-lookup"><span data-stu-id="f2ea0-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f2ea0-135">要求</span><span class="sxs-lookup"><span data-stu-id="f2ea0-135">Request</span></span>
<span data-ttu-id="f2ea0-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f2ea0-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f2ea0-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2ea0-137">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f2ea0-138">C#</span><span class="sxs-lookup"><span data-stu-id="f2ea0-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f2ea0-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="f2ea0-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f2ea0-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2ea0-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f2ea0-141">Java</span><span class="sxs-lookup"><span data-stu-id="f2ea0-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f2ea0-142">応答</span><span class="sxs-lookup"><span data-stu-id="f2ea0-142">Response</span></span>
<span data-ttu-id="f2ea0-143">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f2ea0-143">The following is an example of the response.</span></span>
><span data-ttu-id="f2ea0-144">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="f2ea0-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f2ea0-145">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f2ea0-145">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
