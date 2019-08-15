---
title: 削除済みアイテムを取得する
description: '[削除済みアイテム] から、最近削除されたアイテムのプロパティを取得します。'
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 44f4f91bcdd883b500a469a99646aec32b524f25
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417517"
---
# <a name="get-deleted-item"></a><span data-ttu-id="d7763-103">削除済みアイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="d7763-103">Get deleted item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7763-104">[[削除済みアイテム]](../resources/directory.md) から、最近削除されたアイテムのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="d7763-104">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="d7763-105">現在、[削除済みアイテム] 機能は [group](../resources/group.md) および [user](../resources/user.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="d7763-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7763-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d7763-106">Permissions</span></span>
<span data-ttu-id="d7763-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7763-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="d7763-109">ユーザーの場合: ユーザー。すべて。すべてのユーザーに対して読み取り。</span><span class="sxs-lookup"><span data-stu-id="d7763-109">For users: User.Read.All, User.ReadWrite.All, Directory.Read.All</span></span>
* <span data-ttu-id="d7763-110">グループの場合は、すべてのディレクトリを取得します。すべてのグループを取得します。</span><span class="sxs-lookup"><span data-stu-id="d7763-110">For groups: Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span>

## <a name="http-request"></a><span data-ttu-id="d7763-111">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d7763-111">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deleteditems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d7763-112">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d7763-112">Optional query parameters</span></span>
<span data-ttu-id="d7763-113">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d7763-113">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d7763-114">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d7763-114">Request headers</span></span>
| <span data-ttu-id="d7763-115">名前</span><span class="sxs-lookup"><span data-stu-id="d7763-115">Name</span></span>      |<span data-ttu-id="d7763-116">説明</span><span class="sxs-lookup"><span data-stu-id="d7763-116">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d7763-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7763-117">Authorization</span></span>  | <span data-ttu-id="d7763-118">ベアラー &lt;コード&gt; が*必要*</span><span class="sxs-lookup"><span data-stu-id="d7763-118">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="d7763-119">承諾</span><span class="sxs-lookup"><span data-stu-id="d7763-119">Accept</span></span>  | <span data-ttu-id="d7763-120">application/json</span><span class="sxs-lookup"><span data-stu-id="d7763-120">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7763-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="d7763-121">Request body</span></span>
<span data-ttu-id="d7763-122">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d7763-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7763-123">応答</span><span class="sxs-lookup"><span data-stu-id="d7763-123">Response</span></span>

<span data-ttu-id="d7763-124">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d7763-124">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d7763-125">例</span><span class="sxs-lookup"><span data-stu-id="d7763-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d7763-126">要求</span><span class="sxs-lookup"><span data-stu-id="d7763-126">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d7763-127">プロトコル</span><span class="sxs-lookup"><span data-stu-id="d7763-127">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d7763-128">C#</span><span class="sxs-lookup"><span data-stu-id="d7763-128">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d7763-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7763-129">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d7763-130">目的-C</span><span class="sxs-lookup"><span data-stu-id="d7763-130">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d7763-131">応答</span><span class="sxs-lookup"><span data-stu-id="d7763-131">Response</span></span>
<span data-ttu-id="d7763-p102">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d7763-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directory"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects/$entity",
  "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
  "displayName":"SampleGroup",
  "groupTypes":["Unified"],
  "mail":"example@contoso.com",
  "mailEnabled":true,
  "mailNickname":"Example",
  "securityEnabled":false,
  "visibility":"Public"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
