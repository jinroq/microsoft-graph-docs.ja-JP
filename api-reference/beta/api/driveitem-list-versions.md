---
title: DriveItem のバージョンを一覧表示
description: OneDrive と SharePoint は、ファイルの履歴を保持するように構成できます。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b51982c9aff9f8be8c801b6f0e0fc16e9ff47852
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518472"
---
# <a name="listing-versions-of-a-driveitem"></a><span data-ttu-id="b15a9-103">DriveItem のバージョンを一覧表示</span><span class="sxs-lookup"><span data-stu-id="b15a9-103">Listing versions of a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b15a9-104">OneDrive と SharePoint は、ファイルの履歴を保持するように構成できます。</span><span class="sxs-lookup"><span data-stu-id="b15a9-104">OneDrive and SharePoint can be configured to retain the history for files.</span></span>
<span data-ttu-id="b15a9-105">サービスと構成に応じて、各編集に対する新しいバージョンを作成することができます。ファイルが保存されるたびに作成するか、手動で作成するか、または全く作成しないこともできます。</span><span class="sxs-lookup"><span data-stu-id="b15a9-105">Depending on the service and configuration, a new version can be created for each edit, each time the file is saved, manually, or never.</span></span>

<span data-ttu-id="b15a9-106">ドキュメントの旧バージョンは、ユーザーまたは場所ごとに固有の場合がある管理者設定に応じて、一定期間保持することができます。</span><span class="sxs-lookup"><span data-stu-id="b15a9-106">Previous versions of a document may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="b15a9-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b15a9-107">Permissions</span></span>

<span data-ttu-id="b15a9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b15a9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b15a9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b15a9-110">Permission type</span></span>      | <span data-ttu-id="b15a9-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b15a9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b15a9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b15a9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b15a9-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b15a9-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b15a9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b15a9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b15a9-115">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b15a9-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="b15a9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b15a9-116">Application</span></span> | <span data-ttu-id="b15a9-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b15a9-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="b15a9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b15a9-118">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions
GET /groups/{group-id}/drive/{item-id}/versions
GET /me/drive/items/{item-id}/versions
GET /sites/{site-id}/drive/items/{item-id}/versions
GET /users/{user-id}/drive/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="b15a9-119">応答</span><span class="sxs-lookup"><span data-stu-id="b15a9-119">Response</span></span>

<span data-ttu-id="b15a9-120">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [DriveItemVersion](../resources/driveitemversion.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b15a9-120">If successful, this method returns a `200 OK` response code and collection of [DriveItemVersion](../resources/driveitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="b15a9-121">例</span><span class="sxs-lookup"><span data-stu-id="b15a9-121">Example</span></span>

<span data-ttu-id="b15a9-122">この例では、現在のユーザーのドライブ内のファイルのそのバージョンを取得します。</span><span class="sxs-lookup"><span data-stu-id="b15a9-122">This example retrieves the versions of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="b15a9-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b15a9-123">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="b15a9-124">応答</span><span class="sxs-lookup"><span data-stu-id="b15a9-124">Response</span></span>

<span data-ttu-id="b15a9-125">バージョンのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b15a9-125">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItemVersion)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value":
  [
    {
      "id": "3.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
      "size": 123
    },
    {
      "id": "2.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-11T10:21:03.000Z",
      "size": 62
    },
    {
      "id": "1.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-10T15:20:01.125Z",
      "size": 16
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="b15a9-126">備考</span><span class="sxs-lookup"><span data-stu-id="b15a9-126">Remarks</span></span>

<span data-ttu-id="b15a9-127">OneDrive は、ファイルの旧バージョンの完全なメタデータを保持しません。</span><span class="sxs-lookup"><span data-stu-id="b15a9-127">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="b15a9-128">アプリがファイルの利用可能なバージョンのリストを取得すると、[DriveItemVersion](../resources/driveitemversion.md) リソースが返され、特定のバージョンに関する利用可能な情報が提供されます。</span><span class="sxs-lookup"><span data-stu-id="b15a9-128">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-list-versions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
