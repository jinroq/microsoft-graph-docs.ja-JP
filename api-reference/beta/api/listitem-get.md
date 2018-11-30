---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: SharePoint リストからエントリを取得する
ms.openlocfilehash: 240f9f285178407f167cfb66b790224aa24c35d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071825"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="69cf1-102">リスト内のアイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="69cf1-102">Get an item in a list</span></span>

> <span data-ttu-id="69cf1-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="69cf1-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69cf1-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69cf1-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="69cf1-105">[list][] 内の [item][] のメタデータを返します。</span><span class="sxs-lookup"><span data-stu-id="69cf1-105">Returns the metadata for an [item][] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="69cf1-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="69cf1-108">Permissions</span></span>

<span data-ttu-id="69cf1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="69cf1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69cf1-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="69cf1-111">Permission type</span></span>      | <span data-ttu-id="69cf1-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="69cf1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69cf1-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="69cf1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="69cf1-114">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69cf1-114">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="69cf1-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="69cf1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69cf1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69cf1-116">Not supported.</span></span>    |
|<span data-ttu-id="69cf1-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="69cf1-117">Application</span></span> | <span data-ttu-id="69cf1-118">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69cf1-118">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="69cf1-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="69cf1-119">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="69cf1-120">例</span><span class="sxs-lookup"><span data-stu-id="69cf1-120">Example</span></span>

##### <a name="request"></a><span data-ttu-id="69cf1-121">要求</span><span class="sxs-lookup"><span data-stu-id="69cf1-121">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="69cf1-122">応答</span><span class="sxs-lookup"><span data-stu-id="69cf1-122">Response</span></span>

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
