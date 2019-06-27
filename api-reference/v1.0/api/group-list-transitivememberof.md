---
title: リストグループ推移的な memberOf
description: グループがメンバーであるグループを取得します。  この操作は推移的で、このグループがネストされたメンバーであるすべてのグループも含みます。 ユーザーの Office 365 グループを取得する場合とは異なり、Office 365 グループだけでなく、すべての種類のグループを返します。
author: anchanda
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 0642a686c23cc2bbe1a87fd0439a8b34ff3ca38c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277897"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="6a915-105">リストグループ推移的な memberOf</span><span class="sxs-lookup"><span data-stu-id="6a915-105">List group transitive memberOf</span></span>

<span data-ttu-id="6a915-106">グループがメンバーであるグループを取得します。</span><span class="sxs-lookup"><span data-stu-id="6a915-106">Get groups that the group is a member of.</span></span>  <span data-ttu-id="6a915-107">この操作は推移的で、このグループがネストされたメンバーであるすべてのグループも含みます。</span><span class="sxs-lookup"><span data-stu-id="6a915-107">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="6a915-108">ユーザーの Office 365 グループを取得する場合とは異なり、Office 365 グループだけでなく、すべての種類のグループを返します。</span><span class="sxs-lookup"><span data-stu-id="6a915-108">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a915-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6a915-109">Permissions</span></span>

<span data-ttu-id="6a915-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6a915-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a915-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6a915-112">Permission type</span></span>      | <span data-ttu-id="6a915-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6a915-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a915-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6a915-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6a915-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6a915-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6a915-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6a915-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a915-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a915-117">Not supported.</span></span>    |
|<span data-ttu-id="6a915-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6a915-118">Application</span></span> | <span data-ttu-id="6a915-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a915-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a915-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6a915-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6a915-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6a915-121">Optional query parameters</span></span>
<span data-ttu-id="6a915-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6a915-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6a915-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a915-123">Request headers</span></span>
| <span data-ttu-id="6a915-124">名前</span><span class="sxs-lookup"><span data-stu-id="6a915-124">Name</span></span>       | <span data-ttu-id="6a915-125">型</span><span class="sxs-lookup"><span data-stu-id="6a915-125">Type</span></span> | <span data-ttu-id="6a915-126">説明</span><span class="sxs-lookup"><span data-stu-id="6a915-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6a915-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a915-127">Authorization</span></span>  | <span data-ttu-id="6a915-128">string</span><span class="sxs-lookup"><span data-stu-id="6a915-128">string</span></span>  | <span data-ttu-id="6a915-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6a915-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a915-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="6a915-131">Request body</span></span>
<span data-ttu-id="6a915-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6a915-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a915-133">応答</span><span class="sxs-lookup"><span data-stu-id="6a915-133">Response</span></span>
<span data-ttu-id="6a915-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="6a915-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a915-135">例</span><span class="sxs-lookup"><span data-stu-id="6a915-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a915-136">要求</span><span class="sxs-lookup"><span data-stu-id="6a915-136">Request</span></span>
<span data-ttu-id="6a915-137">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6a915-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="6a915-138">応答</span><span class="sxs-lookup"><span data-stu-id="6a915-138">Response</span></span>

<span data-ttu-id="6a915-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6a915-139">The following is an example of the response.</span></span>
><span data-ttu-id="6a915-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6a915-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6a915-142">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="6a915-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6a915-143">C#</span><span class="sxs-lookup"><span data-stu-id="6a915-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group_transitivememberof-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6a915-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="6a915-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group_transitivememberof-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6a915-145">目的-C</span><span class="sxs-lookup"><span data-stu-id="6a915-145">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_group_transitivememberof-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List group transitive memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-list-transitivememberof.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-list-transitivememberof.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-list-transitivememberof.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
