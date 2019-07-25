---
title: メンバーを追加する
description: '**members** ナビゲーション プロパティを通じて Office 365 のグループ、セキュリティ グループ、メールが有効なセキュリティ グループにメンバーを追加できます。'
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 71a2eba3523898621231f29be775ba03ae45c517
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890088"
---
# <a name="add-member"></a><span data-ttu-id="2a847-103">メンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="2a847-103">Add member</span></span>
<span data-ttu-id="2a847-104">**members** ナビゲーション プロパティを通じて Office 365 のグループ、またはセキュリティ グループにメンバーを追加できます。</span><span class="sxs-lookup"><span data-stu-id="2a847-104">Use this API to add a member to an Office 365 Group, a security group, or a mail-enabled security group through the **members** navigation property.</span></span>

<span data-ttu-id="2a847-105">ユーザーや他のグループを追加できます。</span><span class="sxs-lookup"><span data-stu-id="2a847-105">You can add users or other groups.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="2a847-106">Office 365 のグループには、ユーザーのみを追加できます。</span><span class="sxs-lookup"><span data-stu-id="2a847-106">Important: You can add only users to Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a847-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2a847-107">Permissions</span></span>
<span data-ttu-id="2a847-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2a847-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a847-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2a847-110">Permission type</span></span>      | <span data-ttu-id="2a847-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2a847-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a847-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2a847-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2a847-113">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2a847-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2a847-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2a847-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a847-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2a847-115">Not supported.</span></span>    |
|<span data-ttu-id="2a847-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2a847-116">Application</span></span> | <span data-ttu-id="2a847-117">Group.ReadWrite.All および Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a847-117">Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a847-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2a847-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="2a847-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2a847-119">Request headers</span></span>
| <span data-ttu-id="2a847-120">名前</span><span class="sxs-lookup"><span data-stu-id="2a847-120">Name</span></span>       | <span data-ttu-id="2a847-121">型</span><span class="sxs-lookup"><span data-stu-id="2a847-121">Type</span></span> | <span data-ttu-id="2a847-122">説明</span><span class="sxs-lookup"><span data-stu-id="2a847-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2a847-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a847-123">Authorization</span></span>  | <span data-ttu-id="2a847-124">string</span><span class="sxs-lookup"><span data-stu-id="2a847-124">string</span></span>  | <span data-ttu-id="2a847-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2a847-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a847-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="2a847-127">Request body</span></span>
<span data-ttu-id="2a847-128">要求本文で、追加する [directoryObject](../resources/directoryobject.md)、[ユーザー](../resources/user.md) または [グループ](../resources/group.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2a847-128">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="2a847-129">応答</span><span class="sxs-lookup"><span data-stu-id="2a847-129">Response</span></span>
<span data-ttu-id="2a847-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="2a847-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a847-132">例</span><span class="sxs-lookup"><span data-stu-id="2a847-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2a847-133">要求</span><span class="sxs-lookup"><span data-stu-id="2a847-133">Request</span></span>
<span data-ttu-id="2a847-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2a847-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2a847-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a847-135">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_member_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2a847-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="2a847-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2a847-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a847-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="2a847-138">C#</span><span class="sxs-lookup"><span data-stu-id="2a847-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2a847-139">Java</span><span class="sxs-lookup"><span data-stu-id="2a847-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-member-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="2a847-140">要求本文で、追加する [directoryObject](../resources/directoryobject.md)、[ユーザー](../resources/user.md) または [グループ](../resources/group.md) オブジェクトの `id` の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2a847-140">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="2a847-141">応答</span><span class="sxs-lookup"><span data-stu-id="2a847-141">Response</span></span>
<span data-ttu-id="2a847-142">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2a847-142">The following is an example of the response.</span></span>
><span data-ttu-id="2a847-143">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="2a847-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2a847-144">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2a847-144">All the properties will be returned from an actual call.</span></span>
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
