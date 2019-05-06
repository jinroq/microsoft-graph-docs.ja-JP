---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 共有アイテムのファイルの表示
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 59b626acefc125870412b5c43507fc4e476762d6
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33589852"
---
# <a name="list-items-shared-with-the-signed-in-user"></a><span data-ttu-id="7591f-102">サインイン ユーザーと共有しているアイテムを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7591f-102">List items shared with the signed-in user</span></span>

<span data-ttu-id="7591f-103">[ドライブ](../resources/drive.md) の所有者と共有されている、[DriveItem](../resources/driveitem.md) リソースのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="7591f-103">Retrieve a collection of [DriveItem](../resources/driveitem.md) resources that have been shared with the owner of the [Drive](../resources/drive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7591f-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7591f-104">Permissions</span></span>

<span data-ttu-id="7591f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7591f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7591f-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7591f-107">Permission type</span></span>      | <span data-ttu-id="7591f-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7591f-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7591f-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7591f-109">Delegated (work or school account)</span></span> | <span data-ttu-id="7591f-110">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7591f-110">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7591f-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7591f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7591f-112">Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7591f-112">Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="7591f-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7591f-113">Application</span></span> | <span data-ttu-id="7591f-114">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7591f-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

<span data-ttu-id="7591f-115">**注:** Files.Read または Files.ReadWrite のアクセス許可による /sharedWithMe 要求は成功しますが、いくつかのプロパティが失われている可能性があります。</span><span class="sxs-lookup"><span data-stu-id="7591f-115">**Note:** while the /sharedWithMe request will succeed with Files.Read or Files.ReadWrite permissions, some properties may be missing.</span></span>
<span data-ttu-id="7591f-116">さらに、**すべて**のアクセス許可のうちの一つがなければ、この API から返された共有項目はアクセスできません。</span><span class="sxs-lookup"><span data-stu-id="7591f-116">Additionally, without one of the  **All** permissions, shared items returned from this API will not be accessible.</span></span>

## <a name="http-request"></a><span data-ttu-id="7591f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7591f-117">HTTP request</span></span>

<!-- { "blockType": "request", "name": "shared-with-me", "scopes": "files.read", "tags": "service.graph", "target": "action" } -->

```http
GET /me/drive/sharedWithMe
```

## <a name="response"></a><span data-ttu-id="7591f-118">応答</span><span class="sxs-lookup"><span data-stu-id="7591f-118">Response</span></span>

<span data-ttu-id="7591f-p103">これは、ドライブの所有者を共有している DriveItem リソースを含む、[DriveItem](../resources/driveitem.md) リソースのコレクションを返します。この例では、ドライブはユーザーの既定のドライブです。そのため、これはサインインしているユーザーと共有しているアイテムを返します。</span><span class="sxs-lookup"><span data-stu-id="7591f-p103">This returns a collection of [DriveItem](../resources/driveitem.md) resources which contain the DriveItem resources shared with the owner of the drive. In this example, since the drive is the user's default drive, this returns items shared with the signed in user.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7591f-121">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="7591f-121">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7591f-122">Visual</span><span class="sxs-lookup"><span data-stu-id="7591f-122">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/shared-with-me-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7591f-123">Java</span><span class="sxs-lookup"><span data-stu-id="7591f-123">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/shared-with-me-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="7591f-124">注釈</span><span class="sxs-lookup"><span data-stu-id="7591f-124">Remarks</span></span>

<span data-ttu-id="7591f-p104">**sharedWithMe** アクションから返された DriveItems には、それらが異なるドライブからのアイテムであることを示す [**remoteItem**](../resources/remoteitem.md) ファセットが必ず含まれます。共有された DriveItem リソースにアクセスするには、**remoteItem** で提供された情報を使用して、以下に示す書式で要求を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7591f-p104">DriveItems returned from the **sharedWithMe** action will always include the [**remoteItem**](../resources/remoteitem.md) facet which indicates they are items from a different drive. To access the shared DriveItem resource, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

<!-- { "blockType": "ignored", "name": "drives-get-remoteitem" } -->

```http
GET /drives/{remoteItem-driveId}/items/{remoteItem-id}
```

<!-- {
  "type": "#page.annotation",
  "description": "List the items shared with the owner of a drive.",
  "keywords": "drive,onedrive.drive,default drive",
  "section": "documentation",
  "tocPath": "Sharing/Shared with me",
  "suppressions": [
    "Error: /api-reference/v1.0/api/drive-sharedwithme.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-sharedwithme.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
