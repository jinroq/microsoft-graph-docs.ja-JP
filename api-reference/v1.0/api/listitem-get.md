---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: SharePoint リストからエントリを取得する
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 1a1117717a0afc0d715da2297d69b0453ef2025e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950544"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="318b0-102">リスト内のアイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="318b0-102">Get an item in a list</span></span>

<span data-ttu-id="318b0-103">[list][] 内の [item][] のメタデータを返します。</span><span class="sxs-lookup"><span data-stu-id="318b0-103">Returns the metadata for an [item][] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="318b0-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="318b0-106">Permissions</span></span>

<span data-ttu-id="318b0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="318b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="318b0-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="318b0-109">Permission type</span></span>      | <span data-ttu-id="318b0-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="318b0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="318b0-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="318b0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="318b0-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="318b0-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="318b0-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="318b0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="318b0-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="318b0-114">Not supported.</span></span>    |
|<span data-ttu-id="318b0-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="318b0-115">Application</span></span> | <span data-ttu-id="318b0-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="318b0-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="318b0-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="318b0-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="318b0-118">例</span><span class="sxs-lookup"><span data-stu-id="318b0-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="318b0-119">要求</span><span class="sxs-lookup"><span data-stu-id="318b0-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="318b0-120">応答</span><span class="sxs-lookup"><span data-stu-id="318b0-120">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "5",
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
