---
title: 削除済みアイテムを一覧表示する
description: '[削除済みアイテム] から、最近削除されたアイテムのリストを取得します。'
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5d1fdf1b81ce315266cb63c9e5623caf0c161b18
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33590692"
---
# <a name="list-deleted-items"></a><span data-ttu-id="5744e-103">削除済みアイテムを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="5744e-103">List deleted items</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5744e-104">[[削除済みアイテム]](../resources/directory.md) から、最近削除されたアイテムのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="5744e-104">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="5744e-105">現在、[削除済みアイテム] 機能は [group](../resources/group.md) および [user](../resources/user.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="5744e-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="5744e-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5744e-106">Permissions</span></span>
<span data-ttu-id="5744e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5744e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="5744e-109">User. all、Directory.accessasuser.all、および all。すべてのユーザーの場合、すべてのユーザーが対象となります。</span><span class="sxs-lookup"><span data-stu-id="5744e-109">For users: User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="5744e-110">グループの場合は、すべての Directory.accessasuser.all、およびすべてのディレクトリを取得します。すべてのグループについて、</span><span class="sxs-lookup"><span data-stu-id="5744e-110">For groups: Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="5744e-111">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5744e-111">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="5744e-112">この API は現在、削除済みアイテムからのグループ (microsoft.graph.group) またはユーザー (microsoft.graph.user) のオブジェクト タイプの取得をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="5744e-112">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="5744e-113">タイムは、URI の必須部分として指定します。</span><span class="sxs-lookup"><span data-stu-id="5744e-113">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="5744e-114">タイプが指定されていない GET /directory/deleteditems の呼び出しはサポートされません。</span><span class="sxs-lookup"><span data-stu-id="5744e-114">Calling GET /directory/deleteditems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="5744e-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5744e-115">Optional query parameters</span></span>
<span data-ttu-id="5744e-116">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5744e-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5744e-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5744e-117">Request headers</span></span>
| <span data-ttu-id="5744e-118">名前</span><span class="sxs-lookup"><span data-stu-id="5744e-118">Name</span></span>      |<span data-ttu-id="5744e-119">説明</span><span class="sxs-lookup"><span data-stu-id="5744e-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5744e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5744e-120">Authorization</span></span>  | <span data-ttu-id="5744e-121">ベアラー &lt;コード&gt; が*必要*</span><span class="sxs-lookup"><span data-stu-id="5744e-121">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="5744e-122">承諾</span><span class="sxs-lookup"><span data-stu-id="5744e-122">Accept</span></span>  | <span data-ttu-id="5744e-123">application/json</span><span class="sxs-lookup"><span data-stu-id="5744e-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5744e-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="5744e-124">Request body</span></span>
<span data-ttu-id="5744e-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5744e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5744e-126">応答</span><span class="sxs-lookup"><span data-stu-id="5744e-126">Response</span></span>

<span data-ttu-id="5744e-127">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="5744e-127">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5744e-128">例</span><span class="sxs-lookup"><span data-stu-id="5744e-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5744e-129">要求</span><span class="sxs-lookup"><span data-stu-id="5744e-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```http
GET https://graph.microsoft.com/beta/directory/deleteditems/microsoft.graph.group
```
##### <a name="response"></a><span data-ttu-id="5744e-130">応答</span><span class="sxs-lookup"><span data-stu-id="5744e-130">Response</span></span>
<span data-ttu-id="5744e-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5744e-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5744e-133">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="5744e-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5744e-134">Visual</span><span class="sxs-lookup"><span data-stu-id="5744e-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_deleteditems-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5744e-135">Java</span><span class="sxs-lookup"><span data-stu-id="5744e-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_deleteditems-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/directory-deleteditems-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directory-deleteditems-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
