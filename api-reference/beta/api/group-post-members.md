---
title: メンバーを追加する
description: '**Members**ナビゲーションプロパティを使用して、Office 365 グループまたはセキュリティグループにメンバーを追加します。'
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 64ddd8881cb210a06fff35f0d30d1e3a78c85d81
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323249"
---
# <a name="add-member"></a><span data-ttu-id="b30d1-103">メンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="b30d1-103">Add member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b30d1-104">**Members**ナビゲーションプロパティを使用して、Office 365 グループまたはセキュリティグループにメンバーを追加します。</span><span class="sxs-lookup"><span data-stu-id="b30d1-104">Add a member to an Office 365 group or security group through the **members** navigation property.</span></span>

<span data-ttu-id="b30d1-105">ユーザーや他のグループを追加できます。</span><span class="sxs-lookup"><span data-stu-id="b30d1-105">You can add users or other groups.</span></span> 

> [!Important]
> <span data-ttu-id="b30d1-106">Office 365 グループにユーザーのみを追加できます。</span><span class="sxs-lookup"><span data-stu-id="b30d1-106">You can add only users to Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="b30d1-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b30d1-107">Permissions</span></span>
<span data-ttu-id="b30d1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b30d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b30d1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b30d1-110">Permission type</span></span>      | <span data-ttu-id="b30d1-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b30d1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b30d1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b30d1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b30d1-113">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b30d1-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b30d1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b30d1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b30d1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b30d1-115">Not supported.</span></span>    |
|<span data-ttu-id="b30d1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b30d1-116">Application</span></span> | <span data-ttu-id="b30d1-117">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b30d1-117">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b30d1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b30d1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="b30d1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b30d1-119">Request headers</span></span>
| <span data-ttu-id="b30d1-120">名前</span><span class="sxs-lookup"><span data-stu-id="b30d1-120">Name</span></span> | <span data-ttu-id="b30d1-121">説明</span><span class="sxs-lookup"><span data-stu-id="b30d1-121">Description</span></span>|
|:---- |:-----------|
| <span data-ttu-id="b30d1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b30d1-122">Authorization</span></span> | <span data-ttu-id="b30d1-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b30d1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b30d1-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b30d1-125">Request body</span></span>
<span data-ttu-id="b30d1-126">要求本文で、追加する [directoryObject](../resources/directoryobject.md)、[ユーザー](../resources/user.md) または [グループ](../resources/group.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b30d1-126">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="b30d1-127">応答</span><span class="sxs-lookup"><span data-stu-id="b30d1-127">Response</span></span>
<span data-ttu-id="b30d1-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="b30d1-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b30d1-130">例</span><span class="sxs-lookup"><span data-stu-id="b30d1-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="b30d1-131">要求</span><span class="sxs-lookup"><span data-stu-id="b30d1-131">Request</span></span>
<span data-ttu-id="b30d1-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b30d1-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b30d1-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b30d1-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_group_member"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b30d1-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b30d1-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-group-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b30d1-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="b30d1-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-group-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="b30d1-136">C#</span><span class="sxs-lookup"><span data-stu-id="b30d1-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-group-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b30d1-137">Java</span><span class="sxs-lookup"><span data-stu-id="b30d1-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-group-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="b30d1-138">要求本文で、追加する[Directoryobject](../resources/directoryobject.md)、 [user](../resources/user.md)、 `id`または[group](../resources/group.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b30d1-138">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [group](../resources/group.md) object you want to add.</span></span>

### <a name="response"></a><span data-ttu-id="b30d1-139">応答</span><span class="sxs-lookup"><span data-stu-id="b30d1-139">Response</span></span>
<span data-ttu-id="b30d1-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b30d1-140">The following is an example of the response.</span></span>
><span data-ttu-id="b30d1-141">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="b30d1-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b30d1-142">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b30d1-142">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
