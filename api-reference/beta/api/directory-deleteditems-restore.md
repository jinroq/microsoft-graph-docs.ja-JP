---
title: 削除済みアイテムを復元する
description: '[削除済みアイテム] から、最近削除されたアイテムを復元します。 '
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ff80911e02b9acaaf02abdedd9fd49bc1fc8a82a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437125"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="e1076-103">削除済みアイテムを復元する</span><span class="sxs-lookup"><span data-stu-id="e1076-103">Restore deleted item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1076-104">[[削除済みアイテム]](../resources/directory.md) から、最近削除されたアイテムを復元します。</span><span class="sxs-lookup"><span data-stu-id="e1076-104">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="e1076-105">現在、[削除済みアイテム] 機能は [group](../resources/group.md) および [user](../resources/user.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="e1076-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="e1076-106">アイテムを誤って削除してしまった場合、そのアイテムを完全に復元できます。</span><span class="sxs-lookup"><span data-stu-id="e1076-106">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="e1076-107">最近削除されたアイテムは、最大 30 日間、使用可能な状態に維持されます。</span><span class="sxs-lookup"><span data-stu-id="e1076-107">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="e1076-108">30 日が経過すると、アイテムは完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="e1076-108">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1076-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e1076-109">Permissions</span></span>
<span data-ttu-id="e1076-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e1076-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="e1076-112">ユーザーの場合: Directory.accessasuser.all、すべてのユーザー</span><span class="sxs-lookup"><span data-stu-id="e1076-112">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="e1076-113">グループの場合: Directory.accessasuser.all、all、および All</span><span class="sxs-lookup"><span data-stu-id="e1076-113">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="e1076-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e1076-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deleteditems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="e1076-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e1076-115">Request headers</span></span>
| <span data-ttu-id="e1076-116">名前</span><span class="sxs-lookup"><span data-stu-id="e1076-116">Name</span></span>       | <span data-ttu-id="e1076-117">説明</span><span class="sxs-lookup"><span data-stu-id="e1076-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e1076-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1076-118">Authorization</span></span>  | <span data-ttu-id="e1076-119">ベアラー &lt;コード&gt; が*必要*</span><span class="sxs-lookup"><span data-stu-id="e1076-119">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="e1076-120">承諾</span><span class="sxs-lookup"><span data-stu-id="e1076-120">Accept</span></span> | <span data-ttu-id="e1076-121">application/json</span><span class="sxs-lookup"><span data-stu-id="e1076-121">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1076-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="e1076-122">Request body</span></span>
<span data-ttu-id="e1076-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e1076-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1076-124">応答</span><span class="sxs-lookup"><span data-stu-id="e1076-124">Response</span></span>

<span data-ttu-id="e1076-125">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e1076-125">If successful, this method returns `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1076-126">例</span><span class="sxs-lookup"><span data-stu-id="e1076-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1076-127">要求</span><span class="sxs-lookup"><span data-stu-id="e1076-127">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e1076-128">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e1076-128">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb/restore
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e1076-129">C#</span><span class="sxs-lookup"><span data-stu-id="e1076-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e1076-130">Javascript</span><span class="sxs-lookup"><span data-stu-id="e1076-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e1076-131">目的-C</span><span class="sxs-lookup"><span data-stu-id="e1076-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="e1076-132">要求本文に、[directoryObject](../resources/directoryobject.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e1076-132">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e1076-133">応答</span><span class="sxs-lookup"><span data-stu-id="e1076-133">Response</span></span>
<span data-ttu-id="e1076-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e1076-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects/$entity",
  "@odata.type":"#microsoft.graph.group",
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
  "description": "Create deletedItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
