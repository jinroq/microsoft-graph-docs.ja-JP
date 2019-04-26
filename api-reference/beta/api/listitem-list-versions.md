---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 旧バージョンの SharePoint リスト レコードを取得する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 843c2f501217f7ce1d7923835bf0a7b44a010950
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333497"
---
# <a name="listing-versions-of-a-listitem-preview"></a><span data-ttu-id="967ec-102">ListItem のバージョンを一覧表示する (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="967ec-102">Listing versions of a ListItem (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="967ec-103">SharePoint は、リスト アイテムの履歴を保持するように構成できます。</span><span class="sxs-lookup"><span data-stu-id="967ec-103">SharePoint can be configured to retain the history for list items.</span></span>

<span data-ttu-id="967ec-104">旧バージョンは、ユーザーまたは場所ごとに固有の場合がある管理者設定に応じて、一定期間保持することができます。</span><span class="sxs-lookup"><span data-stu-id="967ec-104">Previous versions may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="967ec-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="967ec-105">Permissions</span></span>

<span data-ttu-id="967ec-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="967ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="967ec-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="967ec-108">Permission type</span></span>             | <span data-ttu-id="967ec-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="967ec-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="967ec-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="967ec-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="967ec-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="967ec-111">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="967ec-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="967ec-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="967ec-113">該当なし</span><span class="sxs-lookup"><span data-stu-id="967ec-113">n/a</span></span>                                         |
| <span data-ttu-id="967ec-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="967ec-114">Application</span></span>                            | <span data-ttu-id="967ec-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="967ec-115">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="967ec-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="967ec-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="967ec-117">応答</span><span class="sxs-lookup"><span data-stu-id="967ec-117">Response</span></span>

<span data-ttu-id="967ec-118">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [ListItemVersion](../resources/listitemversion.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="967ec-118">If successful, this method returns a `200 OK` response code and collection of [ListItemVersion](../resources/listitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="967ec-119">例</span><span class="sxs-lookup"><span data-stu-id="967ec-119">Example</span></span>

<span data-ttu-id="967ec-120">次の使用例では、SharePoint リスト内のリスト アイテムのバージョンを取得します。</span><span class="sxs-lookup"><span data-stu-id="967ec-120">This example retrieves the versions of a listItem in a SharePoint list:</span></span>

### <a name="http-request"></a><span data-ttu-id="967ec-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="967ec-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions-listitem", "scopes": "files.read" } -->

```http
GET /sites/{site-id}/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="967ec-122">応答</span><span class="sxs-lookup"><span data-stu-id="967ec-122">Response</span></span>

<span data-ttu-id="967ec-123">バージョンのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="967ec-123">This returns a collection of versions:</span></span>

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
