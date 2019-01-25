---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ファイルをチェックインします。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ccb4a6dee07cd324a89a7f192b0fe1bb5aaa2e53
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529888"
---
# <a name="check-in-changes-to-a-driveitem-resource"></a><span data-ttu-id="98db4-102">DriveItem リソースへの変更をチェックインする</span><span class="sxs-lookup"><span data-stu-id="98db4-102">Check-in changes to a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98db4-103">チェックアウトされた DriveItem リソースをチェックインします。これにより、他のユーザーがドキュメントのバージョンを利用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="98db4-103">Check-in a checked out DriveItem resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="98db4-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="98db4-104">Permissions</span></span>

<span data-ttu-id="98db4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="98db4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98db4-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="98db4-107">Permission type</span></span>      | <span data-ttu-id="98db4-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="98db4-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98db4-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="98db4-109">Delegated (work or school account)</span></span> | <span data-ttu-id="98db4-110">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98db4-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="98db4-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="98db4-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98db4-112">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98db4-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="98db4-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="98db4-113">Application</span></span> | <span data-ttu-id="98db4-114">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98db4-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="98db4-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="98db4-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

### <a name="request-body"></a><span data-ttu-id="98db4-116">要求本文</span><span class="sxs-lookup"><span data-stu-id="98db4-116">Request body</span></span>

<span data-ttu-id="98db4-117">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="98db4-117">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="98db4-118">名前</span><span class="sxs-lookup"><span data-stu-id="98db4-118">Name</span></span>    | <span data-ttu-id="98db4-119">値</span><span class="sxs-lookup"><span data-stu-id="98db4-119">Value</span></span>  |                                                <span data-ttu-id="98db4-120">説明</span><span class="sxs-lookup"><span data-stu-id="98db4-120">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="98db4-121">checkInAs</span><span class="sxs-lookup"><span data-stu-id="98db4-121">checkInAs</span></span> | <span data-ttu-id="98db4-122">string</span><span class="sxs-lookup"><span data-stu-id="98db4-122">string</span></span> | <span data-ttu-id="98db4-123">省略可能。</span><span class="sxs-lookup"><span data-stu-id="98db4-123">Optional.</span></span> <span data-ttu-id="98db4-124">チェックイン操作が完了した後のドキュメントの適切なステータス。</span><span class="sxs-lookup"><span data-stu-id="98db4-124">The desired status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="98db4-125">`published` または未設定となります。</span><span class="sxs-lookup"><span data-stu-id="98db4-125">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="98db4-126">comment</span><span class="sxs-lookup"><span data-stu-id="98db4-126">comment</span></span>   | <span data-ttu-id="98db4-127">string</span><span class="sxs-lookup"><span data-stu-id="98db4-127">string</span></span> | <span data-ttu-id="98db4-128">バージョンに関連付けられているチェックイン コメント。</span><span class="sxs-lookup"><span data-stu-id="98db4-128">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="example"></a><span data-ttu-id="98db4-129">例</span><span class="sxs-lookup"><span data-stu-id="98db4-129">Example</span></span>

<span data-ttu-id="98db4-130">この例では、`{item-id}` で識別されるファイルをチェックインします。</span><span class="sxs-lookup"><span data-stu-id="98db4-130">This example checks in a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```

## <a name="response"></a><span data-ttu-id="98db4-131">応答</span><span class="sxs-lookup"><span data-stu-id="98db4-131">Response</span></span>

<span data-ttu-id="98db4-132">成功すると、API 呼び出しは `204 No content` を返します。</span><span class="sxs-lookup"><span data-stu-id="98db4-132">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="98db4-133">備考</span><span class="sxs-lookup"><span data-stu-id="98db4-133">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-checkin.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
