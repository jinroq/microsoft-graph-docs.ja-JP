---
title: 削除済みアイテムを復元する
description: '[削除済みアイテム] から、最近削除されたアイテムを復元します。 '
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 06f58e436d0e4b2225013cda90c45d51a7da23cb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555123"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="74f80-103">削除済みアイテムを復元する</span><span class="sxs-lookup"><span data-stu-id="74f80-103">Restore deleted item</span></span>

<span data-ttu-id="74f80-104">[[削除済みアイテム]](../resources/directory.md) から、最近削除されたアイテムを復元します。</span><span class="sxs-lookup"><span data-stu-id="74f80-104">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="74f80-105">現在、[削除済みアイテム] 機能は [group](../resources/group.md) および [user](../resources/user.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="74f80-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="74f80-106">アイテムを誤って削除してしまった場合、そのアイテムを完全に復元できます。</span><span class="sxs-lookup"><span data-stu-id="74f80-106">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="74f80-107">最近削除されたアイテムは、最大 30 日間、使用可能な状態に維持されます。</span><span class="sxs-lookup"><span data-stu-id="74f80-107">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="74f80-108">30 日が経過すると、アイテムは完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="74f80-108">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="74f80-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="74f80-109">Permissions</span></span>
<span data-ttu-id="74f80-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="74f80-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="74f80-112">ユーザーの場合:</span><span class="sxs-lookup"><span data-stu-id="74f80-112">For users:</span></span>

|<span data-ttu-id="74f80-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="74f80-113">Permission type</span></span>      | <span data-ttu-id="74f80-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="74f80-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74f80-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="74f80-115">Delegated (work or school account)</span></span> | <span data-ttu-id="74f80-116">User.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="74f80-116">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="74f80-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="74f80-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74f80-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74f80-118">Not supported.</span></span> |
|<span data-ttu-id="74f80-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="74f80-119">Application</span></span> | <span data-ttu-id="74f80-120">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74f80-120">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="74f80-121">グループの場合:</span><span class="sxs-lookup"><span data-stu-id="74f80-121">For groups:</span></span>

|<span data-ttu-id="74f80-122">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="74f80-122">Permission type</span></span>      | <span data-ttu-id="74f80-123">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="74f80-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74f80-124">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="74f80-124">Delegated (work or school account)</span></span> | <span data-ttu-id="74f80-125">Group.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="74f80-125">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="74f80-126">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="74f80-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74f80-127">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74f80-127">Not supported.</span></span>    |
|<span data-ttu-id="74f80-128">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="74f80-128">Application</span></span> | <span data-ttu-id="74f80-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74f80-129">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="74f80-130">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="74f80-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deletedItems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="74f80-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="74f80-131">Request headers</span></span>
| <span data-ttu-id="74f80-132">名前</span><span class="sxs-lookup"><span data-stu-id="74f80-132">Name</span></span>       | <span data-ttu-id="74f80-133">説明</span><span class="sxs-lookup"><span data-stu-id="74f80-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="74f80-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="74f80-134">Authorization</span></span>  | <span data-ttu-id="74f80-135">ベアラー &lt;コード&gt; が*必要*</span><span class="sxs-lookup"><span data-stu-id="74f80-135">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="74f80-136">承諾</span><span class="sxs-lookup"><span data-stu-id="74f80-136">Accept</span></span> | <span data-ttu-id="74f80-137">application/json</span><span class="sxs-lookup"><span data-stu-id="74f80-137">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="74f80-138">要求本文</span><span class="sxs-lookup"><span data-stu-id="74f80-138">Request body</span></span>
<span data-ttu-id="74f80-139">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="74f80-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74f80-140">応答</span><span class="sxs-lookup"><span data-stu-id="74f80-140">Response</span></span>

<span data-ttu-id="74f80-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="74f80-141">If successful, this method returns `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74f80-142">例</span><span class="sxs-lookup"><span data-stu-id="74f80-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="74f80-143">要求</span><span class="sxs-lookup"><span data-stu-id="74f80-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}/restore
```
<span data-ttu-id="74f80-144">要求本文に、[directoryObject](../resources/directoryobject.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="74f80-144">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="74f80-145">応答</span><span class="sxs-lookup"><span data-stu-id="74f80-145">Response</span></span>
<span data-ttu-id="74f80-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="74f80-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
