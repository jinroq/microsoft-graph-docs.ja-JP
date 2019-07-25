---
title: ドライブ項目のバージョンを一覧表示する
description: OneDrive と SharePoint は、ファイルの履歴を保持するように構成できます。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1b3e703b5214db47467f6bd9117201e34e1eae6e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861010"
---
# <a name="listing-versions-of-a-driveitem"></a><span data-ttu-id="3bf0e-103">ドライブ項目のバージョンを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="3bf0e-103">Listing versions of a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bf0e-104">OneDrive と SharePoint は、ファイルの履歴を保持するように構成できます。</span><span class="sxs-lookup"><span data-stu-id="3bf0e-104">OneDrive and SharePoint can be configured to retain the history for files.</span></span>
<span data-ttu-id="3bf0e-105">サービスと構成に応じて、各編集に対する新しいバージョンを作成することができます。ファイルが保存されるたびに作成するか、手動で作成するか、または全く作成しないこともできます。</span><span class="sxs-lookup"><span data-stu-id="3bf0e-105">Depending on the service and configuration, a new version can be created for each edit, each time the file is saved, manually, or never.</span></span>

<span data-ttu-id="3bf0e-106">ドキュメントの旧バージョンは、ユーザーまたは場所ごとに固有の場合がある管理者設定に応じて、一定期間保持することができます。</span><span class="sxs-lookup"><span data-stu-id="3bf0e-106">Previous versions of a document may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="3bf0e-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3bf0e-107">Permissions</span></span>

<span data-ttu-id="3bf0e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3bf0e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bf0e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3bf0e-110">Permission type</span></span>      | <span data-ttu-id="3bf0e-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3bf0e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3bf0e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3bf0e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3bf0e-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bf0e-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3bf0e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3bf0e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3bf0e-115">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bf0e-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="3bf0e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3bf0e-116">Application</span></span> | <span data-ttu-id="3bf0e-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bf0e-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="3bf0e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3bf0e-118">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions
GET /groups/{group-id}/drive/{item-id}/versions
GET /me/drive/items/{item-id}/versions
GET /sites/{site-id}/drive/items/{item-id}/versions
GET /users/{user-id}/drive/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="3bf0e-119">応答</span><span class="sxs-lookup"><span data-stu-id="3bf0e-119">Response</span></span>

<span data-ttu-id="3bf0e-120">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [DriveItemVersion](../resources/driveitemversion.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="3bf0e-120">If successful, this method returns a `200 OK` response code and collection of [DriveItemVersion](../resources/driveitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="3bf0e-121">例</span><span class="sxs-lookup"><span data-stu-id="3bf0e-121">Example</span></span>

<span data-ttu-id="3bf0e-122">この例では、現在のユーザーのドライブ内のファイルのそのバージョンを取得します。</span><span class="sxs-lookup"><span data-stu-id="3bf0e-122">This example retrieves the versions of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="3bf0e-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3bf0e-123">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3bf0e-124">プロトコル</span><span class="sxs-lookup"><span data-stu-id="3bf0e-124">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-previous-versions", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/versions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3bf0e-125">C#</span><span class="sxs-lookup"><span data-stu-id="3bf0e-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-previous-versions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3bf0e-126">Javascript</span><span class="sxs-lookup"><span data-stu-id="3bf0e-126">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-previous-versions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3bf0e-127">目的-C</span><span class="sxs-lookup"><span data-stu-id="3bf0e-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-previous-versions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3bf0e-128">Java</span><span class="sxs-lookup"><span data-stu-id="3bf0e-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-previous-versions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3bf0e-129">応答</span><span class="sxs-lookup"><span data-stu-id="3bf0e-129">Response</span></span>

<span data-ttu-id="3bf0e-130">バージョンのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="3bf0e-130">This returns a collection of versions:</span></span>

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

## <a name="remarks"></a><span data-ttu-id="3bf0e-131">備考</span><span class="sxs-lookup"><span data-stu-id="3bf0e-131">Remarks</span></span>

<span data-ttu-id="3bf0e-132">OneDrive は、ファイルの旧バージョンの完全なメタデータを保持しません。</span><span class="sxs-lookup"><span data-stu-id="3bf0e-132">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="3bf0e-133">アプリがファイルの利用可能なバージョンのリストを取得すると、[DriveItemVersion](../resources/driveitemversion.md) リソースが返され、特定のバージョンに関する利用可能な情報が提供されます。</span><span class="sxs-lookup"><span data-stu-id="3bf0e-133">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
  ]
}
-->
