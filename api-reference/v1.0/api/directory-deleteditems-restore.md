---
title: 削除済みアイテムを復元する
description: '[削除済みアイテム] から、最近削除されたアイテムを復元します。 '
ms.openlocfilehash: 3fa47d269cefaf54994b57f8f06a92a8ac8fc4b7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022594"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="560cc-103">削除済みアイテムを復元する</span><span class="sxs-lookup"><span data-stu-id="560cc-103">Restore deleted item</span></span>

<span data-ttu-id="560cc-104">[[削除済みアイテム]](../resources/directory.md) から、最近削除されたアイテムを復元します。</span><span class="sxs-lookup"><span data-stu-id="560cc-104">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="560cc-105">現在、[削除済みアイテム] 機能は [group](../resources/group.md) および [user](../resources/user.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="560cc-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="560cc-106">アイテムを誤って削除してしまった場合、そのアイテムを完全に復元できます。</span><span class="sxs-lookup"><span data-stu-id="560cc-106">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="560cc-107">最近削除されたアイテムは、最大 30 日間、使用可能な状態に維持されます。</span><span class="sxs-lookup"><span data-stu-id="560cc-107">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="560cc-108">30 日が経過すると、アイテムは完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="560cc-108">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="560cc-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="560cc-109">Permissions</span></span>
<span data-ttu-id="560cc-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="560cc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="560cc-112">ユーザーの場合:</span><span class="sxs-lookup"><span data-stu-id="560cc-112">For users:</span></span>

|<span data-ttu-id="560cc-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="560cc-113">Permission type</span></span>      | <span data-ttu-id="560cc-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="560cc-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="560cc-115">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="560cc-115">Delegated (work or school account)</span></span> | <span data-ttu-id="560cc-116">User.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="560cc-116">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="560cc-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="560cc-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="560cc-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="560cc-118">Not supported.</span></span> |
|<span data-ttu-id="560cc-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="560cc-119">Application</span></span> | <span data-ttu-id="560cc-120">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="560cc-120">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="560cc-121">グループの場合:</span><span class="sxs-lookup"><span data-stu-id="560cc-121">For groups:</span></span>

|<span data-ttu-id="560cc-122">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="560cc-122">Permission type</span></span>      | <span data-ttu-id="560cc-123">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="560cc-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="560cc-124">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="560cc-124">Delegated (work or school account)</span></span> | <span data-ttu-id="560cc-125">Group.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="560cc-125">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="560cc-126">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="560cc-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="560cc-127">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="560cc-127">Not supported.</span></span>    |
|<span data-ttu-id="560cc-128">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="560cc-128">Application</span></span> | <span data-ttu-id="560cc-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="560cc-129">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="560cc-130">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="560cc-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deletedItems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="560cc-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="560cc-131">Request headers</span></span>
| <span data-ttu-id="560cc-132">名前</span><span class="sxs-lookup"><span data-stu-id="560cc-132">Name</span></span>       | <span data-ttu-id="560cc-133">説明</span><span class="sxs-lookup"><span data-stu-id="560cc-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="560cc-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="560cc-134">Authorization</span></span>  | <span data-ttu-id="560cc-135">ベアラー &lt;コード&gt; が*必要*</span><span class="sxs-lookup"><span data-stu-id="560cc-135">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="560cc-136">Accept</span><span class="sxs-lookup"><span data-stu-id="560cc-136">Accept</span></span> | <span data-ttu-id="560cc-137">application/json</span><span class="sxs-lookup"><span data-stu-id="560cc-137">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="560cc-138">要求本文</span><span class="sxs-lookup"><span data-stu-id="560cc-138">Request body</span></span>
<span data-ttu-id="560cc-139">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="560cc-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="560cc-140">応答</span><span class="sxs-lookup"><span data-stu-id="560cc-140">Response</span></span>

<span data-ttu-id="560cc-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="560cc-141">If successful, this method returns `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="560cc-142">例</span><span class="sxs-lookup"><span data-stu-id="560cc-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="560cc-143">要求</span><span class="sxs-lookup"><span data-stu-id="560cc-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}/restore
```
<span data-ttu-id="560cc-144">要求本文に、[directoryObject](../resources/directoryobject.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="560cc-144">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="560cc-145">応答</span><span class="sxs-lookup"><span data-stu-id="560cc-145">Response</span></span>
<span data-ttu-id="560cc-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="560cc-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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