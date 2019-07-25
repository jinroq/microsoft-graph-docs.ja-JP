---
title: グループ設定の削除
description: グループ設定を削除します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5cb7a47e7ee376a33f8bb4cbbe2c577b05d3f063
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886803"
---
# <a name="delete-a-group-setting"></a><span data-ttu-id="d6ddc-103">グループ設定の削除</span><span class="sxs-lookup"><span data-stu-id="d6ddc-103">Delete a group setting</span></span>

<span data-ttu-id="d6ddc-104">グループ設定を削除します。</span><span class="sxs-lookup"><span data-stu-id="d6ddc-104">Delete a group setting.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6ddc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d6ddc-105">Permissions</span></span>

<span data-ttu-id="d6ddc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d6ddc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d6ddc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d6ddc-108">Permission type</span></span>      | <span data-ttu-id="d6ddc-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d6ddc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6ddc-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d6ddc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d6ddc-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d6ddc-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d6ddc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d6ddc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6ddc-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6ddc-113">Not supported.</span></span>    |
|<span data-ttu-id="d6ddc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d6ddc-114">Application</span></span> | <span data-ttu-id="d6ddc-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6ddc-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6ddc-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d6ddc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupSettings/{id}
DELETE /groups/{id}/settings/{id}

```

## <a name="request-headers"></a><span data-ttu-id="d6ddc-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d6ddc-117">Request headers</span></span>

| <span data-ttu-id="d6ddc-118">名前</span><span class="sxs-lookup"><span data-stu-id="d6ddc-118">Name</span></span> | <span data-ttu-id="d6ddc-119">説明</span><span class="sxs-lookup"><span data-stu-id="d6ddc-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="d6ddc-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6ddc-120">Authorization</span></span>  | <span data-ttu-id="d6ddc-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d6ddc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d6ddc-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d6ddc-123">Content-Type</span></span>  | <span data-ttu-id="d6ddc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d6ddc-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6ddc-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d6ddc-125">Request body</span></span>
<span data-ttu-id="d6ddc-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d6ddc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6ddc-127">応答</span><span class="sxs-lookup"><span data-stu-id="d6ddc-127">Response</span></span>

<span data-ttu-id="d6ddc-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="d6ddc-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6ddc-130">例</span><span class="sxs-lookup"><span data-stu-id="d6ddc-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d6ddc-131">要求</span><span class="sxs-lookup"><span data-stu-id="d6ddc-131">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d6ddc-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="d6ddc-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_groupsetting"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupSettings/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d6ddc-133">C#</span><span class="sxs-lookup"><span data-stu-id="d6ddc-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d6ddc-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="d6ddc-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d6ddc-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="d6ddc-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d6ddc-136">Java</span><span class="sxs-lookup"><span data-stu-id="d6ddc-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-groupsetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d6ddc-137">応答</span><span class="sxs-lookup"><span data-stu-id="d6ddc-137">Response</span></span>
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
  "description": "Delete groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
