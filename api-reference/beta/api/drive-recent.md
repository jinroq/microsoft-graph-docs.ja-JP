---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 最近使用したファイルを一覧表示する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e0e7d6fc4dc16f11f76b4c021f957a8ae580acba
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861511"
---
# <a name="list-recent-files"></a><span data-ttu-id="8d93f-102">最近使用したファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="8d93f-102">List recent files</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d93f-p101">サインインしたユーザーによって最近使用されたアイテムのセットを一覧表示します。このコレクションには、ユーザーのドライブにあるアイテムと、他のドライブとの間でアクセス可能なアイテムが含まれています。</span><span class="sxs-lookup"><span data-stu-id="8d93f-p101">List a set of items that have been recently used by the signed in user. This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d93f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8d93f-105">Permissions</span></span>

<span data-ttu-id="8d93f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8d93f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d93f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8d93f-108">Permission type</span></span>      | <span data-ttu-id="8d93f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8d93f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d93f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8d93f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8d93f-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d93f-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8d93f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8d93f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d93f-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d93f-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="8d93f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8d93f-114">Application</span></span> | <span data-ttu-id="8d93f-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d93f-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d93f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8d93f-116">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8d93f-117">プロトコル</span><span class="sxs-lookup"><span data-stu-id="8d93f-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request",
       "name": "view-recent-files", 
       "scopes": "files.read",
       "target": "action" } -->

```http
GET /me/drive/recent
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8d93f-118">C#</span><span class="sxs-lookup"><span data-stu-id="8d93f-118">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/view-recent-files-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8d93f-119">Javascript</span><span class="sxs-lookup"><span data-stu-id="8d93f-119">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/view-recent-files-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8d93f-120">目的-C</span><span class="sxs-lookup"><span data-stu-id="8d93f-120">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/view-recent-files-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8d93f-121">Java</span><span class="sxs-lookup"><span data-stu-id="8d93f-121">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/view-recent-files-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="8d93f-122">応答</span><span class="sxs-lookup"><span data-stu-id="8d93f-122">Response</span></span>

<span data-ttu-id="8d93f-123">このメソッドは、ドライブの所有者が最近アクセスしたアイテムの [DriveItem](../resources/driveitem.md) リソースのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="8d93f-123">This method returns a collection of [DriveItem](../resources/driveitem.md) resources for items which the owner of the drive has recently accessed.</span></span>

<!-- { "blockType": "response",
       "@odata.type": "Collection(microsoft.graph.driveItem)",
       "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1312abc!1231",
      "remoteItem":
      {
        "id": "1991210caf!192",
        "name": "March Proposal.docx",
        "file": { },
        "size": 19121,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      },
      "fileSystemInfo": {
        "lastAccessedDateTime": "2017-02-20T19:13:00Z"
      }
    },
    {
      "id": "1312def!9943",
      "name": "Vacation.jpg",
      "file": { },
      "size": 37810,
      "parentReference": {
        "driveId": "1312def",
        "id": "1312def!123"
      },
      "fileSystemInfo": {
        "lastAccessedDateTime": "2017-02-20T16:43:21Z"
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="8d93f-124">備考</span><span class="sxs-lookup"><span data-stu-id="8d93f-124">Remarks</span></span>

<span data-ttu-id="8d93f-p103">**recent** アクションから返された DriveItems の中には、それらが異なるドライブからのアイテムであることを示す **remoteItem** ファセットが含まれるものがあります。元の DriveItem オブジェクトにアクセスするには、**remoteItem** で提供された情報を使用して、以下に示す書式で要求を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8d93f-p103">Some driveItems returned from the **recent** action will include the **remoteItem** facet which indicates they are items from another drive. To access the original driveItem object, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

<!-- { "blockType": "ignored", "name": "drives-get-remoteitem" } -->

```http
GET /drives/{remoteItem-driveId}/items/{remoteItem-id}
```

<!--
{
  "type": "#page.annotation",
  "description": "Retrieve a list of recently used files for the owner of the drive.",
  "keywords": "drive,onedrive.drive,default drive",
  "section": "documentation",
  "tocPath": "Drives/Recent files",
  "suppressions": [
  ]
}
-->
