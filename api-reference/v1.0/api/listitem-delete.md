---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: SharePoint リストからエントリを削除する
localization_priority: Normal
ms.prod: sharepoint
description: リストからアイテムを削除します。
doc_type: apiPageType
ms.openlocfilehash: ac07e03892476ad160f76dd49ced3b2bcb63ace6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374023"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="b1dcc-103">リストからアイテムを削除する</span><span class="sxs-lookup"><span data-stu-id="b1dcc-103">Delete an item from a list</span></span>

<span data-ttu-id="b1dcc-104">[list][] からアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="b1dcc-104">Removes an item from a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="b1dcc-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b1dcc-106">Permissions</span></span>

<span data-ttu-id="b1dcc-107">アイテムを削除するには、削除するアイテムへの書き込みアクセス権がユーザーに付与されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b1dcc-107">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="b1dcc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b1dcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1dcc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b1dcc-110">Permission type</span></span>      | <span data-ttu-id="b1dcc-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b1dcc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1dcc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b1dcc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b1dcc-113">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1dcc-113">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b1dcc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b1dcc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1dcc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1dcc-115">Not supported.</span></span>    |
|<span data-ttu-id="b1dcc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b1dcc-116">Application</span></span> | <span data-ttu-id="b1dcc-117">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1dcc-117">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1dcc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b1dcc-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="b1dcc-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b1dcc-119">Optional request headers</span></span>

| <span data-ttu-id="b1dcc-120">名前</span><span class="sxs-lookup"><span data-stu-id="b1dcc-120">Name</span></span>       | <span data-ttu-id="b1dcc-121">値</span><span class="sxs-lookup"><span data-stu-id="b1dcc-121">Value</span></span> | <span data-ttu-id="b1dcc-122">説明</span><span class="sxs-lookup"><span data-stu-id="b1dcc-122">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="b1dcc-123">_if-match_</span><span class="sxs-lookup"><span data-stu-id="b1dcc-123">_if-match_</span></span> | <span data-ttu-id="b1dcc-124">etag</span><span class="sxs-lookup"><span data-stu-id="b1dcc-124">etag</span></span>  | <span data-ttu-id="b1dcc-125">この要求ヘッダーが含まれていて、指定された eTag がアイテムの現在のタグに一致しない場合には、`412 Precondition Failed` 応答が返され、アイテムは削除されません。</span><span class="sxs-lookup"><span data-stu-id="b1dcc-125">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="b1dcc-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b1dcc-126">Request body</span></span>

<span data-ttu-id="b1dcc-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b1dcc-127">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="b1dcc-128">例</span><span class="sxs-lookup"><span data-stu-id="b1dcc-128">Example</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b1dcc-129">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b1dcc-129">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-item-site", "scopes": "files.readwrite sites.readwrite.all" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b1dcc-130">C#</span><span class="sxs-lookup"><span data-stu-id="b1dcc-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-item-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b1dcc-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1dcc-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-item-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b1dcc-132">目的-C</span><span class="sxs-lookup"><span data-stu-id="b1dcc-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-item-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b1dcc-133">Java</span><span class="sxs-lookup"><span data-stu-id="b1dcc-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-item-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="b1dcc-134">応答</span><span class="sxs-lookup"><span data-stu-id="b1dcc-134">Response</span></span>

<span data-ttu-id="b1dcc-135">成功した場合、この呼び出しはリソースが削除され返すものがなかったことを示す `204 No Content` 応答を返します。</span><span class="sxs-lookup"><span data-stu-id="b1dcc-135">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Delete",
  "suppressions": [
  ]
} -->
