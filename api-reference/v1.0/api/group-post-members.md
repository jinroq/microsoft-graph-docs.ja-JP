---
title: メンバーを追加する
description: この API を使用して、**members** ナビゲーション プロパティを通じて Office 365 のグループ、セキュリティ グループ、メールが有効なセキュリティ グループにメンバーを追加できます。
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 9a819ee95010a6702aabf55c92f0106716fdd80d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35456394"
---
# <a name="add-member"></a><span data-ttu-id="55b84-103">メンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="55b84-103">Add member</span></span>
<span data-ttu-id="55b84-104">この API を使用して、**members** ナビゲーション プロパティを通じて Office 365 のグループ、セキュリティ グループ、メールが有効なセキュリティ グループにメンバーを追加できます。</span><span class="sxs-lookup"><span data-stu-id="55b84-104">Use this API to add a member to an Office 365 Group, a security group, or a mail-enabled security group through the **members** navigation property.</span></span>

<span data-ttu-id="55b84-105">ユーザーや他のグループを追加できます。</span><span class="sxs-lookup"><span data-stu-id="55b84-105">You can add users or other groups.</span></span> <span data-ttu-id="55b84-106">重要: Office 365 のグループには、ユーザーのみを追加できます。</span><span class="sxs-lookup"><span data-stu-id="55b84-106">Important: You can add only users to Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="55b84-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="55b84-107">Permissions</span></span>
<span data-ttu-id="55b84-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="55b84-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55b84-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="55b84-110">Permission type</span></span>      | <span data-ttu-id="55b84-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="55b84-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55b84-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="55b84-112">Delegated (work or school account)</span></span> | <span data-ttu-id="55b84-113">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="55b84-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="55b84-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="55b84-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55b84-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="55b84-115">Not supported.</span></span>    |
|<span data-ttu-id="55b84-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="55b84-116">Application</span></span> | <span data-ttu-id="55b84-117">Group.ReadWrite.All および Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55b84-117">Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="55b84-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="55b84-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="55b84-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="55b84-119">Request headers</span></span>
| <span data-ttu-id="55b84-120">名前</span><span class="sxs-lookup"><span data-stu-id="55b84-120">Name</span></span>       | <span data-ttu-id="55b84-121">型</span><span class="sxs-lookup"><span data-stu-id="55b84-121">Type</span></span> | <span data-ttu-id="55b84-122">説明</span><span class="sxs-lookup"><span data-stu-id="55b84-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="55b84-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="55b84-123">Authorization</span></span>  | <span data-ttu-id="55b84-124">string</span><span class="sxs-lookup"><span data-stu-id="55b84-124">string</span></span>  | <span data-ttu-id="55b84-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="55b84-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55b84-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="55b84-127">Request body</span></span>
<span data-ttu-id="55b84-128">要求本文で、追加する [directoryObject](../resources/directoryobject.md)、[ユーザー](../resources/user.md) または [グループ](../resources/group.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="55b84-128">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="55b84-129">応答</span><span class="sxs-lookup"><span data-stu-id="55b84-129">Response</span></span>
<span data-ttu-id="55b84-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="55b84-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55b84-132">例</span><span class="sxs-lookup"><span data-stu-id="55b84-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="55b84-133">要求</span><span class="sxs-lookup"><span data-stu-id="55b84-133">Request</span></span>
<span data-ttu-id="55b84-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="55b84-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="55b84-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="55b84-135">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="55b84-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="55b84-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="55b84-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55b84-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="55b84-138">要求本文で、追加する [directoryObject](../resources/directoryobject.md)、[ユーザー](../resources/user.md) または [グループ](../resources/group.md) オブジェクトの `id` の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="55b84-138">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="55b84-139">応答</span><span class="sxs-lookup"><span data-stu-id="55b84-139">Response</span></span>
<span data-ttu-id="55b84-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="55b84-140">The following is an example of the response.</span></span>
><span data-ttu-id="55b84-141">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="55b84-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="55b84-142">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="55b84-142">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
