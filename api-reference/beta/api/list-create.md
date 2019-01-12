---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: SharePoint リストを作成する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 112a6a1a735bb527bdd2af7c64f02e4848b6e5f3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963977"
---
# <a name="create-a-new-list"></a><span data-ttu-id="67ea0-102">新しいリストを作成する</span><span class="sxs-lookup"><span data-stu-id="67ea0-102">Create a new list</span></span>

> <span data-ttu-id="67ea0-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="67ea0-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67ea0-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67ea0-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="67ea0-105">[site][] で新しい [list][] を作成します。</span><span class="sxs-lookup"><span data-stu-id="67ea0-105">Create a new [list][] in a [site][].</span></span>

## <a name="permissions"></a><span data-ttu-id="67ea0-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="67ea0-106">Permissions</span></span>

<span data-ttu-id="67ea0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="67ea0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="67ea0-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="67ea0-109">Permission type</span></span>             | <span data-ttu-id="67ea0-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="67ea0-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="67ea0-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="67ea0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="67ea0-112">Sites.Manage.All</span><span class="sxs-lookup"><span data-stu-id="67ea0-112">Sites.Manage.All</span></span>                            |
| <span data-ttu-id="67ea0-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="67ea0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67ea0-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67ea0-114">Not supported.</span></span>                              |
| <span data-ttu-id="67ea0-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="67ea0-115">Application</span></span>                            | <span data-ttu-id="67ea0-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67ea0-116">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="67ea0-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="67ea0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="request-body"></a><span data-ttu-id="67ea0-118">要求本文</span><span class="sxs-lookup"><span data-stu-id="67ea0-118">Request body</span></span>

<span data-ttu-id="67ea0-119">要求本文で、作成する [list][] リソースの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="67ea0-119">In the request body, supply a JSON representation of the [list][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="67ea0-120">例</span><span class="sxs-lookup"><span data-stu-id="67ea0-120">Example</span></span>

<span data-ttu-id="67ea0-121">新しい汎用リストを作成する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="67ea0-121">Here is an example of how to create a new generic list.</span></span>

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

<span data-ttu-id="67ea0-122">**注:** カスタム列はオプションです。</span><span class="sxs-lookup"><span data-stu-id="67ea0-122">**Note:** Custom columns are optional.</span></span>

<span data-ttu-id="67ea0-123">ここで指定した列だけでなく、参照された **template** で定義された列も含めて、新しいリストが作成されます。</span><span class="sxs-lookup"><span data-stu-id="67ea0-123">In addition to any columns specified here, new lists are created with columns defined in the referenced **template**.</span></span>
<span data-ttu-id="67ea0-124">**list** ファセットまたは **template** が指定されていない場合、リストは既定で _Title_ 列を含む `genericList` テンプレートとなります。</span><span class="sxs-lookup"><span data-stu-id="67ea0-124">If the **list** facet or **template** is unspecified, the list defaults to the `genericList` template, which includes a _Title_ column.</span></span>

## <a name="response"></a><span data-ttu-id="67ea0-125">応答</span><span class="sxs-lookup"><span data-stu-id="67ea0-125">Response</span></span>

<span data-ttu-id="67ea0-126">成功した場合、このメソッドは作成されたリストの応答本文で [list][] を返します。</span><span class="sxs-lookup"><span data-stu-id="67ea0-126">If successful, this method returns a [list][] in the response body for the created list.</span></span>

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

<span data-ttu-id="67ea0-127">**注:** 応答オブジェクトは、わかりやすくするために切り詰められています。</span><span class="sxs-lookup"><span data-stu-id="67ea0-127">**Note:** The response object is truncated for clarity.</span></span>
<span data-ttu-id="67ea0-128">実際の呼び出しでは、既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="67ea0-128">Default properties will be returned from the actual call.</span></span>

[list]: ../resources/list.md
[site]: ../resources/site.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "List/Create"
} -->
