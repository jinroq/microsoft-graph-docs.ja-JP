---
title: ListItem のバージョンの一覧表示
description: SharePoint は、リスト アイテムの履歴を保持するように構成できます。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5d242fa9d152b62f4dfbc617277623ee0b6d542d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271975"
---
# <a name="listing-versions-of-a-listitem"></a><span data-ttu-id="3962a-103">ListItem のバージョンの一覧表示</span><span class="sxs-lookup"><span data-stu-id="3962a-103">Listing versions of a ListItem</span></span>

<span data-ttu-id="3962a-104">SharePoint は、リスト アイテムの履歴を保持するように構成できます。</span><span class="sxs-lookup"><span data-stu-id="3962a-104">SharePoint can be configured to retain the history for list items.</span></span>

<span data-ttu-id="3962a-105">旧バージョンは、ユーザーまたは場所ごとに固有の場合がある管理者設定に応じて、一定期間保持することができます。</span><span class="sxs-lookup"><span data-stu-id="3962a-105">Previous versions may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="3962a-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3962a-106">Permissions</span></span>

<span data-ttu-id="3962a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3962a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="3962a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3962a-109">Permission type</span></span>             | <span data-ttu-id="3962a-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3962a-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="3962a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3962a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3962a-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3962a-112">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="3962a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3962a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3962a-114">該当なし</span><span class="sxs-lookup"><span data-stu-id="3962a-114">n/a</span></span>                                         |
| <span data-ttu-id="3962a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3962a-115">Application</span></span>                            | <span data-ttu-id="3962a-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3962a-116">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="3962a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3962a-117">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="3962a-118">応答</span><span class="sxs-lookup"><span data-stu-id="3962a-118">Response</span></span>

<span data-ttu-id="3962a-119">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [ListItemVersion](../resources/listitemversion.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="3962a-119">If successful, this method returns a `200 OK` response code and collection of [ListItemVersion](../resources/listitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="3962a-120">例</span><span class="sxs-lookup"><span data-stu-id="3962a-120">Example</span></span>

<span data-ttu-id="3962a-121">次の使用例では、SharePoint リスト内のリスト アイテムのバージョンを取得します。</span><span class="sxs-lookup"><span data-stu-id="3962a-121">This example retrieves the versions of a listItem in a SharePoint list:</span></span>

### <a name="http-request"></a><span data-ttu-id="3962a-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3962a-122">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions-listitem", "scopes": "files.read sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="3962a-123">応答</span><span class="sxs-lookup"><span data-stu-id="3962a-123">Response</span></span>

<span data-ttu-id="3962a-124">バージョンのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="3962a-124">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.listItemVersion)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value":
  [
    {
      "id": "3.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-14T12:34:53.912Z"
    },
    {
      "id": "2.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-11T10:21:03.000Z"
    },
    {
      "id": "1.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-10T15:20:01.125Z"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3962a-125">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="3962a-125">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3962a-126">C#</span><span class="sxs-lookup"><span data-stu-id="3962a-126">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-previous-versions-listitem-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3962a-127">Javascript</span><span class="sxs-lookup"><span data-stu-id="3962a-127">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-previous-versions-listitem-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3962a-128">目的-C</span><span class="sxs-lookup"><span data-stu-id="3962a-128">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-previous-versions-listitem-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitem-list-versions.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/listitem-list-versions.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitem-list-versions.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
