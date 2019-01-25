---
author: chackman
ms.author: chackman
title: 次のドライブのアイテム
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b0c8835593ed7203cc6239485f1dcd4f17f24fe7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518339"
---
# <a name="follow-drive-item"></a><span data-ttu-id="8bddb-102">次のドライブのアイテム</span><span class="sxs-lookup"><span data-stu-id="8bddb-102">Follow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bddb-103">の[driveItem](../resources/driveitem.md)に従います。</span><span class="sxs-lookup"><span data-stu-id="8bddb-103">Follow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="8bddb-104">**注:** アイテムのフォローを取り消し、[フォロー取り消しの項目](driveitem-unfollow.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8bddb-104">**Note:** To unfollow an item, see [Unfollow item](driveitem-unfollow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8bddb-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8bddb-105">Permissions</span></span>

<span data-ttu-id="8bddb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8bddb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bddb-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8bddb-108">Permission type</span></span>      | <span data-ttu-id="8bddb-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8bddb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8bddb-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8bddb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8bddb-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bddb-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8bddb-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8bddb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bddb-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8bddb-113">Not supported.</span></span>    |
|<span data-ttu-id="8bddb-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8bddb-114">Application</span></span> | <span data-ttu-id="8bddb-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bddb-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8bddb-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8bddb-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/follow
POST /groups/{group-id/drive/items/{item-id}/follow
POST /me/drive/items/{item-id}/follow
POST /sites/{site-id}/drive/items/{item-id}/follow
POST /users/{user-id}/drive/items/{item-id}/follow
```

## <a name="request-body"></a><span data-ttu-id="8bddb-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="8bddb-117">Request body</span></span>

<span data-ttu-id="8bddb-118">要求の本文は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="8bddb-118">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="8bddb-119">応答</span><span class="sxs-lookup"><span data-stu-id="8bddb-119">Response</span></span>

<span data-ttu-id="8bddb-120">このメソッドでは、フォローされている項目については、 [DriveItem](../resources/driveitem.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="8bddb-120">This method returns a [DriveItem](../resources/driveitem.md) for the item being followed.</span></span>

## <a name="example"></a><span data-ttu-id="8bddb-121">例</span><span class="sxs-lookup"><span data-stu-id="8bddb-121">Example</span></span>

<span data-ttu-id="8bddb-122">次の使用例は次によって識別される項目は、 `{item-id}`。</span><span class="sxs-lookup"><span data-stu-id="8bddb-122">This example follows an item identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "follow-item", "scopes": "files.read", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/follow
```

<!--
{
  "type": "#page.annotation",
  "description": "Follow an item.",
  "keywords": "follow item",
  "section": "documentation",
  "tocPath": "Items/Follow",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-follow.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "1312abc!1231",
  "name": "March Proposal.docx",
  "size": 19121,
  "lastModifiedDateTime": "2017-12-12T10:40:59Z"
}
```
