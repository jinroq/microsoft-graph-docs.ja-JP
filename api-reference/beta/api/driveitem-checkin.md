---
author: JeremyKelley
description: チェックアウトされた DriveItem リソースをチェックインします。これにより、他のユーザーがドキュメントのバージョンを利用できるようになります。
ms.date: 09/10/2017
title: ファイルをチェックインする
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 4fb16edc3c38db72ffd2c33f891ed5cc3d74654d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957256"
---
# <a name="check-in-changes-to-a-driveitem-resource"></a><span data-ttu-id="feb9f-103">DriveItem リソースへの変更をチェックインする</span><span class="sxs-lookup"><span data-stu-id="feb9f-103">Check-in changes to a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="feb9f-104">チェックアウトされた DriveItem リソースをチェックインします。これにより、他のユーザーがドキュメントのバージョンを利用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="feb9f-104">Check-in a checked out DriveItem resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="feb9f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="feb9f-105">Permissions</span></span>

<span data-ttu-id="feb9f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="feb9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="feb9f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="feb9f-108">Permission type</span></span>      | <span data-ttu-id="feb9f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="feb9f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="feb9f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="feb9f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="feb9f-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="feb9f-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="feb9f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="feb9f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="feb9f-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="feb9f-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="feb9f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="feb9f-114">Application</span></span> | <span data-ttu-id="feb9f-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="feb9f-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="feb9f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="feb9f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

### <a name="request-body"></a><span data-ttu-id="feb9f-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="feb9f-117">Request body</span></span>

<span data-ttu-id="feb9f-118">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="feb9f-118">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="feb9f-119">名前</span><span class="sxs-lookup"><span data-stu-id="feb9f-119">Name</span></span>    | <span data-ttu-id="feb9f-120">値</span><span class="sxs-lookup"><span data-stu-id="feb9f-120">Value</span></span>  |                                                <span data-ttu-id="feb9f-121">説明</span><span class="sxs-lookup"><span data-stu-id="feb9f-121">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="feb9f-122">checkInAs</span><span class="sxs-lookup"><span data-stu-id="feb9f-122">checkInAs</span></span> | <span data-ttu-id="feb9f-123">string</span><span class="sxs-lookup"><span data-stu-id="feb9f-123">string</span></span> | <span data-ttu-id="feb9f-124">省略可能。</span><span class="sxs-lookup"><span data-stu-id="feb9f-124">Optional.</span></span> <span data-ttu-id="feb9f-125">チェックイン操作が完了した後のドキュメントの適切なステータス。</span><span class="sxs-lookup"><span data-stu-id="feb9f-125">The desired status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="feb9f-126">`published` または未設定となります。</span><span class="sxs-lookup"><span data-stu-id="feb9f-126">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="feb9f-127">comment</span><span class="sxs-lookup"><span data-stu-id="feb9f-127">comment</span></span>   | <span data-ttu-id="feb9f-128">string</span><span class="sxs-lookup"><span data-stu-id="feb9f-128">string</span></span> | <span data-ttu-id="feb9f-129">バージョンに関連付けられているチェックイン コメント。</span><span class="sxs-lookup"><span data-stu-id="feb9f-129">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="example"></a><span data-ttu-id="feb9f-130">例</span><span class="sxs-lookup"><span data-stu-id="feb9f-130">Example</span></span>

<span data-ttu-id="feb9f-131">この例では、`{item-id}` で識別されるファイルをチェックインします。</span><span class="sxs-lookup"><span data-stu-id="feb9f-131">This example checks in a file identified by `{item-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="feb9f-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="feb9f-132">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="feb9f-133">C#</span><span class="sxs-lookup"><span data-stu-id="feb9f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkin-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="feb9f-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="feb9f-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkin-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="feb9f-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="feb9f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkin-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="feb9f-136">Java</span><span class="sxs-lookup"><span data-stu-id="feb9f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/checkin-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="feb9f-137">応答</span><span class="sxs-lookup"><span data-stu-id="feb9f-137">Response</span></span>

<span data-ttu-id="feb9f-138">成功すると、API 呼び出しは `204 No content` を返します。</span><span class="sxs-lookup"><span data-stu-id="feb9f-138">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="feb9f-139">備考</span><span class="sxs-lookup"><span data-stu-id="feb9f-139">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
}
-->
