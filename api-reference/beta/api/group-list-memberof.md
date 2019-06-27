---
title: リストグループの memberOf
description: グループが直接メンバーであるグループおよび管理単位を取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 35b715e0ef24ad199b5d77d909a8561a97d176f2
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263001"
---
# <a name="list-group-memberof"></a><span data-ttu-id="15631-103">リストグループの memberOf</span><span class="sxs-lookup"><span data-stu-id="15631-103">List group memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15631-104">グループが直接メンバーであるグループおよび管理単位を取得します。</span><span class="sxs-lookup"><span data-stu-id="15631-104">Get groups and administrative units that the group is a direct member of.</span></span>

<span data-ttu-id="15631-p101">この操作は推移的ではありません。ユーザーの Office 365 グループを取得する場合とは異なり、Office 365 グループだけでなく、すべての種類のグループを返します。</span><span class="sxs-lookup"><span data-stu-id="15631-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span> 

## <a name="permissions"></a><span data-ttu-id="15631-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="15631-107">Permissions</span></span>

<span data-ttu-id="15631-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="15631-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15631-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="15631-110">Permission type</span></span>      | <span data-ttu-id="15631-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="15631-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15631-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="15631-112">Delegated (work or school account)</span></span> | <span data-ttu-id="15631-113">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="15631-113">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="15631-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="15631-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15631-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15631-115">Not supported.</span></span>    |
|<span data-ttu-id="15631-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="15631-116">Application</span></span> | <span data-ttu-id="15631-117">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15631-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="15631-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="15631-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="15631-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="15631-119">Optional query parameters</span></span>
<span data-ttu-id="15631-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="15631-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="15631-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="15631-121">Request headers</span></span>
| <span data-ttu-id="15631-122">名前</span><span class="sxs-lookup"><span data-stu-id="15631-122">Name</span></span>       | <span data-ttu-id="15631-123">型</span><span class="sxs-lookup"><span data-stu-id="15631-123">Type</span></span> | <span data-ttu-id="15631-124">説明</span><span class="sxs-lookup"><span data-stu-id="15631-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="15631-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="15631-125">Authorization</span></span>  | <span data-ttu-id="15631-126">string</span><span class="sxs-lookup"><span data-stu-id="15631-126">string</span></span>  | <span data-ttu-id="15631-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="15631-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15631-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="15631-129">Request body</span></span>
<span data-ttu-id="15631-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="15631-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15631-131">応答</span><span class="sxs-lookup"><span data-stu-id="15631-131">Response</span></span>
<span data-ttu-id="15631-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="15631-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15631-133">例</span><span class="sxs-lookup"><span data-stu-id="15631-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="15631-134">要求</span><span class="sxs-lookup"><span data-stu-id="15631-134">Request</span></span>

<span data-ttu-id="15631-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="15631-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="15631-136">応答</span><span class="sxs-lookup"><span data-stu-id="15631-136">Response</span></span>

<span data-ttu-id="15631-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="15631-137">The following is an example of the response.</span></span>
><span data-ttu-id="15631-138">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="15631-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="15631-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="15631-139">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="15631-140">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="15631-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="15631-141">C#</span><span class="sxs-lookup"><span data-stu-id="15631-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_memberof-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="15631-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="15631-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_memberof-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="15631-143">目的-C</span><span class="sxs-lookup"><span data-stu-id="15631-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_memberof-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-memberof.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-list-memberof.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-list-memberof.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
