---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 旧バージョンのリスト アイテムを取得する - SharePoint API
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 4068ebd1e8a245f2418954ce04bad1f78530acd0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983878"
---
# <a name="get-a-listitemversion-resource-preview"></a><span data-ttu-id="edbb8-102">ListItemVersion リソースを取得する (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="edbb8-102">Get a ListItemVersion resource (preview)</span></span>

> <span data-ttu-id="edbb8-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="edbb8-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="edbb8-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="edbb8-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="edbb8-105">[ListItem](../resources/listitem.md) の特定のバージョンのメタデータを取得します。</span><span class="sxs-lookup"><span data-stu-id="edbb8-105">Retrieve the metadata for a specific version of a [ListItem](../resources/listitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="edbb8-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="edbb8-106">Permissions</span></span>

<span data-ttu-id="edbb8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="edbb8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="edbb8-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="edbb8-109">Permission type</span></span>             | <span data-ttu-id="edbb8-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="edbb8-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="edbb8-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="edbb8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="edbb8-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edbb8-112">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="edbb8-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="edbb8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="edbb8-114">該当なし</span><span class="sxs-lookup"><span data-stu-id="edbb8-114">n/a</span></span>                                         |
| <span data-ttu-id="edbb8-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="edbb8-115">Application</span></span>                            | <span data-ttu-id="edbb8-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edbb8-116">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="edbb8-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="edbb8-117">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a><span data-ttu-id="edbb8-118">応答</span><span class="sxs-lookup"><span data-stu-id="edbb8-118">Response</span></span>

<span data-ttu-id="edbb8-119">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [ListItemVersion](../resources/listitemversion.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="edbb8-119">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/listitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="edbb8-120">例</span><span class="sxs-lookup"><span data-stu-id="edbb8-120">Example</span></span>

<span data-ttu-id="edbb8-121">この例では、listItem の 1 つのバージョンを取得し、fields コレクションを展開して listItem 内のフィールドの値を要求します。</span><span class="sxs-lookup"><span data-stu-id="edbb8-121">This example retrieves a version of a listItem and expands the fields collection to request the values of fields in the listItem.</span></span>

### <a name="http-request"></a><span data-ttu-id="edbb8-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="edbb8-122">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read" } -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}?expand=fields
```

### <a name="response"></a><span data-ttu-id="edbb8-123">応答</span><span class="sxs-lookup"><span data-stu-id="edbb8-123">Response</span></span>

<span data-ttu-id="edbb8-124">バージョンのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="edbb8-124">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItemVersion", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "1.0",
    "lastModifiedBy": {
    "user": {
        "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
        "displayName": "Ryan Gregg"
    }
    },
    "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
    "fields": {  }
}
```

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
