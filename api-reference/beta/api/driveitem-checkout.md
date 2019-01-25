---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ファイルをチェック アウト
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 2d1ce5220b055020c42116c2e93b039a31d229aa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518486"
---
# <a name="check-out-a-driveitem-resource"></a><span data-ttu-id="9fe4b-102">DriveItem リソースをチェックアウトする</span><span class="sxs-lookup"><span data-stu-id="9fe4b-102">Check-out a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fe4b-103">driveItem リソースをチェックアウトして、他者がドキュメントを編集できないようにします。また、ドキュメントが[チェックイン](driveitem-checkin.md)されるまで、変更内容が表示されないようにします。</span><span class="sxs-lookup"><span data-stu-id="9fe4b-103">Check-out a driveItem resource to prevent others from editing the document, and your changes from being visible until the documented is [checked-in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9fe4b-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9fe4b-104">Permissions</span></span>

<span data-ttu-id="9fe4b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9fe4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fe4b-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9fe4b-107">Permission type</span></span>      | <span data-ttu-id="9fe4b-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9fe4b-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9fe4b-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9fe4b-109">Delegated (work or school account)</span></span> | <span data-ttu-id="9fe4b-110">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fe4b-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="9fe4b-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9fe4b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fe4b-112">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fe4b-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="9fe4b-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9fe4b-113">Application</span></span> | <span data-ttu-id="9fe4b-114">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fe4b-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9fe4b-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9fe4b-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="9fe4b-116">要求本文</span><span class="sxs-lookup"><span data-stu-id="9fe4b-116">Request body</span></span>

<span data-ttu-id="9fe4b-117">要求の本文は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="9fe4b-117">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="9fe4b-118">例</span><span class="sxs-lookup"><span data-stu-id="9fe4b-118">Example</span></span>

<span data-ttu-id="9fe4b-119">この例では、`{item-id}` で識別されるファイルをチェックアウトします。</span><span class="sxs-lookup"><span data-stu-id="9fe4b-119">This example checks out a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```

## <a name="response"></a><span data-ttu-id="9fe4b-120">応答</span><span class="sxs-lookup"><span data-stu-id="9fe4b-120">Response</span></span>

<span data-ttu-id="9fe4b-121">成功すると、API 呼び出しは `204 No content` を返します。</span><span class="sxs-lookup"><span data-stu-id="9fe4b-121">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="9fe4b-122">備考</span><span class="sxs-lookup"><span data-stu-id="9fe4b-122">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-checkout.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
