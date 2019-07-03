---
title: メンバーを一覧表示する
description: グループの直接メンバーの一覧を取得します。 グループは、ユーザー、連絡先、および他のグループをメンバーとして持つことができます。
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: f03e1b62d4e1e765cd552802af22361a4e88419a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35441640"
---
# <a name="list-members"></a><span data-ttu-id="4212f-104">メンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="4212f-104">List members</span></span>
<span data-ttu-id="4212f-p102">グループの直接メンバーの一覧を取得します。グループは、ユーザー、連絡先、および他のグループをメンバーとして持つことができます。この操作は推移的ではありません。</span><span class="sxs-lookup"><span data-stu-id="4212f-p102">Get a list of the group's direct members. A group can have users, contacts, and other groups as members. This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="4212f-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4212f-108">Permissions</span></span>
<span data-ttu-id="4212f-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4212f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4212f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4212f-111">Permission type</span></span>      | <span data-ttu-id="4212f-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4212f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4212f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4212f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4212f-114">User.ReadBasic.All、User.Read.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4212f-114">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="4212f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4212f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4212f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4212f-116">Not supported.</span></span>    |
|<span data-ttu-id="4212f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4212f-117">Application</span></span> | <span data-ttu-id="4212f-118">User.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="4212f-118">User.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4212f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4212f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4212f-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="4212f-120">Optional query parameters</span></span>
<span data-ttu-id="4212f-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="4212f-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4212f-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4212f-122">Request headers</span></span>
| <span data-ttu-id="4212f-123">名前</span><span class="sxs-lookup"><span data-stu-id="4212f-123">Name</span></span>       | <span data-ttu-id="4212f-124">型</span><span class="sxs-lookup"><span data-stu-id="4212f-124">Type</span></span> | <span data-ttu-id="4212f-125">説明</span><span class="sxs-lookup"><span data-stu-id="4212f-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4212f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="4212f-126">Authorization</span></span>  | <span data-ttu-id="4212f-127">string</span><span class="sxs-lookup"><span data-stu-id="4212f-127">string</span></span>  | <span data-ttu-id="4212f-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4212f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4212f-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="4212f-130">Request body</span></span>
<span data-ttu-id="4212f-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4212f-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4212f-132">応答</span><span class="sxs-lookup"><span data-stu-id="4212f-132">Response</span></span>
<span data-ttu-id="4212f-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="4212f-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4212f-134">例</span><span class="sxs-lookup"><span data-stu-id="4212f-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4212f-135">要求</span><span class="sxs-lookup"><span data-stu-id="4212f-135">Request</span></span>
<span data-ttu-id="4212f-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4212f-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4212f-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="4212f-137">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4212f-138">C#</span><span class="sxs-lookup"><span data-stu-id="4212f-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4212f-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="4212f-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4212f-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4212f-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4212f-141">応答</span><span class="sxs-lookup"><span data-stu-id="4212f-141">Response</span></span>
<span data-ttu-id="4212f-142">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4212f-142">The following is an example of the response.</span></span>
><span data-ttu-id="4212f-143">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="4212f-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4212f-144">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4212f-144">All the properties will be returned from an actual call.</span></span>
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
