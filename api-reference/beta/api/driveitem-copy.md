---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ファイルまたはフォルダーをコピーする
localization_priority: Normal
ms.openlocfilehash: 8289bd3c15575e1469fe18baf45c6c2f937ed2dd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879444"
---
# <a name="copy-a-driveitem"></a><span data-ttu-id="ed9c4-102">DriveItem をコピーする</span><span class="sxs-lookup"><span data-stu-id="ed9c4-102">Copy a DriveItem</span></span>

> <span data-ttu-id="ed9c4-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ed9c4-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed9c4-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed9c4-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ed9c4-105">新しい親アイテムの下に、または新しい名前を指定して、[driveItem][item-resource] (すべての子を含む) のコピーを非同期に作成します。</span><span class="sxs-lookup"><span data-stu-id="ed9c4-105">Asynchronously creates a copy of an [driveItem][item-resource] (including any children), under a new parent item or with a new name.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed9c4-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ed9c4-106">Permissions</span></span>

<span data-ttu-id="ed9c4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ed9c4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed9c4-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ed9c4-109">Permission type</span></span>      | <span data-ttu-id="ed9c4-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ed9c4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed9c4-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ed9c4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ed9c4-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed9c4-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ed9c4-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ed9c4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed9c4-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed9c4-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ed9c4-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ed9c4-115">Application</span></span> | <span data-ttu-id="ed9c4-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed9c4-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed9c4-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ed9c4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/copy
POST /groups/{groupId}/drive/items/{itemId}/copy
POST /me/drive/items/{item-id}/copy
POST /sites/{siteId}/drive/items/{itemId}/copy
POST /users/{userId}/drive/items/{itemId}/copy
```

### <a name="request-body"></a><span data-ttu-id="ed9c4-118">要求本文</span><span class="sxs-lookup"><span data-stu-id="ed9c4-118">Request body</span></span>

<span data-ttu-id="ed9c4-119">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="ed9c4-119">In the request body, provide a JSON object with the following parameters.</span></span>


| <span data-ttu-id="ed9c4-120">名前</span><span class="sxs-lookup"><span data-stu-id="ed9c4-120">Name</span></span>            | <span data-ttu-id="ed9c4-121">値</span><span class="sxs-lookup"><span data-stu-id="ed9c4-121">Value</span></span>                                          | <span data-ttu-id="ed9c4-122">説明</span><span class="sxs-lookup"><span data-stu-id="ed9c4-122">Description</span></span>                                                                                                 |
|:----------------|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ed9c4-123">parentReference</span><span class="sxs-lookup"><span data-stu-id="ed9c4-123">parentReference</span></span> | [<span data-ttu-id="ed9c4-124">ItemReference</span><span class="sxs-lookup"><span data-stu-id="ed9c4-124">ItemReference</span></span>](../resources/itemreference.md) | <span data-ttu-id="ed9c4-p103">省略可能。コピーが作成される親アイテムへの参照。</span><span class="sxs-lookup"><span data-stu-id="ed9c4-p103">Optional. Reference to the parent item the copy will be created in.</span></span>                                         |
| <span data-ttu-id="ed9c4-127">name</span><span class="sxs-lookup"><span data-stu-id="ed9c4-127">name</span></span>            | <span data-ttu-id="ed9c4-128">文字列</span><span class="sxs-lookup"><span data-stu-id="ed9c4-128">string</span></span>                                         | <span data-ttu-id="ed9c4-p104">省略可能。コピーの新しい名前。これを指定しない場合は、元の名前と同じ名前が使用されます。</span><span class="sxs-lookup"><span data-stu-id="ed9c4-p104">Optional. The new name for the copy. If this isn't provided, the same name will be used as the original.</span></span>    |

<span data-ttu-id="ed9c4-132">**注:** _parentReference_ には、ターゲット フォルダーの `driveId` と `id` パラメーターを含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="ed9c4-132">**Note:** The _parentReference_ should include the `driveId` and `id` parameters for the target folder.</span></span>

## <a name="example"></a><span data-ttu-id="ed9c4-133">例</span><span class="sxs-lookup"><span data-stu-id="ed9c4-133">Example</span></span>

<span data-ttu-id="ed9c4-134">この例では、`{item-id}` で識別されるファイルを `driveId` および `id` の値で識別されるフォルダーにコピーします。</span><span class="sxs-lookup"><span data-stu-id="ed9c4-134">This example copies a file identified by `{item-id}` into a folder identified with a `driveId` and `id` value.</span></span>
<span data-ttu-id="ed9c4-135">ファイルの新しいコピーの名前は `contoso plan (copy).txt` になります。</span><span class="sxs-lookup"><span data-stu-id="ed9c4-135">The new copy of the file will be named `contoso plan (copy).txt`.</span></span>

<!-- { "blockType": "request", "name": "copy-item", "scopes": "files.readwrite", "target": "action" } -->

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

## <a name="response"></a><span data-ttu-id="ed9c4-136">応答</span><span class="sxs-lookup"><span data-stu-id="ed9c4-136">Response</span></span>

<span data-ttu-id="ed9c4-137">要求の受け入れ時に、コピーの[進行状況を監視する](/graph/long-running-actions-overview)方法についての詳細を返します。</span><span class="sxs-lookup"><span data-stu-id="ed9c4-137">Returns details about how to [monitor the progress](/graph/long-running-actions-overview) of the copy, upon accepting the request.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://contoso.sharepoint.com/_api/v2.0/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="ed9c4-138">`Location` ヘッダーの値は、コピー操作の現在の状況を返すサービスの URL を提供します。</span><span class="sxs-lookup"><span data-stu-id="ed9c4-138">The value of the `Location` header provides a URL for a service that will return the current state of the copy operation.</span></span>
<span data-ttu-id="ed9c4-139">この情報を使用して、[コピーがいつ終了したかを判断する](/graph/long-running-actions-overview)ことができます。</span><span class="sxs-lookup"><span data-stu-id="ed9c4-139">You can use this info to [determine when the copy has finished](/graph/long-running-actions-overview).</span></span>

### <a name="remarks"></a><span data-ttu-id="ed9c4-140">備考</span><span class="sxs-lookup"><span data-stu-id="ed9c4-140">Remarks</span></span>

<span data-ttu-id="ed9c4-p107">多くの場合、コピー操作は非同期で実行されます。API からの応答は、コピー操作が受け入れられたか、コピー先のファイル名が既に使用中のためという理由で拒否されたことのみを示します。</span><span class="sxs-lookup"><span data-stu-id="ed9c4-p107">In many cases the copy action is performed asynchronously. The response from the API will only indicate that the copy operation was accepted or rejected, say due to the destination filename already being in use.</span></span>

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
