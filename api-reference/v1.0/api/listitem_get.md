---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: "SharePoint リストからエントリを取得する"
ms.openlocfilehash: 29db5f5a3005aca0003489db4bdb13219e612a96
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="e4769-102">リスト内のアイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="e4769-102">Get an item in a list</span></span>

<span data-ttu-id="e4769-103">[list][] 内の [item][] のメタデータを返します。</span><span class="sxs-lookup"><span data-stu-id="e4769-103">Returns the metadata for an [item][] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listItem.md

## <a name="permissions"></a><span data-ttu-id="e4769-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e4769-106">Permissions</span></span>

<span data-ttu-id="e4769-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e4769-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e4769-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e4769-109">Permission type</span></span>      | <span data-ttu-id="e4769-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e4769-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4769-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e4769-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e4769-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4769-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e4769-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e4769-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4769-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e4769-114">Not supported.</span></span>    |
|<span data-ttu-id="e4769-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e4769-115">Application</span></span> | <span data-ttu-id="e4769-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4769-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4769-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e4769-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="e4769-118">例</span><span class="sxs-lookup"><span data-stu-id="e4769-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e4769-119">要求</span><span class="sxs-lookup"><span data-stu-id="e4769-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="e4769-120">応答</span><span class="sxs-lookup"><span data-stu-id="e4769-120">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "d14922d8-43e6-4c8a-b029-e35c5b4e0d63",
  "listItemId": 2,
  "fields": {
    "Name": "Widget",
    "Color": "Blue",
    "Quantity": 2357
    }
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata"
} -->
