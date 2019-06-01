---
title: 削除済みアイテムを復元する
description: '[削除済みアイテム] から、最近削除されたアイテムを復元します。 '
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a0f38d24e3ba0f11ba12c59e19f933e8f7983fab
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34656735"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="f1ae8-103">削除済みアイテムを復元する</span><span class="sxs-lookup"><span data-stu-id="f1ae8-103">Restore deleted item</span></span>

<span data-ttu-id="f1ae8-104">[[削除済みアイテム]](../resources/directory.md) から、最近削除されたアイテムを復元します。</span><span class="sxs-lookup"><span data-stu-id="f1ae8-104">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="f1ae8-105">現在、[削除済みアイテム] 機能は [group](../resources/group.md) および [user](../resources/user.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f1ae8-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="f1ae8-106">アイテムを誤って削除してしまった場合、そのアイテムを完全に復元できます。</span><span class="sxs-lookup"><span data-stu-id="f1ae8-106">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="f1ae8-107">最近削除されたアイテムは、最大 30 日間、使用可能な状態に維持されます。</span><span class="sxs-lookup"><span data-stu-id="f1ae8-107">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="f1ae8-108">30 日が経過すると、アイテムは完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="f1ae8-108">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1ae8-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f1ae8-109">Permissions</span></span>
<span data-ttu-id="f1ae8-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f1ae8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="f1ae8-112">ユーザーの場合:</span><span class="sxs-lookup"><span data-stu-id="f1ae8-112">For users:</span></span>

|<span data-ttu-id="f1ae8-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f1ae8-113">Permission type</span></span>      | <span data-ttu-id="f1ae8-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f1ae8-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1ae8-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f1ae8-115">Delegated (work or school account)</span></span> | <span data-ttu-id="f1ae8-116">User.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f1ae8-116">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="f1ae8-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f1ae8-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1ae8-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1ae8-118">Not supported.</span></span> |
|<span data-ttu-id="f1ae8-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f1ae8-119">Application</span></span> | <span data-ttu-id="f1ae8-120">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1ae8-120">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="f1ae8-121">グループの場合:</span><span class="sxs-lookup"><span data-stu-id="f1ae8-121">For groups:</span></span>

|<span data-ttu-id="f1ae8-122">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f1ae8-122">Permission type</span></span>      | <span data-ttu-id="f1ae8-123">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f1ae8-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1ae8-124">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f1ae8-124">Delegated (work or school account)</span></span> | <span data-ttu-id="f1ae8-125">Group.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f1ae8-125">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="f1ae8-126">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f1ae8-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1ae8-127">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1ae8-127">Not supported.</span></span>    |
|<span data-ttu-id="f1ae8-128">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f1ae8-128">Application</span></span> | <span data-ttu-id="f1ae8-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1ae8-129">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1ae8-130">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f1ae8-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deletedItems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="f1ae8-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f1ae8-131">Request headers</span></span>
| <span data-ttu-id="f1ae8-132">名前</span><span class="sxs-lookup"><span data-stu-id="f1ae8-132">Name</span></span>       | <span data-ttu-id="f1ae8-133">説明</span><span class="sxs-lookup"><span data-stu-id="f1ae8-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f1ae8-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1ae8-134">Authorization</span></span>  | <span data-ttu-id="f1ae8-135">ベアラー &lt;コード&gt; が*必要*</span><span class="sxs-lookup"><span data-stu-id="f1ae8-135">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="f1ae8-136">承諾</span><span class="sxs-lookup"><span data-stu-id="f1ae8-136">Accept</span></span> | <span data-ttu-id="f1ae8-137">application/json</span><span class="sxs-lookup"><span data-stu-id="f1ae8-137">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1ae8-138">要求本文</span><span class="sxs-lookup"><span data-stu-id="f1ae8-138">Request body</span></span>
<span data-ttu-id="f1ae8-139">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f1ae8-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1ae8-140">応答</span><span class="sxs-lookup"><span data-stu-id="f1ae8-140">Response</span></span>

<span data-ttu-id="f1ae8-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f1ae8-141">If successful, this method returns `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1ae8-142">例</span><span class="sxs-lookup"><span data-stu-id="f1ae8-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1ae8-143">要求</span><span class="sxs-lookup"><span data-stu-id="f1ae8-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}/restore
```
<span data-ttu-id="f1ae8-144">要求本文に、[directoryObject](../resources/directoryobject.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f1ae8-144">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f1ae8-145">応答</span><span class="sxs-lookup"><span data-stu-id="f1ae8-145">Response</span></span>
<span data-ttu-id="f1ae8-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f1ae8-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f1ae8-148">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="f1ae8-148">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f1ae8-149">C#</span><span class="sxs-lookup"><span data-stu-id="f1ae8-149">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_directory-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f1ae8-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="f1ae8-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_directory-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create deletedItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/directory-deleteditems-restore.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/directory-deleteditems-restore.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
