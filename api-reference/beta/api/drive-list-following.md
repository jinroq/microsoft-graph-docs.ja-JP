---
author: chackman
ms.author: chackman
title: 後にリストのアイテム
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: df38a11a09f4ec86eb029f236030cc4565e5d939
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523310"
---
# <a name="list-followed-items"></a><span data-ttu-id="e8694-102">後にリストのアイテム</span><span class="sxs-lookup"><span data-stu-id="e8694-102">List followed items</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8694-103">サインインしているユーザーが行っている[項目](../resources/driveitem.md)を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="e8694-103">List the [items](../resources/driveitem.md) that have been followed by the signed in user.</span></span>
<span data-ttu-id="e8694-104">このコレクションには、アイテムを他のドライブへのアクセスがあるだけでなく、ユーザーのドライブにある項目が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e8694-104">This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8694-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e8694-105">Permissions</span></span>

<span data-ttu-id="e8694-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e8694-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8694-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e8694-108">Permission type</span></span>      | <span data-ttu-id="e8694-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e8694-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8694-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e8694-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e8694-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8694-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e8694-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e8694-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8694-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8694-113">Not supported.</span></span>    |
|<span data-ttu-id="e8694-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e8694-114">Application</span></span> | <span data-ttu-id="e8694-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8694-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8694-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e8694-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-followed-items", "scopes": "files.read" } -->

```http
GET /me/drive/following
```

## <a name="response"></a><span data-ttu-id="e8694-117">応答</span><span class="sxs-lookup"><span data-stu-id="e8694-117">Response</span></span>

<span data-ttu-id="e8694-118">このメソッドでは、ドライブの所有者は、次の項目の[driveItem](../resources/driveitem.md)リソースのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e8694-118">This method returns a collection of [driveItem](../resources/driveitem.md) resources for items which the owner of the drive is following.</span></span>
<span data-ttu-id="e8694-119">アイテムが見つからなかった場合、空のコレクションが返されます。</span><span class="sxs-lookup"><span data-stu-id="e8694-119">If no items were found, an empty collection is returned.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "1312abc!1231",
      "name": "March Proposal.docx",
      "size": 19121,
      "lastModifiedDateTime": "2017-12-12T10:40:59Z"
    },
    {
      "id": "1312def!9943",
      "name": "Vacation.jpg",
      "size": 37810,
      "lastModifiedDateTime": "2016-10-18T10:40:59Z"
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "List the items a user is following.",
  "keywords": "drive,onedrive.drive,list followed items",
  "section": "documentation",
  "tocPath": "Drives/List followed items",
  "suppressions": [
    "Error: /api-reference/beta/api/drive-list-following.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
