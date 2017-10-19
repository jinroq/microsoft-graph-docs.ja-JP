---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "最近使用したファイルを一覧表示する"
ms.openlocfilehash: fd1b25a41369d354d18167f17b3c35e9d40bf3f4
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="list-recent-files"></a><span data-ttu-id="b1b35-102">最近使用したファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b1b35-102">List recent files</span></span>

<span data-ttu-id="b1b35-p101">サインインしたユーザーによって最近使用されたアイテムのセットを一覧表示します。このコレクションには、ユーザーのドライブにあるアイテムと、他のドライブとの間でアクセス可能なアイテムが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b1b35-p101">List a set of items that have been recently used by the signed in user. This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1b35-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b1b35-105">Permissions</span></span>

<span data-ttu-id="b1b35-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b1b35-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b1b35-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b1b35-108">Permission type</span></span>      | <span data-ttu-id="b1b35-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b1b35-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1b35-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b1b35-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b1b35-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1b35-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b1b35-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b1b35-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1b35-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1b35-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="b1b35-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b1b35-114">Application</span></span> | <span data-ttu-id="b1b35-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1b35-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1b35-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b1b35-116">HTTP request</span></span>

<!-- { "blockType": "request",
       "name": "view-recent-files", 
       "scopes": "files.read",
       "target": "action" } -->

```http
GET /me/drive/recent
```

## <a name="response"></a><span data-ttu-id="b1b35-117">応答</span><span class="sxs-lookup"><span data-stu-id="b1b35-117">Response</span></span>

<span data-ttu-id="b1b35-118">このメソッドは、ドライブの所有者が最近アクセスしたアイテムの [DriveItem](../resources/driveitem.md) リソースのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b1b35-118">This returns a collection of [DriveItem](../resources/driveitem.md) resources for items which the owner of the drive has recently accessed. Items outside of the user's drive will include the RemoteItem facet, which provides information to access the shared item.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="b1b35-119">備考</span><span class="sxs-lookup"><span data-stu-id="b1b35-119">Remarks</span></span>

<span data-ttu-id="b1b35-p103">**recent** アクションから返された DriveItems の中には、それらが異なるドライブからのアイテムであることを示す **remoteItem** ファセットが含まれるものがあります。元の DriveItem オブジェクトにアクセスするには、**remoteItem** で提供された情報を使用して、以下に示す書式で要求を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b1b35-p103">Some driveItems returned from the **recent** action will include the **remoteItem** facet which indicates they are items from another drive. To access the original driveItem object, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

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
