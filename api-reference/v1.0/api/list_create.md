---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: "SharePoint リストを作成する"
ms.openlocfilehash: ff7b20e828d8136a9cd6274d533191fd22d903ff
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="create-a-new-list"></a><span data-ttu-id="4099c-102">新しいリストを作成する</span><span class="sxs-lookup"><span data-stu-id="4099c-102">Create a new list item</span></span>

<span data-ttu-id="4099c-103">[site][] で新しい [list][] を作成します。</span><span class="sxs-lookup"><span data-stu-id="4099c-103">Create a new [list][] in a [site][].</span></span>

## <a name="permissions"></a><span data-ttu-id="4099c-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4099c-104">Permissions</span></span>

<span data-ttu-id="4099c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4099c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|            <span data-ttu-id="4099c-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4099c-107">Permission type</span></span>             | <span data-ttu-id="4099c-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4099c-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="4099c-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4099c-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="4099c-110">Sites.Manage.All</span><span class="sxs-lookup"><span data-stu-id="4099c-110">Sites.Manage.All</span></span>                            |
| <span data-ttu-id="4099c-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4099c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4099c-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4099c-112">Not supported.</span></span>                              |
| <span data-ttu-id="4099c-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4099c-113">Application</span></span>                            | <span data-ttu-id="4099c-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4099c-114">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4099c-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4099c-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="request-body"></a><span data-ttu-id="4099c-116">要求本文</span><span class="sxs-lookup"><span data-stu-id="4099c-116">Request body</span></span>

<span data-ttu-id="4099c-117">要求本文で、作成する [list][] リソースの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4099c-117">In the request body, supply a JSON representation of the [DriveItem][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="4099c-118">例</span><span class="sxs-lookup"><span data-stu-id="4099c-118">Example</span></span>

<span data-ttu-id="4099c-119">新しい汎用リストを作成する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4099c-119">Here is an example of how to create a new folder.</span></span>

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

<span data-ttu-id="4099c-120">**注:** カスタム列はオプションです。</span><span class="sxs-lookup"><span data-stu-id="4099c-120">**Note:** Custom columns are optional.</span></span>

<span data-ttu-id="4099c-121">ここで指定した列だけでなく、参照された **template** で定義された列も含めて、新しいリストが作成されます。</span><span class="sxs-lookup"><span data-stu-id="4099c-121">In addition to any columns specified here, new lists are created with columns defined in the referenced **template**.</span></span>
<span data-ttu-id="4099c-122">**list** ファセットまたは **template** が指定されていない場合、リストは既定で _Title_ 列を含む `genericList` テンプレートとなります。</span><span class="sxs-lookup"><span data-stu-id="4099c-122">If the **list** facet or **template** is unspecified, the list defaults to the `genericList` template, which includes a _Title_ column.</span></span>

## <a name="response"></a><span data-ttu-id="4099c-123">応答</span><span class="sxs-lookup"><span data-stu-id="4099c-123">Response</span></span>

<span data-ttu-id="4099c-124">成功した場合、このメソッドは作成されたリストの応答本文で [list][] を返します。</span><span class="sxs-lookup"><span data-stu-id="4099c-124">If successful, this method returns a [driveItem][] object in the response body for the newly created file.</span></span>

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

<span data-ttu-id="4099c-125">**注:** 応答オブジェクトは、わかりやすくするために切り詰められています。</span><span class="sxs-lookup"><span data-stu-id="4099c-125">**Note:** The response object is truncated for clarity.</span></span>
<span data-ttu-id="4099c-126">実際の呼び出しでは、既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4099c-126">All default properties will be returned from the actual call.</span></span>

[list]: ../resources/list.md
[site]: ../resources/site.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "List/Create"
} -->
