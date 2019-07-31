---
title: メンバーを削除する
description: この API を使用して、**members** ナビゲーション プロパティを通じて Office 365 のグループ、セキュリティ グループ、メールが有効なセキュリティ グループからメンバーを削除できます。ユーザーや他のグループを削除できます。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b73ed8d1fc599a3c65b9b08e3caffcfc272bb332
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954054"
---
# <a name="remove-member"></a><span data-ttu-id="ff527-104">メンバーを削除する</span><span class="sxs-lookup"><span data-stu-id="ff527-104">Remove member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff527-105">この API を使用して、 **members**ナビゲーションプロパティを使用してグループからメンバーを削除します。</span><span class="sxs-lookup"><span data-stu-id="ff527-105">Use this API to remove a member from a group via the **members** navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff527-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ff527-106">Permissions</span></span>
<span data-ttu-id="ff527-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff527-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff527-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ff527-109">Permission type</span></span>      | <span data-ttu-id="ff527-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ff527-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff527-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ff527-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ff527-112">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ff527-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="ff527-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ff527-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff527-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff527-114">Not supported.</span></span> |
|<span data-ttu-id="ff527-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ff527-115">Application</span></span> | <span data-ttu-id="ff527-116">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff527-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff527-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ff527-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="ff527-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff527-118">Request headers</span></span>
| <span data-ttu-id="ff527-119">名前</span><span class="sxs-lookup"><span data-stu-id="ff527-119">Name</span></span>       | <span data-ttu-id="ff527-120">型</span><span class="sxs-lookup"><span data-stu-id="ff527-120">Type</span></span> | <span data-ttu-id="ff527-121">説明</span><span class="sxs-lookup"><span data-stu-id="ff527-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ff527-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff527-122">Authorization</span></span>  | <span data-ttu-id="ff527-123">string</span><span class="sxs-lookup"><span data-stu-id="ff527-123">string</span></span>  | <span data-ttu-id="ff527-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ff527-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff527-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ff527-126">Request body</span></span>
<span data-ttu-id="ff527-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ff527-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff527-128">応答</span><span class="sxs-lookup"><span data-stu-id="ff527-128">Response</span></span>
<span data-ttu-id="ff527-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ff527-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff527-131">例</span><span class="sxs-lookup"><span data-stu-id="ff527-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ff527-132">要求</span><span class="sxs-lookup"><span data-stu-id="ff527-132">Request</span></span>
<span data-ttu-id="ff527-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ff527-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ff527-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ff527-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_member_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/members/{id}/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ff527-135">C#</span><span class="sxs-lookup"><span data-stu-id="ff527-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ff527-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="ff527-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ff527-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="ff527-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ff527-138">Java</span><span class="sxs-lookup"><span data-stu-id="ff527-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-member-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="ff527-139">要求内で、$ref セグメント後に削除したいディレクトリ オブジェクトの `id` を指定します。</span><span class="sxs-lookup"><span data-stu-id="ff527-139">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="ff527-140">応答</span><span class="sxs-lookup"><span data-stu-id="ff527-140">Response</span></span>
<span data-ttu-id="ff527-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ff527-141">The following is an example of the response.</span></span>
><span data-ttu-id="ff527-142">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="ff527-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ff527-143">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ff527-143">All the properties will be returned from an actual call.</span></span>
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
