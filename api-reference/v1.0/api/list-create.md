---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: SharePoint リストを作成する
localization_priority: Normal
ms.openlocfilehash: 724a34ea9add74772236b6d0dad90e23c9cac955
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878688"
---
# <a name="create-a-new-list"></a><span data-ttu-id="68949-102">新しいリストを作成する</span><span class="sxs-lookup"><span data-stu-id="68949-102">Create a new list</span></span>

<span data-ttu-id="68949-103">[site][] で新しい [list][] を作成します。</span><span class="sxs-lookup"><span data-stu-id="68949-103">Create a new [list][] in a [site][].</span></span>

## <a name="permissions"></a><span data-ttu-id="68949-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="68949-104">Permissions</span></span>

<span data-ttu-id="68949-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="68949-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="68949-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="68949-107">Permission type</span></span>             | <span data-ttu-id="68949-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="68949-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="68949-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="68949-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="68949-110">Sites.Manage.All</span><span class="sxs-lookup"><span data-stu-id="68949-110">Sites.Manage.All</span></span>                            |
| <span data-ttu-id="68949-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="68949-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68949-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68949-112">Not supported.</span></span>                              |
| <span data-ttu-id="68949-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="68949-113">Application</span></span>                            | <span data-ttu-id="68949-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68949-114">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="68949-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="68949-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

## <a name="request-body"></a><span data-ttu-id="68949-116">要求本文</span><span class="sxs-lookup"><span data-stu-id="68949-116">Request body</span></span>

<span data-ttu-id="68949-117">要求本文で、作成する [list][] リソースの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="68949-117">In the request body, supply a JSON representation of the [list][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="68949-118">例</span><span class="sxs-lookup"><span data-stu-id="68949-118">Example</span></span>

<span data-ttu-id="68949-119">新しい汎用リストを作成する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="68949-119">Here is an example of how to create a new generic list.</span></span>

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

<span data-ttu-id="68949-120">**注:** カスタム列はオプションです。</span><span class="sxs-lookup"><span data-stu-id="68949-120">**Note:** Custom columns are optional.</span></span>

<span data-ttu-id="68949-121">ここで指定した列だけでなく、参照された **template** で定義された列も含めて、新しいリストが作成されます。</span><span class="sxs-lookup"><span data-stu-id="68949-121">In addition to any columns specified here, new lists are created with columns defined in the referenced **template**.</span></span>
<span data-ttu-id="68949-122">**list** ファセットまたは **template** が指定されていない場合、リストは既定で _Title_ 列を含む `genericList` テンプレートとなります。</span><span class="sxs-lookup"><span data-stu-id="68949-122">If the **list** facet or **template** is unspecified, the list defaults to the `genericList` template, which includes a _Title_ column.</span></span>

## <a name="response"></a><span data-ttu-id="68949-123">応答</span><span class="sxs-lookup"><span data-stu-id="68949-123">Response</span></span>

<span data-ttu-id="68949-124">成功した場合、このメソッドは作成されたリストの応答本文で [list][] を返します。</span><span class="sxs-lookup"><span data-stu-id="68949-124">If successful, this method returns a [list][] in the response body for the created list.</span></span>

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

<span data-ttu-id="68949-125">**注:** 応答オブジェクトは、わかりやすくするために切り詰められています。</span><span class="sxs-lookup"><span data-stu-id="68949-125">**Note:** The response object is truncated for clarity.</span></span>
<span data-ttu-id="68949-126">実際の呼び出しでは、既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="68949-126">Default properties will be returned from the actual call.</span></span>

[list]: ../resources/list.md
[site]: ../resources/site.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "List/Create"
} -->
