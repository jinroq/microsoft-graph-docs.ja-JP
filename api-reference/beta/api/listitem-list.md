---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: SharePoint リストからアイテムを取得する
ms.openlocfilehash: 3c6a8259f17091612cf10e1501a24d9eb60e28d4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067749"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="d6c62-102">リスト内のアイテムを列挙する</span><span class="sxs-lookup"><span data-stu-id="d6c62-102">Enumerate items in a list</span></span>

> <span data-ttu-id="d6c62-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d6c62-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6c62-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6c62-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d6c62-105">[リスト][]内の[アイテム][item]のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="d6c62-105">Get the collection of [items][item] in a [list][].</span></span>

[リスト]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="d6c62-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d6c62-107">Permissions</span></span>

<span data-ttu-id="d6c62-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d6c62-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6c62-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d6c62-110">Permission type</span></span>      | <span data-ttu-id="d6c62-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d6c62-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6c62-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d6c62-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d6c62-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6c62-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d6c62-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d6c62-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6c62-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6c62-115">Not supported.</span></span>    |
|<span data-ttu-id="d6c62-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d6c62-116">Application</span></span> | <span data-ttu-id="d6c62-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6c62-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6c62-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d6c62-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="d6c62-119">例</span><span class="sxs-lookup"><span data-stu-id="d6c62-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d6c62-120">要求</span><span class="sxs-lookup"><span data-stu-id="d6c62-120">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-items" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```

#### <a name="response"></a><span data-ttu-id="d6c62-121">応答</span><span class="sxs-lookup"><span data-stu-id="d6c62-121">Response</span></span>

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