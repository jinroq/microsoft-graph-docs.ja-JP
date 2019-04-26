---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 旧バージョンのリスト アイテムを取得する - SharePoint API
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 2193c2e23ad5227e9118f23a782fbaa24756f88b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338706"
---
# <a name="get-a-listitemversion-resource-preview"></a><span data-ttu-id="88a39-102">ListItemVersion リソースを取得する (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="88a39-102">Get a ListItemVersion resource (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88a39-103">[ListItem](../resources/listitem.md) の特定のバージョンのメタデータを取得します。</span><span class="sxs-lookup"><span data-stu-id="88a39-103">Retrieve the metadata for a specific version of a [ListItem](../resources/listitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="88a39-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="88a39-104">Permissions</span></span>

<span data-ttu-id="88a39-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="88a39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="88a39-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="88a39-107">Permission type</span></span>             | <span data-ttu-id="88a39-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="88a39-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="88a39-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="88a39-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="88a39-110">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88a39-110">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="88a39-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="88a39-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88a39-112">該当なし</span><span class="sxs-lookup"><span data-stu-id="88a39-112">n/a</span></span>                                         |
| <span data-ttu-id="88a39-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="88a39-113">Application</span></span>                            | <span data-ttu-id="88a39-114">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88a39-114">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="88a39-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="88a39-115">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a><span data-ttu-id="88a39-116">応答</span><span class="sxs-lookup"><span data-stu-id="88a39-116">Response</span></span>

<span data-ttu-id="88a39-117">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [ListItemVersion](../resources/listitemversion.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="88a39-117">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/listitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="88a39-118">例</span><span class="sxs-lookup"><span data-stu-id="88a39-118">Example</span></span>

<span data-ttu-id="88a39-119">この例では、listItem の 1 つのバージョンを取得し、fields コレクションを展開して listItem 内のフィールドの値を要求します。</span><span class="sxs-lookup"><span data-stu-id="88a39-119">This example retrieves a version of a listItem and expands the fields collection to request the values of fields in the listItem.</span></span>

### <a name="http-request"></a><span data-ttu-id="88a39-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="88a39-120">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read" } -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}?expand=fields
```

### <a name="response"></a><span data-ttu-id="88a39-121">応答</span><span class="sxs-lookup"><span data-stu-id="88a39-121">Response</span></span>

<span data-ttu-id="88a39-122">バージョンのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="88a39-122">This returns a collection of versions:</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": []
}
-->
