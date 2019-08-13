---
title: アイテムを完全に削除する
description: '[削除済みアイテム] からアイテムを完全に削除します。'
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8b4765992016a5fb19a7fecb3d51a820d63c3c34
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321373"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="ad109-103">アイテムを完全に削除する</span><span class="sxs-lookup"><span data-stu-id="ad109-103">Permanently delete item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad109-104">[[削除済みアイテム]](../resources/directory.md) からアイテムを完全に削除します。</span><span class="sxs-lookup"><span data-stu-id="ad109-104">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="ad109-105">現在、[削除済みアイテム] 機能は [group](../resources/group.md) および [user](../resources/user.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="ad109-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="ad109-106">[削除済みアイテム] から、アイテムを完全に削除できます。</span><span class="sxs-lookup"><span data-stu-id="ad109-106">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="ad109-107">ただし、アイテムを完全に削除すると、そのアイテムを復元することが**不可能**になります。</span><span class="sxs-lookup"><span data-stu-id="ad109-107">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad109-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ad109-108">Permissions</span></span>
<span data-ttu-id="ad109-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ad109-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="ad109-111">ユーザーの場合: Directory.accessasuser.all、すべてのユーザー</span><span class="sxs-lookup"><span data-stu-id="ad109-111">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="ad109-112">グループの場合: Directory.accessasuser.all、all、および All</span><span class="sxs-lookup"><span data-stu-id="ad109-112">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="ad109-113">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ad109-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deleteditems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ad109-114">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad109-114">Request headers</span></span>
| <span data-ttu-id="ad109-115">名前</span><span class="sxs-lookup"><span data-stu-id="ad109-115">Name</span></span>       | <span data-ttu-id="ad109-116">説明</span><span class="sxs-lookup"><span data-stu-id="ad109-116">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ad109-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad109-117">Authorization</span></span>  | <span data-ttu-id="ad109-118">ベアラー &lt;コード&gt; が*必要*</span><span class="sxs-lookup"><span data-stu-id="ad109-118">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="ad109-119">承諾</span><span class="sxs-lookup"><span data-stu-id="ad109-119">Accept</span></span>  | <span data-ttu-id="ad109-120">application/json</span><span class="sxs-lookup"><span data-stu-id="ad109-120">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad109-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="ad109-121">Request body</span></span>
<span data-ttu-id="ad109-122">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ad109-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad109-123">応答</span><span class="sxs-lookup"><span data-stu-id="ad109-123">Response</span></span>

<span data-ttu-id="ad109-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ad109-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad109-126">例</span><span class="sxs-lookup"><span data-stu-id="ad109-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad109-127">要求</span><span class="sxs-lookup"><span data-stu-id="ad109-127">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ad109-128">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ad109-128">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ad109-129">C#</span><span class="sxs-lookup"><span data-stu-id="ad109-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ad109-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad109-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ad109-131">目的-C</span><span class="sxs-lookup"><span data-stu-id="ad109-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ad109-132">Java</span><span class="sxs-lookup"><span data-stu-id="ad109-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ad109-133">応答</span><span class="sxs-lookup"><span data-stu-id="ad109-133">Response</span></span>
<span data-ttu-id="ad109-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ad109-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
