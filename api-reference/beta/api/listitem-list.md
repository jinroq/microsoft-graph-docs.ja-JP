---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: SharePoint リストからアイテムを取得する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c96577782218a96952855147702fc6ecddab6652
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510401"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="84d09-102">リスト内のアイテムを列挙する</span><span class="sxs-lookup"><span data-stu-id="84d09-102">Enumerate items in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84d09-103">[リスト][]内の[アイテム][item]のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="84d09-103">Get the collection of [items][item] in a [list][].</span></span>

[リスト]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="84d09-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="84d09-105">Permissions</span></span>

<span data-ttu-id="84d09-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="84d09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84d09-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="84d09-108">Permission type</span></span>      | <span data-ttu-id="84d09-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="84d09-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84d09-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="84d09-110">Delegated (work or school account)</span></span> | <span data-ttu-id="84d09-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84d09-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="84d09-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="84d09-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84d09-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="84d09-113">Not supported.</span></span>    |
|<span data-ttu-id="84d09-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="84d09-114">Application</span></span> | <span data-ttu-id="84d09-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84d09-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="84d09-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="84d09-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="84d09-117">例</span><span class="sxs-lookup"><span data-stu-id="84d09-117">Example</span></span>

#### <a name="request"></a><span data-ttu-id="84d09-118">要求</span><span class="sxs-lookup"><span data-stu-id="84d09-118">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-items" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```

#### <a name="response"></a><span data-ttu-id="84d09-119">応答</span><span class="sxs-lookup"><span data-stu-id="84d09-119">Response</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Enumerate",
  "suppressions": [
    "Error: /api-reference/beta/api/listitem-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
