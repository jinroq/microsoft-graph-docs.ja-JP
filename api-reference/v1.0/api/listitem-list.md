---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: SharePoint リストからアイテムを取得する
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 3739997cdc5410ecffbf21277ecff1497b60a190
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968639"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="11f01-102">リスト内のアイテムを列挙する</span><span class="sxs-lookup"><span data-stu-id="11f01-102">Enumerate items in a list</span></span>

<span data-ttu-id="11f01-103">[リスト][]内の[アイテム][item]のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="11f01-103">Get the collection of [items][item] in a [list][].</span></span>

[リスト]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="11f01-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="11f01-105">Permissions</span></span>

<span data-ttu-id="11f01-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="11f01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11f01-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="11f01-108">Permission type</span></span>      | <span data-ttu-id="11f01-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="11f01-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11f01-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="11f01-110">Delegated (work or school account)</span></span> | <span data-ttu-id="11f01-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11f01-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="11f01-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="11f01-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11f01-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11f01-113">Not supported.</span></span>    |
|<span data-ttu-id="11f01-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="11f01-114">Application</span></span> | <span data-ttu-id="11f01-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11f01-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="11f01-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="11f01-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="11f01-117">例</span><span class="sxs-lookup"><span data-stu-id="11f01-117">Example</span></span>

#### <a name="request"></a><span data-ttu-id="11f01-118">要求</span><span class="sxs-lookup"><span data-stu-id="11f01-118">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-items", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```

#### <a name="response"></a><span data-ttu-id="11f01-119">応答</span><span class="sxs-lookup"><span data-stu-id="11f01-119">Response</span></span>

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
