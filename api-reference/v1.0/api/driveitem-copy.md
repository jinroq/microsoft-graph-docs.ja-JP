---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ファイルまたはフォルダーをコピーする
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 99987dc70099e74a0d5273a40d3cb8a69af7ecdb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881803"
---
# <a name="copy-a-driveitem"></a><span data-ttu-id="5ae6f-102">DriveItem をコピーする</span><span class="sxs-lookup"><span data-stu-id="5ae6f-102">Copy a DriveItem</span></span>

<span data-ttu-id="5ae6f-103">新しい親アイテムの下に、または新しい名前を指定して、[driveItem][item-resource] (すべての子を含む) のコピーを非同期に作成します。</span><span class="sxs-lookup"><span data-stu-id="5ae6f-103">Asynchronously creates a copy of an [driveItem][item-resource] (including any children), under a new parent item or with a new name.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ae6f-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5ae6f-104">Permissions</span></span>

<span data-ttu-id="5ae6f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ae6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ae6f-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5ae6f-107">Permission type</span></span>      | <span data-ttu-id="5ae6f-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5ae6f-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ae6f-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5ae6f-109">Delegated (work or school account)</span></span> | <span data-ttu-id="5ae6f-110">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ae6f-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="5ae6f-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5ae6f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ae6f-112">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ae6f-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="5ae6f-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5ae6f-113">Application</span></span> | <span data-ttu-id="5ae6f-114">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ae6f-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ae6f-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5ae6f-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/copy
POST /groups/{groupId}/drive/items/{itemId}/copy
POST /me/drive/items/{item-id}/copy
POST /sites/{siteId}/drive/items/{itemId}/copy
POST /users/{userId}/drive/items/{itemId}/copy
```

### <a name="request-body"></a><span data-ttu-id="5ae6f-116">要求本文</span><span class="sxs-lookup"><span data-stu-id="5ae6f-116">Request body</span></span>

<span data-ttu-id="5ae6f-117">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="5ae6f-117">In the request body, provide a JSON object with the following parameters.</span></span>


| <span data-ttu-id="5ae6f-118">名前</span><span class="sxs-lookup"><span data-stu-id="5ae6f-118">Name</span></span>            | <span data-ttu-id="5ae6f-119">値</span><span class="sxs-lookup"><span data-stu-id="5ae6f-119">Value</span></span>                                          | <span data-ttu-id="5ae6f-120">説明</span><span class="sxs-lookup"><span data-stu-id="5ae6f-120">Description</span></span>                                                                                                 |
|:----------------|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="5ae6f-121">parentReference</span><span class="sxs-lookup"><span data-stu-id="5ae6f-121">parentReference</span></span> | [<span data-ttu-id="5ae6f-122">ItemReference</span><span class="sxs-lookup"><span data-stu-id="5ae6f-122">ItemReference</span></span>](../resources/itemreference.md) | <span data-ttu-id="5ae6f-p102">省略可能。コピーが作成される親アイテムへの参照。</span><span class="sxs-lookup"><span data-stu-id="5ae6f-p102">Optional. Reference to the parent item the copy will be created in.</span></span>                                         |
| <span data-ttu-id="5ae6f-125">name</span><span class="sxs-lookup"><span data-stu-id="5ae6f-125">name</span></span>            | <span data-ttu-id="5ae6f-126">string</span><span class="sxs-lookup"><span data-stu-id="5ae6f-126">string</span></span>                                         | <span data-ttu-id="5ae6f-p103">省略可能。コピーの新しい名前。これを指定しない場合は、元の名前と同じ名前が使用されます。</span><span class="sxs-lookup"><span data-stu-id="5ae6f-p103">Optional. The new name for the copy. If this isn't provided, the same name will be used as the original.</span></span>    |

<span data-ttu-id="5ae6f-130">**注:** _parentReference_ には、ターゲット フォルダーの `driveId` と `id` パラメーターを含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="5ae6f-130">**Note:** The _parentReference_ should include the `driveId` and `id` parameters for the target folder.</span></span>

## <a name="example"></a><span data-ttu-id="5ae6f-131">例</span><span class="sxs-lookup"><span data-stu-id="5ae6f-131">Example</span></span>

<span data-ttu-id="5ae6f-132">この例では、`{item-id}` で識別されるファイルを `driveId` および `id` の値で識別されるフォルダーにコピーします。</span><span class="sxs-lookup"><span data-stu-id="5ae6f-132">This example copies a file identified by `{item-id}` into a folder identified with a `driveId` and `id` value.</span></span>
<span data-ttu-id="5ae6f-133">ファイルの新しいコピーの名前は `contoso plan (copy).txt` になります。</span><span class="sxs-lookup"><span data-stu-id="5ae6f-133">The new copy of the file will be named `contoso plan (copy).txt`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5ae6f-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="5ae6f-134">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "copy-item", "scopes": "files.readwrite", "tags": "service.graph", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "driveId": "6F7D00BF-FC4D-4E62-9769-6AEA81F3A21B",
    "id": "DCD0D3AD-8989-4F23-A5A2-2C086050513F"
  },
  "name": "contoso plan (copy).txt"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5ae6f-135">C#</span><span class="sxs-lookup"><span data-stu-id="5ae6f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/copy-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5ae6f-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="5ae6f-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/copy-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5ae6f-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="5ae6f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/copy-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5ae6f-138">Java</span><span class="sxs-lookup"><span data-stu-id="5ae6f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/copy-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="5ae6f-139">応答</span><span class="sxs-lookup"><span data-stu-id="5ae6f-139">Response</span></span>

<span data-ttu-id="5ae6f-140">要求の受け入れ時に、コピーの[進行状況を監視する](/graph/long-running-actions-overview)方法についての詳細を返します。</span><span class="sxs-lookup"><span data-stu-id="5ae6f-140">Returns details about how to [monitor the progress](/graph/long-running-actions-overview) of the copy, upon accepting the request.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://contoso.sharepoint.com/_api/v2.0/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="5ae6f-p105">`Location` ヘッダーの値は、コピー操作の現在の状況を返すサービスの URL を提供します。 この情報を使用して、[コピーがいつ終了したかを判断する](/graph/long-running-actions-overview)ことができます。</span><span class="sxs-lookup"><span data-stu-id="5ae6f-p105">The value of the `Location` header provides a URL for a service that will return the current state of the copy operation. You can use this info to [determine when the copy has finished](/graph/long-running-actions-overview).</span></span>

### <a name="remarks"></a><span data-ttu-id="5ae6f-143">備考</span><span class="sxs-lookup"><span data-stu-id="5ae6f-143">Remarks</span></span>

<span data-ttu-id="5ae6f-p106">多くの場合、コピー操作は非同期で実行されます。API からの応答は、コピー操作が受け入れられたか、コピー先のファイル名が既に使用中のためという理由で拒否されたことのみを示します。</span><span class="sxs-lookup"><span data-stu-id="5ae6f-p106">In many cases the copy action is performed asynchronously. The response from the API will only indicate that the copy operation was accepted or rejected, say due to the destination filename already being in use.</span></span>

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
} -->
