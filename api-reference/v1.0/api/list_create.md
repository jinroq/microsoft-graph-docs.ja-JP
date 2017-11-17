---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: "SharePoint リストを作成する"
ms.openlocfilehash: 7ba657bda38c25ef8f1e5fdda2f7438794e04d2a
ms.sourcegitcommit: 339070a20730bc4d363da7eb346d5f3c1e1d6c3e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/18/2017
---
# <a name="create-a-new-list"></a><span data-ttu-id="c2e15-102">新しいリストを作成する</span><span class="sxs-lookup"><span data-stu-id="c2e15-102">Create a new list</span></span>

<span data-ttu-id="c2e15-103">[site][] で新しい [list][] を作成します。</span><span class="sxs-lookup"><span data-stu-id="c2e15-103">Create a new [list][] in a [site][].</span></span>

## <a name="permissions"></a><span data-ttu-id="c2e15-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c2e15-104">Permissions</span></span>

<span data-ttu-id="c2e15-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c2e15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|            <span data-ttu-id="c2e15-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c2e15-107">Permission type</span></span>             | <span data-ttu-id="c2e15-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c2e15-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="c2e15-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c2e15-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="c2e15-110">Sites.Manage.All</span><span class="sxs-lookup"><span data-stu-id="c2e15-110">Sites.Manage.All</span></span>                            |
| <span data-ttu-id="c2e15-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c2e15-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2e15-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c2e15-112">Not supported.</span></span>                              |
| <span data-ttu-id="c2e15-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c2e15-113">Application</span></span>                            | <span data-ttu-id="c2e15-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2e15-114">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c2e15-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c2e15-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

## <a name="request-body"></a><span data-ttu-id="c2e15-116">要求本文</span><span class="sxs-lookup"><span data-stu-id="c2e15-116">Request body</span></span>

<span data-ttu-id="c2e15-117">要求本文で、作成する [list][] リソースの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c2e15-117">In the request body, supply a JSON representation of the [list][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="c2e15-118">例</span><span class="sxs-lookup"><span data-stu-id="c2e15-118">Example</span></span>

<span data-ttu-id="c2e15-119">新しい汎用リストを作成する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c2e15-119">Here is an example of how to create a new generic list.</span></span>

<!-- { "blockType": "request", "name": "create-list", "scopes": "sites.readwrite.all" } -->

```http
POST /sites/{site-id}/lists
Content-Type: application/json

{
  "name": "Books",
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

<span data-ttu-id="c2e15-120">**注:** カスタム列はオプションです。</span><span class="sxs-lookup"><span data-stu-id="c2e15-120">**Note:** Custom columns are optional.</span></span>

<span data-ttu-id="c2e15-121">ここで指定した列だけでなく、参照された **template** で定義された列も含めて、新しいリストが作成されます。</span><span class="sxs-lookup"><span data-stu-id="c2e15-121">In addition to any columns specified here, new lists are created with columns defined in the referenced **template**.</span></span>
<span data-ttu-id="c2e15-122">**list** ファセットまたは **template** が指定されていない場合、リストは既定で _Title_ 列を含む `genericList` テンプレートとなります。</span><span class="sxs-lookup"><span data-stu-id="c2e15-122">If the **list** facet or **template** is unspecified, the list defaults to the `genericList` template, which includes a _Title_ column.</span></span>

## <a name="response"></a><span data-ttu-id="c2e15-123">応答</span><span class="sxs-lookup"><span data-stu-id="c2e15-123">Response</span></span>

<span data-ttu-id="c2e15-124">成功した場合、このメソッドは作成されたリストの応答本文で [list][] を返します。</span><span class="sxs-lookup"><span data-stu-id="c2e15-124">If successful, this method returns a [list][] in the response body for the created list.</span></span>

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

<span data-ttu-id="c2e15-125">**注:**応答オブジェクトは、わかりやすくするために切り詰められています。</span><span class="sxs-lookup"><span data-stu-id="c2e15-125">**Note:** The response object is truncated for clarity.</span></span>
<span data-ttu-id="c2e15-126">実際の呼び出しでは、既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c2e15-126">Default properties will be returned from the actual call.</span></span>

[list]: ../resources/list.md
[site]: ../resources/site.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "List/Create"
} -->
