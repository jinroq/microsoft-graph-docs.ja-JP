---
title: 削除済みアイテムを取得する
description: '[削除済みアイテム] から、最近削除されたアイテムのプロパティを取得します。'
author: lleonard-msft
ms.openlocfilehash: e3a42fffba9a447661010ac9f6f5cff19df880c1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353712"
---
# <a name="get-deleted-item"></a><span data-ttu-id="8e60a-103">削除済みアイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="8e60a-103">Get deleted item</span></span>

<span data-ttu-id="8e60a-104">[[削除済みアイテム]](../resources/directory.md) から、最近削除されたアイテムのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="8e60a-104">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="8e60a-105">現在、[削除済みアイテム] 機能は [group](../resources/group.md) および [user](../resources/user.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="8e60a-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e60a-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8e60a-106">Permissions</span></span>
<span data-ttu-id="8e60a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8e60a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="8e60a-109">ユーザーの場合:</span><span class="sxs-lookup"><span data-stu-id="8e60a-109">For users:</span></span>

|<span data-ttu-id="8e60a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8e60a-110">Permission type</span></span>      | <span data-ttu-id="8e60a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8e60a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e60a-112">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="8e60a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8e60a-113">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8e60a-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span></span> |
|<span data-ttu-id="8e60a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8e60a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e60a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e60a-115">Not supported.</span></span> |
|<span data-ttu-id="8e60a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8e60a-116">Application</span></span> | <span data-ttu-id="8e60a-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e60a-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="8e60a-118">グループの場合:</span><span class="sxs-lookup"><span data-stu-id="8e60a-118">For groups:</span></span>

|<span data-ttu-id="8e60a-119">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8e60a-119">Permission type</span></span>      | <span data-ttu-id="8e60a-120">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8e60a-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e60a-121">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="8e60a-121">Delegated (work or school account)</span></span> | <span data-ttu-id="8e60a-122">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8e60a-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="8e60a-123">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8e60a-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e60a-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e60a-124">Not supported.</span></span>    |
|<span data-ttu-id="8e60a-125">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8e60a-125">Application</span></span> | <span data-ttu-id="8e60a-126">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e60a-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e60a-127">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8e60a-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deletedItems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8e60a-128">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8e60a-128">Optional query parameters</span></span>
<span data-ttu-id="8e60a-129">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8e60a-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e60a-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8e60a-130">Request headers</span></span>
| <span data-ttu-id="8e60a-131">名前</span><span class="sxs-lookup"><span data-stu-id="8e60a-131">Name</span></span>      |<span data-ttu-id="8e60a-132">説明</span><span class="sxs-lookup"><span data-stu-id="8e60a-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8e60a-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e60a-133">Authorization</span></span>  | <span data-ttu-id="8e60a-134">ベアラー &lt;コード&gt; が*必要*</span><span class="sxs-lookup"><span data-stu-id="8e60a-134">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="8e60a-135">Accept</span><span class="sxs-lookup"><span data-stu-id="8e60a-135">Accept</span></span>  | <span data-ttu-id="8e60a-136">application/json</span><span class="sxs-lookup"><span data-stu-id="8e60a-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e60a-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="8e60a-137">Request body</span></span>
<span data-ttu-id="8e60a-138">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8e60a-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e60a-139">応答</span><span class="sxs-lookup"><span data-stu-id="8e60a-139">Response</span></span>

<span data-ttu-id="8e60a-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8e60a-140">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8e60a-141">例</span><span class="sxs-lookup"><span data-stu-id="8e60a-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8e60a-142">要求</span><span class="sxs-lookup"><span data-stu-id="8e60a-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
##### <a name="response"></a><span data-ttu-id="8e60a-143">応答</span><span class="sxs-lookup"><span data-stu-id="8e60a-143">Response</span></span>
<span data-ttu-id="8e60a-p102">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8e60a-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
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