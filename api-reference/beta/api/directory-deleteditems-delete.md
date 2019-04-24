---
title: アイテムを完全に削除する
description: '[削除済みアイテム] からアイテムを完全に削除します。'
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 048008e31bc5cd7884dd3d7e9259412070404d9d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455127"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="b6254-103">アイテムを完全に削除する</span><span class="sxs-lookup"><span data-stu-id="b6254-103">Permanently delete item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6254-104">[[削除済みアイテム]](../resources/directory.md) からアイテムを完全に削除します。</span><span class="sxs-lookup"><span data-stu-id="b6254-104">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="b6254-105">現在、[削除済みアイテム] 機能は [group](../resources/group.md) および [user](../resources/user.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b6254-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="b6254-106">[削除済みアイテム] から、アイテムを完全に削除できます。</span><span class="sxs-lookup"><span data-stu-id="b6254-106">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="b6254-107">ただし、アイテムを完全に削除すると、そのアイテムを復元することが**不可能**になります。</span><span class="sxs-lookup"><span data-stu-id="b6254-107">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6254-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b6254-108">Permissions</span></span>
<span data-ttu-id="b6254-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b6254-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="b6254-111">ユーザーの場合: directory.accessasuser.all、すべてのユーザー</span><span class="sxs-lookup"><span data-stu-id="b6254-111">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="b6254-112">グループの場合: directory.accessasuser.all、all、および all</span><span class="sxs-lookup"><span data-stu-id="b6254-112">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="b6254-113">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b6254-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deleteditems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b6254-114">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b6254-114">Request headers</span></span>
| <span data-ttu-id="b6254-115">名前</span><span class="sxs-lookup"><span data-stu-id="b6254-115">Name</span></span>       | <span data-ttu-id="b6254-116">説明</span><span class="sxs-lookup"><span data-stu-id="b6254-116">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b6254-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6254-117">Authorization</span></span>  | <span data-ttu-id="b6254-118">ベアラー &lt;コード&gt; が*必要*</span><span class="sxs-lookup"><span data-stu-id="b6254-118">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="b6254-119">承諾</span><span class="sxs-lookup"><span data-stu-id="b6254-119">Accept</span></span>  | <span data-ttu-id="b6254-120">application/json</span><span class="sxs-lookup"><span data-stu-id="b6254-120">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6254-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="b6254-121">Request body</span></span>
<span data-ttu-id="b6254-122">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b6254-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6254-123">応答</span><span class="sxs-lookup"><span data-stu-id="b6254-123">Response</span></span>

<span data-ttu-id="b6254-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="b6254-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6254-126">例</span><span class="sxs-lookup"><span data-stu-id="b6254-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b6254-127">要求</span><span class="sxs-lookup"><span data-stu-id="b6254-127">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
##### <a name="response"></a><span data-ttu-id="b6254-128">応答</span><span class="sxs-lookup"><span data-stu-id="b6254-128">Response</span></span>
<span data-ttu-id="b6254-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b6254-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/directory-deleteditems-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
