---
title: 削除済みアイテムを一覧表示する
description: '[削除済みアイテム] から、最近削除されたアイテムのリストを取得します。'
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9c132ba47ebc9e91d30b92f3361ee334f236c772
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417526"
---
# <a name="list-deleted-items"></a><span data-ttu-id="996e0-103">削除済みアイテムを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="996e0-103">List deleted items</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="996e0-104">[[削除済みアイテム]](../resources/directory.md) から、最近削除されたアイテムのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="996e0-104">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="996e0-105">現在、[削除済みアイテム] 機能は [group](../resources/group.md) および [user](../resources/user.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="996e0-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="996e0-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="996e0-106">Permissions</span></span>
<span data-ttu-id="996e0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="996e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="996e0-109">User. all、Directory.accessasuser.all、および all。すべてのユーザーの場合、すべてのユーザーが対象となります。</span><span class="sxs-lookup"><span data-stu-id="996e0-109">For users: User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="996e0-110">グループの場合は、すべての Directory.accessasuser.all、およびすべてのディレクトリを取得します。すべてのグループについて、</span><span class="sxs-lookup"><span data-stu-id="996e0-110">For groups: Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="996e0-111">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="996e0-111">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="996e0-112">この API は現在、削除済みアイテムからのグループ (microsoft.graph.group) またはユーザー (microsoft.graph.user) のオブジェクト タイプの取得をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="996e0-112">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="996e0-113">タイムは、URI の必須部分として指定します。</span><span class="sxs-lookup"><span data-stu-id="996e0-113">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="996e0-114">タイプが指定されていない GET /directory/deleteditems の呼び出しはサポートされません。</span><span class="sxs-lookup"><span data-stu-id="996e0-114">Calling GET /directory/deleteditems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="996e0-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="996e0-115">Optional query parameters</span></span>
<span data-ttu-id="996e0-116">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="996e0-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="996e0-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="996e0-117">Request headers</span></span>
| <span data-ttu-id="996e0-118">名前</span><span class="sxs-lookup"><span data-stu-id="996e0-118">Name</span></span>      |<span data-ttu-id="996e0-119">説明</span><span class="sxs-lookup"><span data-stu-id="996e0-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="996e0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="996e0-120">Authorization</span></span>  | <span data-ttu-id="996e0-121">ベアラー &lt;コード&gt; が*必要*</span><span class="sxs-lookup"><span data-stu-id="996e0-121">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="996e0-122">承諾</span><span class="sxs-lookup"><span data-stu-id="996e0-122">Accept</span></span>  | <span data-ttu-id="996e0-123">application/json</span><span class="sxs-lookup"><span data-stu-id="996e0-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="996e0-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="996e0-124">Request body</span></span>
<span data-ttu-id="996e0-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="996e0-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="996e0-126">応答</span><span class="sxs-lookup"><span data-stu-id="996e0-126">Response</span></span>

<span data-ttu-id="996e0-127">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="996e0-127">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="996e0-128">例</span><span class="sxs-lookup"><span data-stu-id="996e0-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="996e0-129">要求</span><span class="sxs-lookup"><span data-stu-id="996e0-129">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="996e0-130">プロトコル</span><span class="sxs-lookup"><span data-stu-id="996e0-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```http
GET https://graph.microsoft.com/beta/directory/deleteditems/microsoft.graph.group
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="996e0-131">C#</span><span class="sxs-lookup"><span data-stu-id="996e0-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-deleteditems-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="996e0-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="996e0-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-deleteditems-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="996e0-133">目的-C</span><span class="sxs-lookup"><span data-stu-id="996e0-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-deleteditems-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="996e0-134">応答</span><span class="sxs-lookup"><span data-stu-id="996e0-134">Response</span></span>
<span data-ttu-id="996e0-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="996e0-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "value": [
    {
      "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
      "displayName":"SampleGroup",
      "groupTypes":["Unified"],
      "mail":"example@contoso.com",
      "mailEnabled":true,
      "mailNickname":"Example",
      "securityEnabled":false,
      "visibility":"Public"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List deleteditems",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
