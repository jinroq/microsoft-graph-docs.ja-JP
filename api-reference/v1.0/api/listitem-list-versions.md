---
title: ListItem のバージョンの一覧表示
description: SharePoint は、リスト アイテムの履歴を保持するように構成できます。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: fcff5934cddaef1b49b03e01f023c9e3c7ce1e71
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884561"
---
# <a name="listing-versions-of-a-listitem"></a><span data-ttu-id="3c4c5-103">ListItem のバージョンの一覧表示</span><span class="sxs-lookup"><span data-stu-id="3c4c5-103">Listing versions of a ListItem</span></span>

<span data-ttu-id="3c4c5-104">SharePoint は、リスト アイテムの履歴を保持するように構成できます。</span><span class="sxs-lookup"><span data-stu-id="3c4c5-104">SharePoint can be configured to retain the history for list items.</span></span>

<span data-ttu-id="3c4c5-105">旧バージョンは、ユーザーまたは場所ごとに固有の場合がある管理者設定に応じて、一定期間保持することができます。</span><span class="sxs-lookup"><span data-stu-id="3c4c5-105">Previous versions may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c4c5-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3c4c5-106">Permissions</span></span>

<span data-ttu-id="3c4c5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3c4c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="3c4c5-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3c4c5-109">Permission type</span></span>             | <span data-ttu-id="3c4c5-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3c4c5-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="3c4c5-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3c4c5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3c4c5-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c4c5-112">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="3c4c5-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3c4c5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c4c5-114">該当なし</span><span class="sxs-lookup"><span data-stu-id="3c4c5-114">n/a</span></span>                                         |
| <span data-ttu-id="3c4c5-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3c4c5-115">Application</span></span>                            | <span data-ttu-id="3c4c5-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c4c5-116">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="3c4c5-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3c4c5-117">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="3c4c5-118">応答</span><span class="sxs-lookup"><span data-stu-id="3c4c5-118">Response</span></span>

<span data-ttu-id="3c4c5-119">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [ListItemVersion](../resources/listitemversion.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="3c4c5-119">If successful, this method returns a `200 OK` response code and collection of [ListItemVersion](../resources/listitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="3c4c5-120">例</span><span class="sxs-lookup"><span data-stu-id="3c4c5-120">Example</span></span>

<span data-ttu-id="3c4c5-121">次の使用例では、SharePoint リスト内のリスト アイテムのバージョンを取得します。</span><span class="sxs-lookup"><span data-stu-id="3c4c5-121">This example retrieves the versions of a listItem in a SharePoint list:</span></span>

### <a name="http-request"></a><span data-ttu-id="3c4c5-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3c4c5-122">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3c4c5-123">プロトコル</span><span class="sxs-lookup"><span data-stu-id="3c4c5-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-previous-versions-listitem", "scopes": "files.read sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3c4c5-124">C#</span><span class="sxs-lookup"><span data-stu-id="3c4c5-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-previous-versions-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3c4c5-125">Javascript</span><span class="sxs-lookup"><span data-stu-id="3c4c5-125">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-previous-versions-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3c4c5-126">目的-C</span><span class="sxs-lookup"><span data-stu-id="3c4c5-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-previous-versions-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3c4c5-127">Java</span><span class="sxs-lookup"><span data-stu-id="3c4c5-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-previous-versions-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3c4c5-128">応答</span><span class="sxs-lookup"><span data-stu-id="3c4c5-128">Response</span></span>

<span data-ttu-id="3c4c5-129">バージョンのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="3c4c5-129">This returns a collection of versions:</span></span>

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


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
  ]
} -->
