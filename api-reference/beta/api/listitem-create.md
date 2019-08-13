---
author: JeremyKelley
description: リストに新しい listItem を作成します。
ms.date: 09/11/2017
title: SharePoint リストに新しいエントリを作成する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 8b1b4ba187c204769d55355bebbfd5468aa6956c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343007"
---
# <a name="create-a-new-item-in-a-list"></a><span data-ttu-id="3d514-103">リストに新しいアイテムを作成する</span><span class="sxs-lookup"><span data-stu-id="3d514-103">Create a new item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d514-104">[list][] に新しい [listItem][] を作成します。</span><span class="sxs-lookup"><span data-stu-id="3d514-104">Create a new [listItem][] in a [list][].</span></span>

## <a name="permissions"></a><span data-ttu-id="3d514-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3d514-105">Permissions</span></span>

<span data-ttu-id="3d514-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3d514-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d514-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3d514-108">Permission type</span></span>      | <span data-ttu-id="3d514-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3d514-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d514-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3d514-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3d514-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d514-111">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3d514-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3d514-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d514-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3d514-113">Not supported.</span></span>    |
|<span data-ttu-id="3d514-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3d514-114">Application</span></span> | <span data-ttu-id="3d514-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d514-115">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d514-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3d514-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
```

## <a name="request-body"></a><span data-ttu-id="3d514-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="3d514-117">Request body</span></span>

<span data-ttu-id="3d514-118">要求本文で、作成する [listItem][] リソースの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3d514-118">In the request body, supply a JSON representation of the [listItem][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="3d514-119">例</span><span class="sxs-lookup"><span data-stu-id="3d514-119">Example</span></span>

<span data-ttu-id="3d514-120">新しい汎用リスト アイテムを作成する方法の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3d514-120">Here is an example of how to create a new generic list item.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3d514-121">プロトコル</span><span class="sxs-lookup"><span data-stu-id="3d514-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
POST https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
Content-Type: application/json

{
  "fields": {
    "Title": "Widget",
    "Color": "Purple",
    "Weight": 32
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3d514-122">C#</span><span class="sxs-lookup"><span data-stu-id="3d514-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3d514-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3d514-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3d514-124">目的-C</span><span class="sxs-lookup"><span data-stu-id="3d514-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3d514-125">Java</span><span class="sxs-lookup"><span data-stu-id="3d514-125">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="3d514-126">応答</span><span class="sxs-lookup"><span data-stu-id="3d514-126">Response</span></span>

<span data-ttu-id="3d514-127">成功した場合、このメソッドは作成されたリスト アイテムの応答本文で [listItem][] を返します。</span><span class="sxs-lookup"><span data-stu-id="3d514-127">If successful, this method returns a [listItem][] in the response body for the created list item.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "20",
  "createdDateTime": "2016-08-30T08:26:00Z",
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

<span data-ttu-id="3d514-128">**注:** 応答オブジェクトは、わかりやすくするために切り詰められています。</span><span class="sxs-lookup"><span data-stu-id="3d514-128">**Note:** The response object is truncated for clarity.</span></span> <span data-ttu-id="3d514-129">実際の呼び出しでは、既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="3d514-129">Default properties will be returned from the actual call.</span></span>

[list]: ../resources/list.md
[listItem]: ../resources/listitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Add a new item to a SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Create",
  "suppressions": [
  ]
}
-->
