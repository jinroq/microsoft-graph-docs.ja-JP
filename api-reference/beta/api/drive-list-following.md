---
author: chackman
ms.author: chackman
title: 後にリストのアイテム
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 0489c14b943b6fa6eafb41932bb9bb906fea3351
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921480"
---
# <a name="list-followed-items"></a><span data-ttu-id="56980-102">後にリストのアイテム</span><span class="sxs-lookup"><span data-stu-id="56980-102">List followed items</span></span>

> <span data-ttu-id="56980-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="56980-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56980-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56980-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="56980-105">サインインしているユーザーが行っている[項目](../resources/driveitem.md)を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="56980-105">List the [items](../resources/driveitem.md) that have been followed by the signed in user.</span></span>
<span data-ttu-id="56980-106">このコレクションには、アイテムを他のドライブへのアクセスがあるだけでなく、ユーザーのドライブにある項目が含まれています。</span><span class="sxs-lookup"><span data-stu-id="56980-106">This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="56980-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="56980-107">Permissions</span></span>

<span data-ttu-id="56980-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="56980-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56980-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="56980-110">Permission type</span></span>      | <span data-ttu-id="56980-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="56980-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56980-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="56980-112">Delegated (work or school account)</span></span> | <span data-ttu-id="56980-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56980-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="56980-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="56980-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56980-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56980-115">Not supported.</span></span>    |
|<span data-ttu-id="56980-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="56980-116">Application</span></span> | <span data-ttu-id="56980-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56980-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="56980-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="56980-118">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-followed-items", "scopes": "files.read" } -->

```http
GET /me/drive/following
```

## <a name="response"></a><span data-ttu-id="56980-119">応答</span><span class="sxs-lookup"><span data-stu-id="56980-119">Response</span></span>

<span data-ttu-id="56980-120">このメソッドでは、ドライブの所有者は、次の項目の[driveItem](../resources/driveitem.md)リソースのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="56980-120">This method returns a collection of [driveItem](../resources/driveitem.md) resources for items which the owner of the drive is following.</span></span>
<span data-ttu-id="56980-121">アイテムが見つからなかった場合、空のコレクションが返されます。</span><span class="sxs-lookup"><span data-stu-id="56980-121">If no items were found, an empty collection is returned.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "List the items a user is following.",
  "keywords": "drive,onedrive.drive,list followed items",
  "section": "documentation",
  "tocPath": "Drives/List followed items"
} -->
