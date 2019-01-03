---
title: 削除済みアイテムを一覧表示する
description: '[削除済みアイテム] から、最近削除されたアイテムのリストを取得します。'
author: lleonard-msft
ms.openlocfilehash: 4c972ca554f7a073ddfb5b3472784240c691c973
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314281"
---
# <a name="list-deleted-items"></a><span data-ttu-id="12683-103">削除済みアイテムを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="12683-103">List deleted items</span></span>

<span data-ttu-id="12683-104">[[削除済みアイテム]](../resources/directory.md) から、最近削除されたアイテムのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="12683-104">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="12683-105">現在、[削除済みアイテム] 機能は [group](../resources/group.md) および [user](../resources/user.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="12683-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="12683-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="12683-106">Permissions</span></span>
<span data-ttu-id="12683-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="12683-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="12683-109">ユーザーの場合:</span><span class="sxs-lookup"><span data-stu-id="12683-109">For users:</span></span>

|<span data-ttu-id="12683-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="12683-110">Permission type</span></span>      | <span data-ttu-id="12683-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="12683-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12683-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="12683-112">Delegated (work or school account)</span></span> | <span data-ttu-id="12683-113">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="12683-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="12683-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="12683-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12683-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12683-115">Not supported.</span></span> |
|<span data-ttu-id="12683-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="12683-116">Application</span></span> | <span data-ttu-id="12683-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12683-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="12683-118">グループの場合:</span><span class="sxs-lookup"><span data-stu-id="12683-118">For groups:</span></span>

|<span data-ttu-id="12683-119">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="12683-119">Permission type</span></span>      | <span data-ttu-id="12683-120">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="12683-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12683-121">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="12683-121">Delegated (work or school account)</span></span> | <span data-ttu-id="12683-122">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="12683-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="12683-123">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="12683-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12683-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12683-124">Not supported.</span></span>    |
|<span data-ttu-id="12683-125">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="12683-125">Application</span></span> | <span data-ttu-id="12683-126">Group.Read.All、Group.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="12683-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="12683-127">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="12683-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deletedItems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="12683-128">この API は現在、削除済みアイテムからのグループ (microsoft.graph.group) またはユーザー (microsoft.graph.user) のオブジェクト タイプの取得をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="12683-128">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="12683-129">タイムは、URI の必須部分として指定します。</span><span class="sxs-lookup"><span data-stu-id="12683-129">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="12683-130">GET/ディレクトリ/を呼び出す型のない deletedItems はサポートされません。</span><span class="sxs-lookup"><span data-stu-id="12683-130">Calling GET /directory/deletedItems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="12683-131">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="12683-131">Optional query parameters</span></span>
<span data-ttu-id="12683-132">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="12683-132">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="12683-133">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="12683-133">Request headers</span></span>
| <span data-ttu-id="12683-134">名前</span><span class="sxs-lookup"><span data-stu-id="12683-134">Name</span></span>      |<span data-ttu-id="12683-135">説明</span><span class="sxs-lookup"><span data-stu-id="12683-135">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="12683-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="12683-136">Authorization</span></span>  | <span data-ttu-id="12683-137">ベアラー &lt;コード&gt; が*必要*</span><span class="sxs-lookup"><span data-stu-id="12683-137">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="12683-138">Accept</span><span class="sxs-lookup"><span data-stu-id="12683-138">Accept</span></span>  | <span data-ttu-id="12683-139">application/json</span><span class="sxs-lookup"><span data-stu-id="12683-139">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="12683-140">要求本文</span><span class="sxs-lookup"><span data-stu-id="12683-140">Request body</span></span>
<span data-ttu-id="12683-141">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="12683-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12683-142">応答</span><span class="sxs-lookup"><span data-stu-id="12683-142">Response</span></span>

<span data-ttu-id="12683-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="12683-143">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="12683-144">例</span><span class="sxs-lookup"><span data-stu-id="12683-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12683-145">要求</span><span class="sxs-lookup"><span data-stu-id="12683-145">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.group
```
##### <a name="response"></a><span data-ttu-id="12683-146">応答</span><span class="sxs-lookup"><span data-stu-id="12683-146">Response</span></span>
<span data-ttu-id="12683-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="12683-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
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