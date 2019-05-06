---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: SharePoint リストからエントリを削除する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: bbc9d7b98cc532a8bed10da622cb49509d339d5a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33598023"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="b2752-102">リストからアイテムを削除する</span><span class="sxs-lookup"><span data-stu-id="b2752-102">Delete an item from a list</span></span>

<span data-ttu-id="b2752-103">[list][] からアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="b2752-103">Removes an item from a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="b2752-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b2752-105">Permissions</span></span>

<span data-ttu-id="b2752-106">アイテムを削除するには、削除するアイテムへの書き込みアクセス権がユーザーに付与されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b2752-106">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="b2752-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b2752-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2752-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b2752-109">Permission type</span></span>      | <span data-ttu-id="b2752-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b2752-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2752-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b2752-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b2752-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2752-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b2752-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b2752-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2752-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b2752-114">Not supported.</span></span>    |
|<span data-ttu-id="b2752-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b2752-115">Application</span></span> | <span data-ttu-id="b2752-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2752-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2752-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b2752-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="b2752-118">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b2752-118">Optional request headers</span></span>

| <span data-ttu-id="b2752-119">名前</span><span class="sxs-lookup"><span data-stu-id="b2752-119">Name</span></span>       | <span data-ttu-id="b2752-120">値</span><span class="sxs-lookup"><span data-stu-id="b2752-120">Value</span></span> | <span data-ttu-id="b2752-121">説明</span><span class="sxs-lookup"><span data-stu-id="b2752-121">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="b2752-122">_if-match_</span><span class="sxs-lookup"><span data-stu-id="b2752-122">_if-match_</span></span> | <span data-ttu-id="b2752-123">etag</span><span class="sxs-lookup"><span data-stu-id="b2752-123">etag</span></span>  | <span data-ttu-id="b2752-124">この要求ヘッダーが含まれていて、指定された eTag がアイテムの現在のタグに一致しない場合には、`412 Precondition Failed` 応答が返され、アイテムは削除されません。</span><span class="sxs-lookup"><span data-stu-id="b2752-124">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="b2752-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b2752-125">Request body</span></span>

<span data-ttu-id="b2752-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b2752-126">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="b2752-127">例</span><span class="sxs-lookup"><span data-stu-id="b2752-127">Example</span></span>

<!-- { "blockType": "request", "name": "delete-item-site", "scopes": "files.readwrite sites.readwrite.all" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="b2752-128">応答</span><span class="sxs-lookup"><span data-stu-id="b2752-128">Response</span></span>

<span data-ttu-id="b2752-129">成功した場合、この呼び出しはリソースが削除され返すものがなかったことを示す `204 No Content` 応答を返します。</span><span class="sxs-lookup"><span data-stu-id="b2752-129">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b2752-130">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="b2752-130">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b2752-131">Visual</span><span class="sxs-lookup"><span data-stu-id="b2752-131">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete-item-site-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b2752-132">Java</span><span class="sxs-lookup"><span data-stu-id="b2752-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete-item-site-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Delete",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitem-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitem-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
