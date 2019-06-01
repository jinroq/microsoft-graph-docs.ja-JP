---
title: 削除済みアイテムを復元する
description: '[削除済みアイテム] から、最近削除されたアイテムを復元します。 '
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 93944a8327405344a543302556070e7058464040
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34656168"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="cb5f1-103">削除済みアイテムを復元する</span><span class="sxs-lookup"><span data-stu-id="cb5f1-103">Restore deleted item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb5f1-104">[[削除済みアイテム]](../resources/directory.md) から、最近削除されたアイテムを復元します。</span><span class="sxs-lookup"><span data-stu-id="cb5f1-104">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="cb5f1-105">現在、[削除済みアイテム] 機能は [group](../resources/group.md) および [user](../resources/user.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="cb5f1-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="cb5f1-106">アイテムを誤って削除してしまった場合、そのアイテムを完全に復元できます。</span><span class="sxs-lookup"><span data-stu-id="cb5f1-106">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="cb5f1-107">最近削除されたアイテムは、最大 30 日間、使用可能な状態に維持されます。</span><span class="sxs-lookup"><span data-stu-id="cb5f1-107">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="cb5f1-108">30 日が経過すると、アイテムは完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="cb5f1-108">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb5f1-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cb5f1-109">Permissions</span></span>
<span data-ttu-id="cb5f1-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cb5f1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="cb5f1-112">ユーザーの場合: Directory.accessasuser.all、すべてのユーザー</span><span class="sxs-lookup"><span data-stu-id="cb5f1-112">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="cb5f1-113">グループの場合: Directory.accessasuser.all、all、および All</span><span class="sxs-lookup"><span data-stu-id="cb5f1-113">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="cb5f1-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cb5f1-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deleteditems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="cb5f1-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cb5f1-115">Request headers</span></span>
| <span data-ttu-id="cb5f1-116">名前</span><span class="sxs-lookup"><span data-stu-id="cb5f1-116">Name</span></span>       | <span data-ttu-id="cb5f1-117">説明</span><span class="sxs-lookup"><span data-stu-id="cb5f1-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cb5f1-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb5f1-118">Authorization</span></span>  | <span data-ttu-id="cb5f1-119">ベアラー &lt;コード&gt; が*必要*</span><span class="sxs-lookup"><span data-stu-id="cb5f1-119">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="cb5f1-120">承諾</span><span class="sxs-lookup"><span data-stu-id="cb5f1-120">Accept</span></span> | <span data-ttu-id="cb5f1-121">application/json</span><span class="sxs-lookup"><span data-stu-id="cb5f1-121">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb5f1-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="cb5f1-122">Request body</span></span>
<span data-ttu-id="cb5f1-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cb5f1-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb5f1-124">応答</span><span class="sxs-lookup"><span data-stu-id="cb5f1-124">Response</span></span>

<span data-ttu-id="cb5f1-125">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cb5f1-125">If successful, this method returns `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb5f1-126">例</span><span class="sxs-lookup"><span data-stu-id="cb5f1-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cb5f1-127">要求</span><span class="sxs-lookup"><span data-stu-id="cb5f1-127">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb/restore
```
<span data-ttu-id="cb5f1-128">要求本文に、[directoryObject](../resources/directoryobject.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cb5f1-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="cb5f1-129">応答</span><span class="sxs-lookup"><span data-stu-id="cb5f1-129">Response</span></span>
<span data-ttu-id="cb5f1-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cb5f1-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="cb5f1-132">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="cb5f1-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cb5f1-133">C#</span><span class="sxs-lookup"><span data-stu-id="cb5f1-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_directory-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cb5f1-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="cb5f1-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_directory-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/directory-deleteditems-restore.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directory-deleteditems-restore.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
