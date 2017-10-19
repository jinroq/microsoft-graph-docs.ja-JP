---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: "SharePoint リストからアイテムを取得する"
ms.openlocfilehash: a7f66db11ef201d0ae5afb2cc49887ee10dc89d7
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="3b3a8-102">リスト内のアイテムを列挙する</span><span class="sxs-lookup"><span data-stu-id="3b3a8-102">Enumerate items in a list</span></span>

<span data-ttu-id="3b3a8-103">[リスト][]内の[アイテム][item]のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="3b3a8-103">Get the collection of [items][item] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listItem.md

## <a name="permissions"></a><span data-ttu-id="3b3a8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3b3a8-105">Permissions</span></span>

<span data-ttu-id="3b3a8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3b3a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3b3a8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3b3a8-108">Permission type</span></span>      | <span data-ttu-id="3b3a8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3b3a8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b3a8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3b3a8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3b3a8-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b3a8-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3b3a8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3b3a8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b3a8-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b3a8-113">Not supported.</span></span>    |
|<span data-ttu-id="3b3a8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3b3a8-114">Application</span></span> | <span data-ttu-id="3b3a8-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b3a8-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b3a8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3b3a8-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="3b3a8-117">例</span><span class="sxs-lookup"><span data-stu-id="3b3a8-117">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3b3a8-118">要求</span><span class="sxs-lookup"><span data-stu-id="3b3a8-118">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-items" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```

#### <a name="response"></a><span data-ttu-id="3b3a8-119">応答</span><span class="sxs-lookup"><span data-stu-id="3b3a8-119">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.listItem)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "2",
      "fields": {
        "Name": "Gadget",
        "Color": "Red",
        "Quantity": 503
       }
    },
    {
      "id": "4",
      "fields": {
        "Name": "Widget",
        "Color": "Blue",
        "Quantity": 2357
       }
    },
    {
      "id": "7",
      "fields": {
        "Name": "Gizmo",
        "Color": "Green",
        "Quantity": 92
       }
    }
  ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Enumerate"
} -->
