---
title: リスト アイテムのバージョンを一覧表示
description: SharePoint は、リスト アイテムの履歴を保持するように構成できます。
ms.openlocfilehash: 43f28b355b733ba9651bba90f81179e59ebd3610
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021662"
---
# <a name="listing-versions-of-a-listitem"></a><span data-ttu-id="1759d-103">リスト アイテムのバージョンを一覧表示</span><span class="sxs-lookup"><span data-stu-id="1759d-103">Listing versions of a ListItem</span></span>

<span data-ttu-id="1759d-104">SharePoint は、リスト アイテムの履歴を保持するように構成できます。</span><span class="sxs-lookup"><span data-stu-id="1759d-104">SharePoint can be configured to retain the history for list items.</span></span>

<span data-ttu-id="1759d-105">旧バージョンは、ユーザーまたは場所ごとに固有の場合がある管理者設定に応じて、一定期間保持することができます。</span><span class="sxs-lookup"><span data-stu-id="1759d-105">Previous versions may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="1759d-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1759d-106">Permissions</span></span>

<span data-ttu-id="1759d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1759d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="1759d-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1759d-109">Permission type</span></span>             | <span data-ttu-id="1759d-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1759d-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="1759d-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1759d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1759d-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1759d-112">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="1759d-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1759d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1759d-114">該当なし</span><span class="sxs-lookup"><span data-stu-id="1759d-114">n/a</span></span>                                         |
| <span data-ttu-id="1759d-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1759d-115">Application</span></span>                            | <span data-ttu-id="1759d-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1759d-116">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="1759d-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1759d-117">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="1759d-118">応答</span><span class="sxs-lookup"><span data-stu-id="1759d-118">Response</span></span>

<span data-ttu-id="1759d-119">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [ListItemVersion](../resources/listitemversion.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="1759d-119">If successful, this method returns a `200 OK` response code and collection of [ListItemVersion](../resources/listitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="1759d-120">例</span><span class="sxs-lookup"><span data-stu-id="1759d-120">Example</span></span>

<span data-ttu-id="1759d-121">次の使用例では、SharePoint リスト内のリスト アイテムのバージョンを取得します。</span><span class="sxs-lookup"><span data-stu-id="1759d-121">This example retrieves the versions of a listItem in a SharePoint list:</span></span>

### <a name="http-request"></a><span data-ttu-id="1759d-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1759d-122">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions-listitem", "scopes": "files.read sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="1759d-123">応答</span><span class="sxs-lookup"><span data-stu-id="1759d-123">Response</span></span>

<span data-ttu-id="1759d-124">バージョンのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="1759d-124">This returns a collection of versions:</span></span>

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
  "tocPath": "Items/Version history"
} -->