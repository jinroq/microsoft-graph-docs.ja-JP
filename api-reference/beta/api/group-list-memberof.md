---
title: リストグループの memberOf
description: グループが直接メンバーであるグループおよび管理単位を取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 311837236f20039178ee4865489a83baa9fd8c1a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33592947"
---
# <a name="list-group-memberof"></a><span data-ttu-id="d0ead-103">リストグループの memberOf</span><span class="sxs-lookup"><span data-stu-id="d0ead-103">List group memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0ead-104">グループが直接メンバーであるグループおよび管理単位を取得します。</span><span class="sxs-lookup"><span data-stu-id="d0ead-104">Get groups and administrative units that the group is a direct member of.</span></span>

<span data-ttu-id="d0ead-p101">この操作は推移的ではありません。ユーザーの Office 365 グループを取得する場合とは異なり、Office 365 グループだけでなく、すべての種類のグループを返します。</span><span class="sxs-lookup"><span data-stu-id="d0ead-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span> 

## <a name="permissions"></a><span data-ttu-id="d0ead-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d0ead-107">Permissions</span></span>

<span data-ttu-id="d0ead-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d0ead-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0ead-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d0ead-110">Permission type</span></span>      | <span data-ttu-id="d0ead-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d0ead-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0ead-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d0ead-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d0ead-113">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d0ead-113">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d0ead-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d0ead-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0ead-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0ead-115">Not supported.</span></span>    |
|<span data-ttu-id="d0ead-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d0ead-116">Application</span></span> | <span data-ttu-id="d0ead-117">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0ead-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0ead-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d0ead-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d0ead-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d0ead-119">Optional query parameters</span></span>
<span data-ttu-id="d0ead-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d0ead-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d0ead-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d0ead-121">Request headers</span></span>
| <span data-ttu-id="d0ead-122">名前</span><span class="sxs-lookup"><span data-stu-id="d0ead-122">Name</span></span>       | <span data-ttu-id="d0ead-123">型</span><span class="sxs-lookup"><span data-stu-id="d0ead-123">Type</span></span> | <span data-ttu-id="d0ead-124">説明</span><span class="sxs-lookup"><span data-stu-id="d0ead-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d0ead-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0ead-125">Authorization</span></span>  | <span data-ttu-id="d0ead-126">string</span><span class="sxs-lookup"><span data-stu-id="d0ead-126">string</span></span>  | <span data-ttu-id="d0ead-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d0ead-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0ead-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="d0ead-129">Request body</span></span>
<span data-ttu-id="d0ead-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d0ead-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0ead-131">応答</span><span class="sxs-lookup"><span data-stu-id="d0ead-131">Response</span></span>
<span data-ttu-id="d0ead-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d0ead-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0ead-133">例</span><span class="sxs-lookup"><span data-stu-id="d0ead-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0ead-134">要求</span><span class="sxs-lookup"><span data-stu-id="d0ead-134">Request</span></span>

<span data-ttu-id="d0ead-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d0ead-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="d0ead-136">応答</span><span class="sxs-lookup"><span data-stu-id="d0ead-136">Response</span></span>

<span data-ttu-id="d0ead-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d0ead-137">The following is an example of the response.</span></span>
><span data-ttu-id="d0ead-138">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="d0ead-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d0ead-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d0ead-139">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d0ead-140">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="d0ead-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d0ead-141">Visual</span><span class="sxs-lookup"><span data-stu-id="d0ead-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_memberof-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d0ead-142">Java</span><span class="sxs-lookup"><span data-stu-id="d0ead-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_memberof-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/group-list-memberof.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-list-memberof.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
