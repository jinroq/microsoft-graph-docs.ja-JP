---
title: メンバーを一覧表示する
description: グループの直接メンバーの一覧を取得します。 グループは、ユーザー、連絡先、および他のグループをメンバーとして持つことができます。
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 6c79b4bd4ee3059e693e63817420e1c5d0b8d612
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35279325"
---
# <a name="list-members"></a><span data-ttu-id="68aff-104">メンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="68aff-104">List members</span></span>
<span data-ttu-id="68aff-p102">グループの直接メンバーの一覧を取得します。グループは、ユーザー、連絡先、および他のグループをメンバーとして持つことができます。この操作は推移的ではありません。</span><span class="sxs-lookup"><span data-stu-id="68aff-p102">Get a list of the group's direct members. A group can have users, contacts, and other groups as members. This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="68aff-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="68aff-108">Permissions</span></span>
<span data-ttu-id="68aff-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="68aff-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68aff-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="68aff-111">Permission type</span></span>      | <span data-ttu-id="68aff-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="68aff-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68aff-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="68aff-113">Delegated (work or school account)</span></span> | <span data-ttu-id="68aff-114">User.ReadBasic.All、User.Read.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="68aff-114">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="68aff-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="68aff-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68aff-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68aff-116">Not supported.</span></span>    |
|<span data-ttu-id="68aff-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="68aff-117">Application</span></span> | <span data-ttu-id="68aff-118">User.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="68aff-118">User.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="68aff-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="68aff-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="68aff-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="68aff-120">Optional query parameters</span></span>
<span data-ttu-id="68aff-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="68aff-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="68aff-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="68aff-122">Request headers</span></span>
| <span data-ttu-id="68aff-123">名前</span><span class="sxs-lookup"><span data-stu-id="68aff-123">Name</span></span>       | <span data-ttu-id="68aff-124">型</span><span class="sxs-lookup"><span data-stu-id="68aff-124">Type</span></span> | <span data-ttu-id="68aff-125">説明</span><span class="sxs-lookup"><span data-stu-id="68aff-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="68aff-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="68aff-126">Authorization</span></span>  | <span data-ttu-id="68aff-127">string</span><span class="sxs-lookup"><span data-stu-id="68aff-127">string</span></span>  | <span data-ttu-id="68aff-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="68aff-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="68aff-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="68aff-130">Request body</span></span>
<span data-ttu-id="68aff-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="68aff-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68aff-132">応答</span><span class="sxs-lookup"><span data-stu-id="68aff-132">Response</span></span>
<span data-ttu-id="68aff-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="68aff-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68aff-134">例</span><span class="sxs-lookup"><span data-stu-id="68aff-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="68aff-135">要求</span><span class="sxs-lookup"><span data-stu-id="68aff-135">Request</span></span>
<span data-ttu-id="68aff-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="68aff-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```

#### <a name="response"></a><span data-ttu-id="68aff-137">応答</span><span class="sxs-lookup"><span data-stu-id="68aff-137">Response</span></span>
<span data-ttu-id="68aff-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="68aff-138">The following is an example of the response.</span></span>
><span data-ttu-id="68aff-139">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="68aff-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="68aff-140">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="68aff-140">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="68aff-141">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="68aff-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="68aff-142">C#</span><span class="sxs-lookup"><span data-stu-id="68aff-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_members-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="68aff-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="68aff-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_members-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="68aff-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="68aff-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_members-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-list-members.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-list-members.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-list-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
