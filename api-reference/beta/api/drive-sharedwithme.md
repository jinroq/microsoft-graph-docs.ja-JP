---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 自分と共有されるファイルを一覧表示する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 06c6607de9fa36fd8b1dedc3bf5ded3cfad1228e
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481014"
---
# <a name="list-items-shared-with-the-signed-in-user"></a><span data-ttu-id="691a4-102">サインイン ユーザーと共有しているアイテムを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="691a4-102">List items shared with the signed-in user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="691a4-103">[ドライブ](../resources/drive.md) の所有者と共有されている、[DriveItem](../resources/driveitem.md) リソースのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="691a4-103">Retrieve a collection of [DriveItem](../resources/driveitem.md) resources that have been shared with the owner of the [Drive](../resources/drive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="691a4-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="691a4-104">Permissions</span></span>

<span data-ttu-id="691a4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="691a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="691a4-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="691a4-107">Permission type</span></span>      | <span data-ttu-id="691a4-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="691a4-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="691a4-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="691a4-109">Delegated (work or school account)</span></span> | <span data-ttu-id="691a4-110">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="691a4-110">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="691a4-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="691a4-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="691a4-112">Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="691a4-112">Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="691a4-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="691a4-113">Application</span></span> | <span data-ttu-id="691a4-114">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="691a4-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

<span data-ttu-id="691a4-115">**注:** /sharedwithme 要求は、ファイルを使用して正常に終了します。読み取りまたは書き込みのアクセス許可がありません。一部のプロパティが不足している可能性があります。</span><span class="sxs-lookup"><span data-stu-id="691a4-115">**Note:** while the /sharedWithMe request will succeed with Files.Read or Files.ReadWrite permissions, some properties may be missing.</span></span>
<span data-ttu-id="691a4-116">さらに、**すべて**のアクセス許可のうちの一つがなければ、この API から返された共有項目はアクセスできません。</span><span class="sxs-lookup"><span data-stu-id="691a4-116">Additionally, without one of the  **All** permissions, shared items returned from this API will not be accessible.</span></span>

## <a name="http-request"></a><span data-ttu-id="691a4-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="691a4-117">HTTP request</span></span>

<!-- { "blockType": "request", "name": "shared-with-me", "scopes": "files.read", "target": "action" } -->

```http
GET /me/drive/sharedWithMe
```

## <a name="response"></a><span data-ttu-id="691a4-118">応答</span><span class="sxs-lookup"><span data-stu-id="691a4-118">Response</span></span>

<span data-ttu-id="691a4-p103">これは、ドライブの所有者を共有している DriveItem リソースを含む、[DriveItem](../resources/driveitem.md) リソースのコレクションを返します。この例では、ドライブはユーザーの既定のドライブです。そのため、これはサインインしているユーザーと共有しているアイテムを返します。</span><span class="sxs-lookup"><span data-stu-id="691a4-p103">This returns a collection of [DriveItem](../resources/driveitem.md) resources which contain the DriveItem resources shared with the owner of the drive. In this example, since the drive is the user's default drive, this returns items shared with the signed in user.</span></span>

<!-- {"blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1312abc",
      "remoteItem": {
        "id": "1991210caf!192",
        "name": "March Proposal.docx",
        "file": { },
        "size": 19121,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      }
    },
    {
      "id": "1312def",
      "remoteItem": {
        "id": "1991210caf!1991",
        "name": "Team Roster.xlsx",
        "file": { },
        "size": 37619,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="691a4-121">注釈</span><span class="sxs-lookup"><span data-stu-id="691a4-121">Remarks</span></span>

<span data-ttu-id="691a4-p104">**sharedWithMe** アクションから返された DriveItems には、それらが異なるドライブからのアイテムであることを示す [**remoteItem**](../resources/remoteitem.md) ファセットが必ず含まれます。共有された DriveItem リソースにアクセスするには、**remoteItem** で提供された情報を使用して、以下に示す書式で要求を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="691a4-p104">DriveItems returned from the **sharedWithMe** action will always include the [**remoteItem**](../resources/remoteitem.md) facet which indicates they are items from a different drive. To access the shared DriveItem resource, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

<!-- { "blockType": "ignored", "name": "drives-get-remoteitem" } -->

```http
GET /drives/{remoteItem-driveId}/items/{remoteItem-id}
```

<!--
{
  "type": "#page.annotation",
  "description": "List the items shared with the owner of a drive.",
  "keywords": "drive,onedrive.drive,default drive",
  "section": "documentation",
  "tocPath": "Sharing/Shared with me",
  "suppressions": [
    "Error: /api-reference/beta/api/drive-sharedwithme.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
