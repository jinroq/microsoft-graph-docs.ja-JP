---
title: アイテムを完全に削除する
description: '[削除済みアイテム] からアイテムを完全に削除します。'
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a22fd0ee6017dbd93735a739eb3cfb4336e432e5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015643"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="ee4da-103">アイテムを完全に削除する</span><span class="sxs-lookup"><span data-stu-id="ee4da-103">Permanently delete item</span></span>

<span data-ttu-id="ee4da-104">[[削除済みアイテム]](../resources/directory.md) からアイテムを完全に削除します。</span><span class="sxs-lookup"><span data-stu-id="ee4da-104">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="ee4da-105">現在、[削除済みアイテム] 機能は [group](../resources/group.md) および [user](../resources/user.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="ee4da-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="ee4da-106">[削除済みアイテム] から、アイテムを完全に削除できます。</span><span class="sxs-lookup"><span data-stu-id="ee4da-106">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="ee4da-107">ただし、アイテムを完全に削除すると、そのアイテムを復元することが**不可能**になります。</span><span class="sxs-lookup"><span data-stu-id="ee4da-107">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee4da-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ee4da-108">Permissions</span></span>
<span data-ttu-id="ee4da-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ee4da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="ee4da-111">ユーザーの場合:</span><span class="sxs-lookup"><span data-stu-id="ee4da-111">For users:</span></span>

|<span data-ttu-id="ee4da-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ee4da-112">Permission type</span></span>      | <span data-ttu-id="ee4da-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ee4da-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee4da-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ee4da-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ee4da-115">User.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ee4da-115">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="ee4da-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ee4da-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee4da-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee4da-117">Not supported.</span></span> |
|<span data-ttu-id="ee4da-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ee4da-118">Application</span></span> | <span data-ttu-id="ee4da-119">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee4da-119">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="ee4da-120">グループの場合:</span><span class="sxs-lookup"><span data-stu-id="ee4da-120">For groups:</span></span>

|<span data-ttu-id="ee4da-121">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ee4da-121">Permission type</span></span>      | <span data-ttu-id="ee4da-122">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ee4da-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee4da-123">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ee4da-123">Delegated (work or school account)</span></span> | <span data-ttu-id="ee4da-124">Group.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ee4da-124">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="ee4da-125">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ee4da-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee4da-126">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee4da-126">Not supported.</span></span>    |
|<span data-ttu-id="ee4da-127">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ee4da-127">Application</span></span> | <span data-ttu-id="ee4da-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee4da-128">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee4da-129">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ee4da-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deletedItems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ee4da-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee4da-130">Request headers</span></span>
| <span data-ttu-id="ee4da-131">名前</span><span class="sxs-lookup"><span data-stu-id="ee4da-131">Name</span></span>       | <span data-ttu-id="ee4da-132">説明</span><span class="sxs-lookup"><span data-stu-id="ee4da-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ee4da-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee4da-133">Authorization</span></span>  | <span data-ttu-id="ee4da-134">ベアラー &lt;コード&gt; が*必要*</span><span class="sxs-lookup"><span data-stu-id="ee4da-134">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="ee4da-135">承諾</span><span class="sxs-lookup"><span data-stu-id="ee4da-135">Accept</span></span>  | <span data-ttu-id="ee4da-136">application/json</span><span class="sxs-lookup"><span data-stu-id="ee4da-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee4da-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="ee4da-137">Request body</span></span>
<span data-ttu-id="ee4da-138">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ee4da-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee4da-139">応答</span><span class="sxs-lookup"><span data-stu-id="ee4da-139">Response</span></span>

<span data-ttu-id="ee4da-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ee4da-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee4da-142">例</span><span class="sxs-lookup"><span data-stu-id="ee4da-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ee4da-143">要求</span><span class="sxs-lookup"><span data-stu-id="ee4da-143">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ee4da-144">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ee4da-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ee4da-145">C#</span><span class="sxs-lookup"><span data-stu-id="ee4da-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ee4da-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="ee4da-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ee4da-147">目的-C</span><span class="sxs-lookup"><span data-stu-id="ee4da-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ee4da-148">Java</span><span class="sxs-lookup"><span data-stu-id="ee4da-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ee4da-149">応答</span><span class="sxs-lookup"><span data-stu-id="ee4da-149">Response</span></span>
<span data-ttu-id="ee4da-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ee4da-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
