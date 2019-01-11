---
title: アイテムを完全に削除する
description: '[削除済みアイテム] からアイテムを完全に削除します。'
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 00f44be1c89b35b81f3665d4bd568939ed309e22
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805188"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="f0f76-103">アイテムを完全に削除する</span><span class="sxs-lookup"><span data-stu-id="f0f76-103">Permanently delete item</span></span>

<span data-ttu-id="f0f76-104">[[削除済みアイテム]](../resources/directory.md) からアイテムを完全に削除します。</span><span class="sxs-lookup"><span data-stu-id="f0f76-104">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="f0f76-105">現在、[削除済みアイテム] 機能は [group](../resources/group.md) および [user](../resources/user.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f0f76-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="f0f76-106">[削除済みアイテム] から、アイテムを完全に削除できます。</span><span class="sxs-lookup"><span data-stu-id="f0f76-106">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="f0f76-107">ただし、アイテムを完全に削除すると、そのアイテムを復元することが**不可能**になります。</span><span class="sxs-lookup"><span data-stu-id="f0f76-107">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0f76-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f0f76-108">Permissions</span></span>
<span data-ttu-id="f0f76-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f0f76-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="f0f76-111">ユーザーの場合:</span><span class="sxs-lookup"><span data-stu-id="f0f76-111">For users:</span></span>

|<span data-ttu-id="f0f76-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f0f76-112">Permission type</span></span>      | <span data-ttu-id="f0f76-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f0f76-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0f76-114">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="f0f76-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f0f76-115">User.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f0f76-115">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="f0f76-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f0f76-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0f76-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0f76-117">Not supported.</span></span> |
|<span data-ttu-id="f0f76-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f0f76-118">Application</span></span> | <span data-ttu-id="f0f76-119">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0f76-119">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="f0f76-120">グループの場合:</span><span class="sxs-lookup"><span data-stu-id="f0f76-120">For groups:</span></span>

|<span data-ttu-id="f0f76-121">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f0f76-121">Permission type</span></span>      | <span data-ttu-id="f0f76-122">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f0f76-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0f76-123">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="f0f76-123">Delegated (work or school account)</span></span> | <span data-ttu-id="f0f76-124">Group.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f0f76-124">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="f0f76-125">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f0f76-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0f76-126">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0f76-126">Not supported.</span></span>    |
|<span data-ttu-id="f0f76-127">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f0f76-127">Application</span></span> | <span data-ttu-id="f0f76-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0f76-128">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0f76-129">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f0f76-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deletedItems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f0f76-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f0f76-130">Request headers</span></span>
| <span data-ttu-id="f0f76-131">名前</span><span class="sxs-lookup"><span data-stu-id="f0f76-131">Name</span></span>       | <span data-ttu-id="f0f76-132">説明</span><span class="sxs-lookup"><span data-stu-id="f0f76-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f0f76-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0f76-133">Authorization</span></span>  | <span data-ttu-id="f0f76-134">ベアラー &lt;コード&gt; が*必要*</span><span class="sxs-lookup"><span data-stu-id="f0f76-134">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="f0f76-135">Accept</span><span class="sxs-lookup"><span data-stu-id="f0f76-135">Accept</span></span>  | <span data-ttu-id="f0f76-136">application/json</span><span class="sxs-lookup"><span data-stu-id="f0f76-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0f76-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="f0f76-137">Request body</span></span>
<span data-ttu-id="f0f76-138">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f0f76-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0f76-139">応答</span><span class="sxs-lookup"><span data-stu-id="f0f76-139">Response</span></span>

<span data-ttu-id="f0f76-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="f0f76-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0f76-142">例</span><span class="sxs-lookup"><span data-stu-id="f0f76-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f0f76-143">要求</span><span class="sxs-lookup"><span data-stu-id="f0f76-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
##### <a name="response"></a><span data-ttu-id="f0f76-144">応答</span><span class="sxs-lookup"><span data-stu-id="f0f76-144">Response</span></span>
<span data-ttu-id="f0f76-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f0f76-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
