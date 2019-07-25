---
author: chackman
ms.author: chackman
title: フォローされたアイテムを一覧表示する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1efa34191693a0511e28d00ea29accd54877a586
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861584"
---
# <a name="list-followed-items"></a><span data-ttu-id="f75ce-102">フォローされたアイテムを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f75ce-102">List followed items</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f75ce-103">サインインしているユーザーがフォローされている[アイテム](../resources/driveitem.md)を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="f75ce-103">List the [items](../resources/driveitem.md) that have been followed by the signed in user.</span></span>
<span data-ttu-id="f75ce-104">このコレクションには、ユーザーのドライブにあるアイテムと、他のドライブとの間でアクセス可能なアイテムが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f75ce-104">This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="f75ce-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f75ce-105">Permissions</span></span>

<span data-ttu-id="f75ce-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f75ce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f75ce-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f75ce-108">Permission type</span></span>      | <span data-ttu-id="f75ce-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f75ce-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f75ce-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f75ce-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f75ce-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f75ce-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f75ce-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f75ce-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f75ce-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f75ce-113">Not supported.</span></span>    |
|<span data-ttu-id="f75ce-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f75ce-114">Application</span></span> | <span data-ttu-id="f75ce-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f75ce-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f75ce-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f75ce-116">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f75ce-117">プロトコル</span><span class="sxs-lookup"><span data-stu-id="f75ce-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-followed-items", "scopes": "files.read" } -->

```http
GET /me/drive/following
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f75ce-118">C#</span><span class="sxs-lookup"><span data-stu-id="f75ce-118">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-followed-items-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f75ce-119">Javascript</span><span class="sxs-lookup"><span data-stu-id="f75ce-119">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-followed-items-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f75ce-120">目的-C</span><span class="sxs-lookup"><span data-stu-id="f75ce-120">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-followed-items-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f75ce-121">Java</span><span class="sxs-lookup"><span data-stu-id="f75ce-121">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-followed-items-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="f75ce-122">応答</span><span class="sxs-lookup"><span data-stu-id="f75ce-122">Response</span></span>

<span data-ttu-id="f75ce-123">このメソッドは、ドライブの所有者がフォローしているアイテムについて、drive [item](../resources/driveitem.md)リソースのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f75ce-123">This method returns a collection of [driveItem](../resources/driveitem.md) resources for items which the owner of the drive is following.</span></span>
<span data-ttu-id="f75ce-124">アイテムが見つからない場合は、空のコレクションが返されます。</span><span class="sxs-lookup"><span data-stu-id="f75ce-124">If no items were found, an empty collection is returned.</span></span>

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
