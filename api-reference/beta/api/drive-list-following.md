---
author: chackman
description: サインインしているユーザーがフォローされているアイテムを一覧表示します。
title: フォローされたアイテムを一覧表示する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: c8fface18f7b783d463f4df57f97c610a45103ab
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321220"
---
# <a name="list-followed-items"></a><span data-ttu-id="5479c-103">フォローされたアイテムを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="5479c-103">List followed items</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5479c-104">サインインしているユーザーがフォローされている[アイテム](../resources/driveitem.md)を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="5479c-104">List the [items](../resources/driveitem.md) that have been followed by the signed in user.</span></span>
<span data-ttu-id="5479c-105">このコレクションには、ユーザーのドライブにあるアイテムと、他のドライブとの間でアクセス可能なアイテムが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5479c-105">This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="5479c-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5479c-106">Permissions</span></span>

<span data-ttu-id="5479c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5479c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5479c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5479c-109">Permission type</span></span>      | <span data-ttu-id="5479c-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5479c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5479c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5479c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5479c-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5479c-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="5479c-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5479c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5479c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5479c-114">Not supported.</span></span>    |
|<span data-ttu-id="5479c-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5479c-115">Application</span></span> | <span data-ttu-id="5479c-116">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5479c-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5479c-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5479c-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5479c-118">プロトコル</span><span class="sxs-lookup"><span data-stu-id="5479c-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-followed-items", "scopes": "files.read" } -->

```http
GET /me/drive/following
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5479c-119">C#</span><span class="sxs-lookup"><span data-stu-id="5479c-119">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-followed-items-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5479c-120">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5479c-120">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-followed-items-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5479c-121">目的-C</span><span class="sxs-lookup"><span data-stu-id="5479c-121">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-followed-items-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5479c-122">Java</span><span class="sxs-lookup"><span data-stu-id="5479c-122">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-followed-items-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="5479c-123">応答</span><span class="sxs-lookup"><span data-stu-id="5479c-123">Response</span></span>

<span data-ttu-id="5479c-124">このメソッドは、ドライブの所有者がフォローしているアイテムについて、drive [item](../resources/driveitem.md)リソースのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="5479c-124">This method returns a collection of [driveItem](../resources/driveitem.md) resources for items which the owner of the drive is following.</span></span>
<span data-ttu-id="5479c-125">アイテムが見つからない場合は、空のコレクションが返されます。</span><span class="sxs-lookup"><span data-stu-id="5479c-125">If no items were found, an empty collection is returned.</span></span>

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
  ]
}
-->
