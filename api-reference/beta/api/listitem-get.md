---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: SharePoint リストからエントリを取得する
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 60a413060a3b86264cd1b1ae1a2fbc632c98e7bf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540976"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="823c2-102">リスト内のアイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="823c2-102">Get an item in a list</span></span>

<span data-ttu-id="823c2-103">[list][] 内の [item][] のメタデータを返します。</span><span class="sxs-lookup"><span data-stu-id="823c2-103">Returns the metadata for an [item][] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="823c2-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="823c2-106">Permissions</span></span>

<span data-ttu-id="823c2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="823c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="823c2-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="823c2-109">Permission type</span></span>      | <span data-ttu-id="823c2-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="823c2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="823c2-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="823c2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="823c2-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="823c2-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="823c2-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="823c2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="823c2-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="823c2-114">Not supported.</span></span>    |
|<span data-ttu-id="823c2-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="823c2-115">Application</span></span> | <span data-ttu-id="823c2-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="823c2-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="823c2-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="823c2-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="823c2-118">例</span><span class="sxs-lookup"><span data-stu-id="823c2-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="823c2-119">要求</span><span class="sxs-lookup"><span data-stu-id="823c2-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="823c2-120">応答</span><span class="sxs-lookup"><span data-stu-id="823c2-120">Response</span></span>

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
