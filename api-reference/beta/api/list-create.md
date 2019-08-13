---
author: JeremyKelley
description: site で新しい list を作成します。
ms.date: 09/11/2017
title: SharePoint リストを作成する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: bbc23b04fe38e61e7e7313ca34ea9c2800854e8b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347130"
---
# <a name="create-a-new-list"></a><span data-ttu-id="419a4-103">新しいリストを作成する</span><span class="sxs-lookup"><span data-stu-id="419a4-103">Create a new list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="419a4-104">[site][] で新しい [list][] を作成します。</span><span class="sxs-lookup"><span data-stu-id="419a4-104">Create a new [list][] in a [site][].</span></span>

## <a name="permissions"></a><span data-ttu-id="419a4-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="419a4-105">Permissions</span></span>

<span data-ttu-id="419a4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="419a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="419a4-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="419a4-108">Permission type</span></span>             | <span data-ttu-id="419a4-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="419a4-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="419a4-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="419a4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="419a4-111">Sites.Manage.All</span><span class="sxs-lookup"><span data-stu-id="419a4-111">Sites.Manage.All</span></span>                            |
| <span data-ttu-id="419a4-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="419a4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="419a4-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="419a4-113">Not supported.</span></span>                              |
| <span data-ttu-id="419a4-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="419a4-114">Application</span></span>                            | <span data-ttu-id="419a4-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="419a4-115">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="419a4-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="419a4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="request-body"></a><span data-ttu-id="419a4-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="419a4-117">Request body</span></span>

<span data-ttu-id="419a4-118">要求本文で、作成する [list][] リソースの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="419a4-118">In the request body, supply a JSON representation of the [list][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="419a4-119">例</span><span class="sxs-lookup"><span data-stu-id="419a4-119">Example</span></span>

<span data-ttu-id="419a4-120">新しい汎用リストを作成する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="419a4-120">Here is an example of how to create a new generic list.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="419a4-121">プロトコル</span><span class="sxs-lookup"><span data-stu-id="419a4-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-list", "scopes": "sites.readwrite.all" } -->

```http
POST /sites/{site-id}/lists
Content-Type: application/json

{
  "displayName": "Books",
  "columns": [
    {
      "name": "Author",
      "text": { }
    },
    {
      "name": "PageCount",
      "number": { }
    }
  ],
  "list": {
    "template": "genericList"
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="419a4-122">C#</span><span class="sxs-lookup"><span data-stu-id="419a4-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="419a4-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="419a4-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="419a4-124">目的-C</span><span class="sxs-lookup"><span data-stu-id="419a4-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="419a4-125">Java</span><span class="sxs-lookup"><span data-stu-id="419a4-125">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-list-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="419a4-126">**注:** カスタム列はオプションです。</span><span class="sxs-lookup"><span data-stu-id="419a4-126">**Note:** Custom columns are optional.</span></span>

<span data-ttu-id="419a4-127">ここで指定した列だけでなく、参照された **template** で定義された列も含めて、新しいリストが作成されます。</span><span class="sxs-lookup"><span data-stu-id="419a4-127">In addition to any columns specified here, new lists are created with columns defined in the referenced **template**.</span></span>
<span data-ttu-id="419a4-128">**list** ファセットまたは **template** が指定されていない場合、リストは既定で _Title_ 列を含む `genericList` テンプレートとなります。</span><span class="sxs-lookup"><span data-stu-id="419a4-128">If the **list** facet or **template** is unspecified, the list defaults to the `genericList` template, which includes a _Title_ column.</span></span>

## <a name="response"></a><span data-ttu-id="419a4-129">応答</span><span class="sxs-lookup"><span data-stu-id="419a4-129">Response</span></span>

<span data-ttu-id="419a4-130">成功した場合、このメソッドは作成されたリストの応答本文で [list][] を返します。</span><span class="sxs-lookup"><span data-stu-id="419a4-130">If successful, this method returns a [list][] in the response body for the created list.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.list", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "22e03ef3-6ef4-424d-a1d3-92a337807c30",
  "createdDateTime": "2017-04-30T01:21:00Z",
  "createdBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  },
  "lastModifiedDateTime": "2016-08-30T08:26:00Z",
  "lastModifiedBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  }
}
```

<span data-ttu-id="419a4-131">**注:** 応答オブジェクトは、わかりやすくするために切り詰められています。</span><span class="sxs-lookup"><span data-stu-id="419a4-131">**Note:** The response object is truncated for clarity.</span></span>
<span data-ttu-id="419a4-132">実際の呼び出しでは、既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="419a4-132">Default properties will be returned from the actual call.</span></span>

[list]: ../resources/list.md
[サイト]: ../resources/site.md
[site]: ../resources/site.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a new SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "List/Create",
  "suppressions": [
  ]
}
-->
