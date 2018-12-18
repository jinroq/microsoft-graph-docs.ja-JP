---
title: 削除済みアイテムを取得する
description: '[削除済みアイテム] から、最近削除されたアイテムのプロパティを取得します。'
author: lleonard-msft
ms.openlocfilehash: 38961b6151ab4b5ec9dfe8d72cc82cd6c48a28f6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322534"
---
# <a name="get-deleted-item"></a><span data-ttu-id="2fab1-103">削除済みアイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="2fab1-103">Get deleted item</span></span>

> <span data-ttu-id="2fab1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2fab1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2fab1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2fab1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2fab1-106">[[削除済みアイテム]](../resources/directory.md) から、最近削除されたアイテムのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="2fab1-106">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="2fab1-107">現在、[削除済みアイテム] 機能は [group](../resources/group.md) および [user](../resources/user.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="2fab1-107">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="2fab1-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2fab1-108">Permissions</span></span>
<span data-ttu-id="2fab1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2fab1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="2fab1-111">ユーザー: User.Read.All、User.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2fab1-111">For users: User.Read.All, User.ReadWrite.All, Directory.Read.All</span></span>
* <span data-ttu-id="2fab1-112">グループ: Group.Read.All、Group.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2fab1-112">For groups: Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span>

## <a name="http-request"></a><span data-ttu-id="2fab1-113">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2fab1-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deleteditems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2fab1-114">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2fab1-114">Optional query parameters</span></span>
<span data-ttu-id="2fab1-115">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2fab1-115">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2fab1-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2fab1-116">Request headers</span></span>
| <span data-ttu-id="2fab1-117">名前</span><span class="sxs-lookup"><span data-stu-id="2fab1-117">Name</span></span>      |<span data-ttu-id="2fab1-118">説明</span><span class="sxs-lookup"><span data-stu-id="2fab1-118">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2fab1-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2fab1-119">Authorization</span></span>  | <span data-ttu-id="2fab1-120">ベアラー &lt;コード&gt; が*必要*</span><span class="sxs-lookup"><span data-stu-id="2fab1-120">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="2fab1-121">Accept</span><span class="sxs-lookup"><span data-stu-id="2fab1-121">Accept</span></span>  | <span data-ttu-id="2fab1-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2fab1-122">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2fab1-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="2fab1-123">Request body</span></span>
<span data-ttu-id="2fab1-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2fab1-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2fab1-125">応答</span><span class="sxs-lookup"><span data-stu-id="2fab1-125">Response</span></span>

<span data-ttu-id="2fab1-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2fab1-126">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2fab1-127">例</span><span class="sxs-lookup"><span data-stu-id="2fab1-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2fab1-128">要求</span><span class="sxs-lookup"><span data-stu-id="2fab1-128">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
##### <a name="response"></a><span data-ttu-id="2fab1-129">応答</span><span class="sxs-lookup"><span data-stu-id="2fab1-129">Response</span></span>
<span data-ttu-id="2fab1-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2fab1-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->