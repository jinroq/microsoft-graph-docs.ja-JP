---
title: アイテムを完全に削除する
description: '[削除済みアイテム] からアイテムを完全に削除します。'
ms.openlocfilehash: 1665c72f3ff2e9f4105ab12a2c771e428d116c59
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066358"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="f54cc-103">アイテムを完全に削除する</span><span class="sxs-lookup"><span data-stu-id="f54cc-103">Permanently delete item</span></span>

> <span data-ttu-id="f54cc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f54cc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f54cc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f54cc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f54cc-106">[[削除済みアイテム]](../resources/directory.md) からアイテムを完全に削除します。</span><span class="sxs-lookup"><span data-stu-id="f54cc-106">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="f54cc-107">現在、[削除済みアイテム] 機能は [group](../resources/group.md) および [user](../resources/user.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f54cc-107">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="f54cc-108">[削除済みアイテム] から、アイテムを完全に削除できます。</span><span class="sxs-lookup"><span data-stu-id="f54cc-108">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="f54cc-109">ただし、アイテムを完全に削除すると、そのアイテムを復元することが**不可能**になります。</span><span class="sxs-lookup"><span data-stu-id="f54cc-109">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="f54cc-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f54cc-110">Permissions</span></span>
<span data-ttu-id="f54cc-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f54cc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="f54cc-113">ユーザー: User.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f54cc-113">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="f54cc-114">グループ: Group.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f54cc-114">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="f54cc-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f54cc-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deleteditems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f54cc-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f54cc-116">Request headers</span></span>
| <span data-ttu-id="f54cc-117">名前</span><span class="sxs-lookup"><span data-stu-id="f54cc-117">Name</span></span>       | <span data-ttu-id="f54cc-118">説明</span><span class="sxs-lookup"><span data-stu-id="f54cc-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f54cc-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f54cc-119">Authorization</span></span>  | <span data-ttu-id="f54cc-120">ベアラー &lt;コード&gt; が*必要*</span><span class="sxs-lookup"><span data-stu-id="f54cc-120">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="f54cc-121">Accept</span><span class="sxs-lookup"><span data-stu-id="f54cc-121">Accept</span></span>  | <span data-ttu-id="f54cc-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f54cc-122">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f54cc-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="f54cc-123">Request body</span></span>
<span data-ttu-id="f54cc-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f54cc-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f54cc-125">応答</span><span class="sxs-lookup"><span data-stu-id="f54cc-125">Response</span></span>

<span data-ttu-id="f54cc-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="f54cc-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f54cc-128">例</span><span class="sxs-lookup"><span data-stu-id="f54cc-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f54cc-129">要求</span><span class="sxs-lookup"><span data-stu-id="f54cc-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
##### <a name="response"></a><span data-ttu-id="f54cc-130">応答</span><span class="sxs-lookup"><span data-stu-id="f54cc-130">Response</span></span>
<span data-ttu-id="f54cc-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f54cc-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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