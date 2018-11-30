---
title: DriveItem のバージョンを一覧表示
description: OneDrive と SharePoint は、ファイルの履歴を保持するように構成できます。
ms.openlocfilehash: a0092fa244543fbc2233cd9de20ecebd2938fd79
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069220"
---
# <a name="listing-versions-of-a-driveitem"></a><span data-ttu-id="83b2a-103">DriveItem のバージョンを一覧表示</span><span class="sxs-lookup"><span data-stu-id="83b2a-103">Listing versions of a DriveItem</span></span>

> <span data-ttu-id="83b2a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="83b2a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="83b2a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83b2a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="83b2a-106">OneDrive と SharePoint は、ファイルの履歴を保持するように構成できます。</span><span class="sxs-lookup"><span data-stu-id="83b2a-106">OneDrive and SharePoint can be configured to retain the history for files.</span></span>
<span data-ttu-id="83b2a-107">サービスと構成に応じて、各編集に対する新しいバージョンを作成することができます。ファイルが保存されるたびに作成するか、手動で作成するか、または全く作成しないこともできます。</span><span class="sxs-lookup"><span data-stu-id="83b2a-107">Depending on the service and configuration, a new version can be created for each edit, each time the file is saved, manually, or never.</span></span>

<span data-ttu-id="83b2a-108">ドキュメントの旧バージョンは、ユーザーまたは場所ごとに固有の場合がある管理者設定に応じて、一定期間保持することができます。</span><span class="sxs-lookup"><span data-stu-id="83b2a-108">Previous versions of a document may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="83b2a-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="83b2a-109">Permissions</span></span>

<span data-ttu-id="83b2a-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="83b2a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83b2a-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="83b2a-112">Permission type</span></span>      | <span data-ttu-id="83b2a-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="83b2a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83b2a-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="83b2a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="83b2a-115">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83b2a-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="83b2a-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="83b2a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83b2a-117">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83b2a-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="83b2a-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="83b2a-118">Application</span></span> | <span data-ttu-id="83b2a-119">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83b2a-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="83b2a-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="83b2a-120">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions
GET /groups/{group-id}/drive/{item-id}/versions
GET /me/drive/items/{item-id}/versions
GET /sites/{site-id}/drive/items/{item-id}/versions
GET /users/{user-id}/drive/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="83b2a-121">応答</span><span class="sxs-lookup"><span data-stu-id="83b2a-121">Response</span></span>

<span data-ttu-id="83b2a-122">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [DriveItemVersion](../resources/driveitemversion.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="83b2a-122">If successful, this method returns a `200 OK` response code and collection of [DriveItemVersion](../resources/driveitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="83b2a-123">例</span><span class="sxs-lookup"><span data-stu-id="83b2a-123">Example</span></span>

<span data-ttu-id="83b2a-124">この例では、現在のユーザーのドライブ内のファイルのそのバージョンを取得します。</span><span class="sxs-lookup"><span data-stu-id="83b2a-124">This example retrieves the versions of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="83b2a-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="83b2a-125">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="83b2a-126">応答</span><span class="sxs-lookup"><span data-stu-id="83b2a-126">Response</span></span>

<span data-ttu-id="83b2a-127">バージョンのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="83b2a-127">This returns a collection of versions:</span></span>

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

## <a name="remarks"></a><span data-ttu-id="83b2a-128">備考</span><span class="sxs-lookup"><span data-stu-id="83b2a-128">Remarks</span></span>

<span data-ttu-id="83b2a-129">OneDrive は、ファイルの旧バージョンの完全なメタデータを保持しません。</span><span class="sxs-lookup"><span data-stu-id="83b2a-129">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="83b2a-130">アプリがファイルの利用可能なバージョンのリストを取得すると、[DriveItemVersion](../resources/driveitemversion.md) リソースが返され、特定のバージョンに関する利用可能な情報が提供されます。</span><span class="sxs-lookup"><span data-stu-id="83b2a-130">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
