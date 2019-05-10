---
title: 所有者を一覧表示する
description: 'グループの所有者の一覧を取得します。所有者は、グループ オブジェクトの変更を許可されている管理者以外のユーザーです。 '
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: ad2c5abbbfe7178386612ebb3980be36db690823
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33614122"
---
# <a name="list-owners"></a><span data-ttu-id="cac83-104">所有者を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="cac83-104">List owners</span></span>
<span data-ttu-id="cac83-p102">グループの所有者の一覧を取得します。所有者は、グループ オブジェクトの変更を許可されている管理者以外のユーザーです。</span><span class="sxs-lookup"><span data-stu-id="cac83-p102">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="cac83-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cac83-107">Permissions</span></span>
<span data-ttu-id="cac83-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cac83-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cac83-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cac83-110">Permission type</span></span>      | <span data-ttu-id="cac83-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cac83-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cac83-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cac83-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cac83-113">Group.Read.All と User.ReadBasic.All、Group.Read.All と User.Read.All、Group.Read.All と User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cac83-113">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span>   |
|<span data-ttu-id="cac83-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cac83-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cac83-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cac83-115">Not supported.</span></span>    |
|<span data-ttu-id="cac83-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cac83-116">Application</span></span> | <span data-ttu-id="cac83-117">Group.Read.All と User.Read.All、Group.Read.All と User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cac83-117">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cac83-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cac83-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cac83-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="cac83-119">Optional query parameters</span></span>
<span data-ttu-id="cac83-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="cac83-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cac83-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cac83-121">Request headers</span></span>
| <span data-ttu-id="cac83-122">名前</span><span class="sxs-lookup"><span data-stu-id="cac83-122">Name</span></span>       | <span data-ttu-id="cac83-123">型</span><span class="sxs-lookup"><span data-stu-id="cac83-123">Type</span></span> | <span data-ttu-id="cac83-124">説明</span><span class="sxs-lookup"><span data-stu-id="cac83-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cac83-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="cac83-125">Authorization</span></span>  | <span data-ttu-id="cac83-126">string</span><span class="sxs-lookup"><span data-stu-id="cac83-126">string</span></span>  | <span data-ttu-id="cac83-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cac83-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cac83-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="cac83-129">Request body</span></span>
<span data-ttu-id="cac83-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cac83-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cac83-131">応答</span><span class="sxs-lookup"><span data-stu-id="cac83-131">Response</span></span>
<span data-ttu-id="cac83-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [user](../resources/user.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="cac83-132">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cac83-133">例</span><span class="sxs-lookup"><span data-stu-id="cac83-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cac83-134">要求</span><span class="sxs-lookup"><span data-stu-id="cac83-134">Request</span></span>
<span data-ttu-id="cac83-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cac83-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/owners
```

#### <a name="response"></a><span data-ttu-id="cac83-136">応答</span><span class="sxs-lookup"><span data-stu-id="cac83-136">Response</span></span>
<span data-ttu-id="cac83-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cac83-137">The following is an example of the response.</span></span>
><span data-ttu-id="cac83-138">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="cac83-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cac83-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="cac83-139">All the properties will be returned from an actual call.</span></span>
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
      "@odata.type": "#microsoft.graph.user"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="cac83-140">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="cac83-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cac83-141">C#</span><span class="sxs-lookup"><span data-stu-id="cac83-141">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_owners-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cac83-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="cac83-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_owners-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-list-owners.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-list-owners.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
