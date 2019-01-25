---
author: chackman
ms.author: chackman
title: ドライブ項目のフォローを取り消します
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 064ab2d5ad86df5341a0f2f5a46fe7c227ff35fb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513110"
---
# <a name="unfollow-drive-item"></a><span data-ttu-id="86884-102">ドライブ項目のフォローを取り消します</span><span class="sxs-lookup"><span data-stu-id="86884-102">Unfollow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86884-103">[DriveItem](../resources/driveitem.md)のフォローを取り消します。</span><span class="sxs-lookup"><span data-stu-id="86884-103">Unfollow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="86884-104">**注:** 以下の項目には、[以下の項目](driveitem-follow.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="86884-104">**Note:** To follow an item, see [Follow Item](driveitem-follow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="86884-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="86884-105">Permissions</span></span>

<span data-ttu-id="86884-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="86884-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86884-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="86884-108">Permission type</span></span>      | <span data-ttu-id="86884-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="86884-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86884-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="86884-110">Delegated (work or school account)</span></span> | <span data-ttu-id="86884-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86884-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="86884-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="86884-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86884-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86884-113">Not supported.</span></span>    |
|<span data-ttu-id="86884-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="86884-114">Application</span></span> | <span data-ttu-id="86884-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86884-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="86884-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="86884-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/drive/following/{item-id} 
DELETE /users/{user-id}/drive/following/{item-id}
```

## <a name="request-body"></a><span data-ttu-id="86884-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="86884-117">Request body</span></span>

<span data-ttu-id="86884-118">要求の本文は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="86884-118">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="86884-119">応答</span><span class="sxs-lookup"><span data-stu-id="86884-119">Response</span></span>

<span data-ttu-id="86884-120">成功すると、API 呼び出しは `204 No Content` を返します。</span><span class="sxs-lookup"><span data-stu-id="86884-120">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="86884-121">例</span><span class="sxs-lookup"><span data-stu-id="86884-121">Example</span></span>

<span data-ttu-id="86884-122">次の使用例で識別される項目を unfollows `{item-id}`。</span><span class="sxs-lookup"><span data-stu-id="86884-122">This example unfollows an item identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "unfollow-item", "scopes": "files.read" } -->

```http
DELETE /me/drive/following/{item-id}
```


<!--
{
  "type": "#page.annotation",
  "description": "Unfollow an item that the user is following.",
  "keywords": "unfollow item",
  "section": "documentation",
  "tocPath": "Items/Unfollow",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-unfollow.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
