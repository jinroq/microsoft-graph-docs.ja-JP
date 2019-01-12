---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 最近使用したファイルを一覧表示する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: d99caa91bc0b5d7140d3628db42955e558de3598
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915403"
---
# <a name="list-recent-files"></a><span data-ttu-id="a6da7-102">最近使用したファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a6da7-102">List recent files</span></span>

> <span data-ttu-id="a6da7-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a6da7-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6da7-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6da7-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a6da7-p102">サインインしたユーザーによって最近使用されたアイテムのセットを一覧表示します。このコレクションには、ユーザーのドライブにあるアイテムと、他のドライブとの間でアクセス可能なアイテムが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a6da7-p102">List a set of items that have been recently used by the signed in user. This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6da7-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a6da7-107">Permissions</span></span>

<span data-ttu-id="a6da7-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6da7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6da7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a6da7-110">Permission type</span></span>      | <span data-ttu-id="a6da7-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a6da7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6da7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a6da7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a6da7-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6da7-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a6da7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a6da7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6da7-115">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6da7-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a6da7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a6da7-116">Application</span></span> | <span data-ttu-id="a6da7-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6da7-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6da7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a6da7-118">HTTP request</span></span>

<!-- { "blockType": "request",
       "name": "view-recent-files", 
       "scopes": "files.read",
       "target": "action" } -->

```http
GET /me/drive/recent
```

## <a name="response"></a><span data-ttu-id="a6da7-119">応答</span><span class="sxs-lookup"><span data-stu-id="a6da7-119">Response</span></span>

<span data-ttu-id="a6da7-120">このメソッドは、ドライブの所有者が最近アクセスしたアイテムの [DriveItem](../resources/driveitem.md) リソースのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a6da7-120">This method returns a collection of [DriveItem](../resources/driveitem.md) resources for items which the owner of the drive has recently accessed.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="a6da7-121">備考</span><span class="sxs-lookup"><span data-stu-id="a6da7-121">Remarks</span></span>

<span data-ttu-id="a6da7-p104">**recent** アクションから返された DriveItems の中には、それらが異なるドライブからのアイテムであることを示す **remoteItem** ファセットが含まれるものがあります。元の DriveItem オブジェクトにアクセスするには、**remoteItem** で提供された情報を使用して、以下に示す書式で要求を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a6da7-p104">Some driveItems returned from the **recent** action will include the **remoteItem** facet which indicates they are items from another drive. To access the original driveItem object, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

<!-- { "blockType": "ignored", "name": "drives-get-remoteitem" } -->

```http
GET /drives/{remoteItem-driveId}/items/{remoteItem-id}
```

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve a list of recently used files for the owner of the drive.",
  "keywords": "drive,onedrive.drive,default drive",
  "section": "documentation",
  "tocPath": "Drives/Recent files"
} -->
