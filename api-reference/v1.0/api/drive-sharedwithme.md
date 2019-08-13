---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 共有アイテムのファイルの表示
localization_priority: Priority
ms.prod: sharepoint
description: ドライブの所有者と共有されている、DriveItem リソースのコレクションを取得します。
doc_type: apiPageType
ms.openlocfilehash: ca78c3b618a0c323687dd1e38690a600aa9516fe
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36375157"
---
# <a name="list-items-shared-with-the-signed-in-user"></a><span data-ttu-id="fe65c-103">サインイン ユーザーと共有しているアイテムを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="fe65c-103">List items shared with the signed-in user</span></span>

<span data-ttu-id="fe65c-104">[ドライブ](../resources/drive.md) の所有者と共有されている、[DriveItem](../resources/driveitem.md) リソースのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="fe65c-104">Retrieve a collection of [DriveItem](../resources/driveitem.md) resources that have been shared with the owner of the [Drive](../resources/drive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fe65c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fe65c-105">Permissions</span></span>

<span data-ttu-id="fe65c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe65c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe65c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fe65c-108">Permission type</span></span>      | <span data-ttu-id="fe65c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fe65c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe65c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fe65c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fe65c-111">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe65c-111">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="fe65c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fe65c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe65c-113">Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe65c-113">Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="fe65c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fe65c-114">Application</span></span> | <span data-ttu-id="fe65c-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe65c-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

<span data-ttu-id="fe65c-116">**注:** Files.Read または Files.ReadWrite のアクセス許可による /sharedWithMe 要求は成功しますが、いくつかのプロパティが失われている可能性があります。</span><span class="sxs-lookup"><span data-stu-id="fe65c-116">**Note:** while the /sharedWithMe request will succeed with Files.Read or Files.ReadWrite permissions, some properties may be missing.</span></span>
<span data-ttu-id="fe65c-117">さらに、**すべて**のアクセス許可のうちの一つがなければ、この API から返された共有項目はアクセスできません。</span><span class="sxs-lookup"><span data-stu-id="fe65c-117">Additionally, without one of the  **All** permissions, shared items returned from this API will not be accessible.</span></span>

## <a name="http-request"></a><span data-ttu-id="fe65c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fe65c-118">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fe65c-119">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe65c-119">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "shared-with-me", "scopes": "files.read", "tags": "service.graph", "target": "action" } -->

```http
GET /me/drive/sharedWithMe
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fe65c-120">C#</span><span class="sxs-lookup"><span data-stu-id="fe65c-120">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shared-with-me-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fe65c-121">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe65c-121">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shared-with-me-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fe65c-122">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe65c-122">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shared-with-me-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fe65c-123">Java</span><span class="sxs-lookup"><span data-stu-id="fe65c-123">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shared-with-me-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="fe65c-124">応答</span><span class="sxs-lookup"><span data-stu-id="fe65c-124">Response</span></span>

<span data-ttu-id="fe65c-p103">これは、ドライブの所有者を共有している DriveItem リソースを含む、[DriveItem](../resources/driveitem.md) リソースのコレクションを返します。この例では、ドライブはユーザーの既定のドライブです。そのため、これはサインインしているユーザーと共有しているアイテムを返します。</span><span class="sxs-lookup"><span data-stu-id="fe65c-p103">This returns a collection of [DriveItem](../resources/driveitem.md) resources which contain the DriveItem resources shared with the owner of the drive. In this example, since the drive is the user's default drive, this returns items shared with the signed in user.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="fe65c-127">注釈</span><span class="sxs-lookup"><span data-stu-id="fe65c-127">Remarks</span></span>

<span data-ttu-id="fe65c-p104">**sharedWithMe** アクションから返された DriveItems には、それらが異なるドライブからのアイテムであることを示す [**remoteItem**](../resources/remoteitem.md) ファセットが必ず含まれます。共有された DriveItem リソースにアクセスするには、**remoteItem** で提供された情報を使用して、以下に示す書式で要求を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="fe65c-p104">DriveItems returned from the **sharedWithMe** action will always include the [**remoteItem**](../resources/remoteitem.md) facet which indicates they are items from a different drive. To access the shared DriveItem resource, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

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
  ]
} -->
