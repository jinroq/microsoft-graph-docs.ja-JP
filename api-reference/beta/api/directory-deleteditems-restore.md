---
title: 削除済みアイテムを復元する
description: '[削除済みアイテム] から、最近削除されたアイテムを復元します。 '
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8c9a6e84a723fc0087f3155e4b2e973e72276233
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935970"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="4b880-103">削除済みアイテムを復元する</span><span class="sxs-lookup"><span data-stu-id="4b880-103">Restore deleted item</span></span>

> <span data-ttu-id="4b880-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4b880-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b880-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b880-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4b880-106">[[削除済みアイテム]](../resources/directory.md) から、最近削除されたアイテムを復元します。</span><span class="sxs-lookup"><span data-stu-id="4b880-106">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="4b880-107">現在、[削除済みアイテム] 機能は [group](../resources/group.md) および [user](../resources/user.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="4b880-107">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="4b880-108">アイテムを誤って削除してしまった場合、そのアイテムを完全に復元できます。</span><span class="sxs-lookup"><span data-stu-id="4b880-108">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="4b880-109">最近削除されたアイテムは、最大 30 日間、使用可能な状態に維持されます。</span><span class="sxs-lookup"><span data-stu-id="4b880-109">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="4b880-110">30 日が経過すると、アイテムは完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="4b880-110">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b880-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4b880-111">Permissions</span></span>
<span data-ttu-id="4b880-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4b880-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="4b880-114">ユーザー: User.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4b880-114">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="4b880-115">グループ: Group.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4b880-115">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="4b880-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4b880-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deleteditems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="4b880-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4b880-117">Request headers</span></span>
| <span data-ttu-id="4b880-118">名前</span><span class="sxs-lookup"><span data-stu-id="4b880-118">Name</span></span>       | <span data-ttu-id="4b880-119">説明</span><span class="sxs-lookup"><span data-stu-id="4b880-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4b880-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b880-120">Authorization</span></span>  | <span data-ttu-id="4b880-121">ベアラー &lt;コード&gt; が*必要*</span><span class="sxs-lookup"><span data-stu-id="4b880-121">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="4b880-122">Accept</span><span class="sxs-lookup"><span data-stu-id="4b880-122">Accept</span></span> | <span data-ttu-id="4b880-123">application/json</span><span class="sxs-lookup"><span data-stu-id="4b880-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b880-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="4b880-124">Request body</span></span>
<span data-ttu-id="4b880-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4b880-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b880-126">応答</span><span class="sxs-lookup"><span data-stu-id="4b880-126">Response</span></span>

<span data-ttu-id="4b880-127">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4b880-127">If successful, this method returns `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b880-128">例</span><span class="sxs-lookup"><span data-stu-id="4b880-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4b880-129">要求</span><span class="sxs-lookup"><span data-stu-id="4b880-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb/restore
```
<span data-ttu-id="4b880-130">要求本文に、[directoryObject](../resources/directoryobject.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4b880-130">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4b880-131">応答</span><span class="sxs-lookup"><span data-stu-id="4b880-131">Response</span></span>
<span data-ttu-id="4b880-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4b880-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create deletedItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
