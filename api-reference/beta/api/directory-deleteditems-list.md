---
title: 削除済みアイテムを一覧表示する
description: '[削除済みアイテム] から、最近削除されたアイテムのリストを取得します。'
author: lleonard-msft
ms.openlocfilehash: 205052402f4402b9895cca6cc46b6ab656a51ed8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358724"
---
# <a name="list-deleted-items"></a><span data-ttu-id="30dbb-103">削除済みアイテムを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="30dbb-103">List deleted items</span></span>

> <span data-ttu-id="30dbb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="30dbb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="30dbb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="30dbb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="30dbb-106">[[削除済みアイテム]](../resources/directory.md) から、最近削除されたアイテムのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="30dbb-106">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="30dbb-107">現在、[削除済みアイテム] 機能は [group](../resources/group.md) および [user](../resources/user.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="30dbb-107">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="30dbb-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="30dbb-108">Permissions</span></span>
<span data-ttu-id="30dbb-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="30dbb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="30dbb-111">ユーザー: User.Read.All、Directory.Read.All、User.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="30dbb-111">For users: User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="30dbb-112">グループ: Group.Read.All、Directory.Read.All、Group.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="30dbb-112">For groups: Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="30dbb-113">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="30dbb-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="30dbb-114">この API は現在、削除済みアイテムからのグループ (microsoft.graph.group) またはユーザー (microsoft.graph.user) のオブジェクト タイプの取得をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="30dbb-114">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="30dbb-115">タイムは、URI の必須部分として指定します。</span><span class="sxs-lookup"><span data-stu-id="30dbb-115">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="30dbb-116">タイプが指定されていない GET /directory/deleteditems の呼び出しはサポートされません。</span><span class="sxs-lookup"><span data-stu-id="30dbb-116">Calling GET /directory/deleteditems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="30dbb-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="30dbb-117">Optional query parameters</span></span>
<span data-ttu-id="30dbb-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="30dbb-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="30dbb-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="30dbb-119">Request headers</span></span>
| <span data-ttu-id="30dbb-120">名前</span><span class="sxs-lookup"><span data-stu-id="30dbb-120">Name</span></span>      |<span data-ttu-id="30dbb-121">説明</span><span class="sxs-lookup"><span data-stu-id="30dbb-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="30dbb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="30dbb-122">Authorization</span></span>  | <span data-ttu-id="30dbb-123">ベアラー &lt;コード&gt; が*必要*</span><span class="sxs-lookup"><span data-stu-id="30dbb-123">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="30dbb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="30dbb-124">Accept</span></span>  | <span data-ttu-id="30dbb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="30dbb-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="30dbb-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="30dbb-126">Request body</span></span>
<span data-ttu-id="30dbb-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="30dbb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30dbb-128">応答</span><span class="sxs-lookup"><span data-stu-id="30dbb-128">Response</span></span>

<span data-ttu-id="30dbb-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="30dbb-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="30dbb-130">例</span><span class="sxs-lookup"><span data-stu-id="30dbb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="30dbb-131">要求</span><span class="sxs-lookup"><span data-stu-id="30dbb-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```http
GET https://graph.microsoft.com/beta/directory/deleteditems/microsoft.graph.group
```
##### <a name="response"></a><span data-ttu-id="30dbb-132">応答</span><span class="sxs-lookup"><span data-stu-id="30dbb-132">Response</span></span>
<span data-ttu-id="30dbb-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="30dbb-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List deleteditems",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->