---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 前のバージョンを復元する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 74ac8e9913b1d199d9baa019de6ea32b38e3654f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454294"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="dc0c2-102">DriveItem の旧バージョンを復元する</span><span class="sxs-lookup"><span data-stu-id="dc0c2-102">Restore a previous version of a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc0c2-103">DriveItem の旧バージョンを現在のバージョンに復元します。</span><span class="sxs-lookup"><span data-stu-id="dc0c2-103">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="dc0c2-104">旧バージョンのコンテンツを持つ新しいバージョンを作成します。しかし、ファイルの既存のバージョンはすべて保持されます。</span><span class="sxs-lookup"><span data-stu-id="dc0c2-104">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc0c2-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dc0c2-105">Permissions</span></span>

<span data-ttu-id="dc0c2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dc0c2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc0c2-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dc0c2-108">Permission type</span></span>      | <span data-ttu-id="dc0c2-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dc0c2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc0c2-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dc0c2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dc0c2-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc0c2-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="dc0c2-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dc0c2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc0c2-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc0c2-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="dc0c2-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dc0c2-114">Application</span></span> | <span data-ttu-id="dc0c2-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc0c2-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc0c2-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dc0c2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="dc0c2-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="dc0c2-117">Request body</span></span>

<span data-ttu-id="dc0c2-118">要求の本文は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="dc0c2-118">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="dc0c2-119">例</span><span class="sxs-lookup"><span data-stu-id="dc0c2-119">Example</span></span>

<span data-ttu-id="dc0c2-120">この例では、`{item-id}` と `{version-id}` で指定されたファイルのバージョンを復元します。</span><span class="sxs-lookup"><span data-stu-id="dc0c2-120">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="dc0c2-121">応答</span><span class="sxs-lookup"><span data-stu-id="dc0c2-121">Response</span></span>

<span data-ttu-id="dc0c2-122">成功すると、API 呼び出しは `204 No content` を返します。</span><span class="sxs-lookup"><span data-stu-id="dc0c2-122">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitemversion-restore.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
