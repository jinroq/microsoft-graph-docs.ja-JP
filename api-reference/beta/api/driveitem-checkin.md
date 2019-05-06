---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ファイルをチェックインする
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 982a581d44e39e6ddcc7bb3a52da64cd2a2eaf55
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33589365"
---
# <a name="check-in-changes-to-a-driveitem-resource"></a><span data-ttu-id="59dde-102">DriveItem リソースへの変更をチェックインする</span><span class="sxs-lookup"><span data-stu-id="59dde-102">Check-in changes to a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59dde-103">チェックアウトされた DriveItem リソースをチェックインします。これにより、他のユーザーがドキュメントのバージョンを利用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="59dde-103">Check-in a checked out DriveItem resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="59dde-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="59dde-104">Permissions</span></span>

<span data-ttu-id="59dde-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="59dde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59dde-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="59dde-107">Permission type</span></span>      | <span data-ttu-id="59dde-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="59dde-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59dde-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="59dde-109">Delegated (work or school account)</span></span> | <span data-ttu-id="59dde-110">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59dde-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="59dde-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="59dde-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59dde-112">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59dde-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="59dde-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="59dde-113">Application</span></span> | <span data-ttu-id="59dde-114">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59dde-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="59dde-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="59dde-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

### <a name="request-body"></a><span data-ttu-id="59dde-116">要求本文</span><span class="sxs-lookup"><span data-stu-id="59dde-116">Request body</span></span>

<span data-ttu-id="59dde-117">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="59dde-117">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="59dde-118">名前</span><span class="sxs-lookup"><span data-stu-id="59dde-118">Name</span></span>    | <span data-ttu-id="59dde-119">値</span><span class="sxs-lookup"><span data-stu-id="59dde-119">Value</span></span>  |                                                <span data-ttu-id="59dde-120">説明</span><span class="sxs-lookup"><span data-stu-id="59dde-120">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="59dde-121">checkInAs</span><span class="sxs-lookup"><span data-stu-id="59dde-121">checkInAs</span></span> | <span data-ttu-id="59dde-122">string</span><span class="sxs-lookup"><span data-stu-id="59dde-122">string</span></span> | <span data-ttu-id="59dde-123">省略可能。</span><span class="sxs-lookup"><span data-stu-id="59dde-123">Optional.</span></span> <span data-ttu-id="59dde-124">チェックイン操作が完了した後のドキュメントの適切なステータス。</span><span class="sxs-lookup"><span data-stu-id="59dde-124">The desired status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="59dde-125">`published` または未設定となります。</span><span class="sxs-lookup"><span data-stu-id="59dde-125">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="59dde-126">comment</span><span class="sxs-lookup"><span data-stu-id="59dde-126">comment</span></span>   | <span data-ttu-id="59dde-127">string</span><span class="sxs-lookup"><span data-stu-id="59dde-127">string</span></span> | <span data-ttu-id="59dde-128">バージョンに関連付けられているチェックイン コメント。</span><span class="sxs-lookup"><span data-stu-id="59dde-128">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="example"></a><span data-ttu-id="59dde-129">例</span><span class="sxs-lookup"><span data-stu-id="59dde-129">Example</span></span>

<span data-ttu-id="59dde-130">この例では、`{item-id}` で識別されるファイルをチェックインします。</span><span class="sxs-lookup"><span data-stu-id="59dde-130">This example checks in a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```

## <a name="response"></a><span data-ttu-id="59dde-131">応答</span><span class="sxs-lookup"><span data-stu-id="59dde-131">Response</span></span>

<span data-ttu-id="59dde-132">成功すると、API 呼び出しは `204 No content` を返します。</span><span class="sxs-lookup"><span data-stu-id="59dde-132">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="59dde-133">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="59dde-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="59dde-134">Visual</span><span class="sxs-lookup"><span data-stu-id="59dde-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/checkin-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="59dde-135">Java</span><span class="sxs-lookup"><span data-stu-id="59dde-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/checkin-item-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="remarks"></a><span data-ttu-id="59dde-136">備考</span><span class="sxs-lookup"><span data-stu-id="59dde-136">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-checkin.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-checkin.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
