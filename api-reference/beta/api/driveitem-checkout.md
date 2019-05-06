---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ファイルをチェックアウトする
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: aaee21e48cba0a317600e2d1a5ab3fc29e9c02c4
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33589260"
---
# <a name="check-out-a-driveitem-resource"></a><span data-ttu-id="183be-102">DriveItem リソースをチェックアウトする</span><span class="sxs-lookup"><span data-stu-id="183be-102">Check-out a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="183be-103">driveItem リソースをチェックアウトして、他者がドキュメントを編集できないようにします。また、ドキュメントが[チェックイン](driveitem-checkin.md)されるまで、変更内容が表示されないようにします。</span><span class="sxs-lookup"><span data-stu-id="183be-103">Check-out a driveItem resource to prevent others from editing the document, and your changes from being visible until the documented is [checked-in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="183be-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="183be-104">Permissions</span></span>

<span data-ttu-id="183be-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="183be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="183be-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="183be-107">Permission type</span></span>      | <span data-ttu-id="183be-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="183be-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="183be-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="183be-109">Delegated (work or school account)</span></span> | <span data-ttu-id="183be-110">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="183be-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="183be-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="183be-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="183be-112">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="183be-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="183be-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="183be-113">Application</span></span> | <span data-ttu-id="183be-114">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="183be-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="183be-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="183be-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="183be-116">要求本文</span><span class="sxs-lookup"><span data-stu-id="183be-116">Request body</span></span>

<span data-ttu-id="183be-117">要求の本文は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="183be-117">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="183be-118">例</span><span class="sxs-lookup"><span data-stu-id="183be-118">Example</span></span>

<span data-ttu-id="183be-119">この例では、`{item-id}` で識別されるファイルをチェックアウトします。</span><span class="sxs-lookup"><span data-stu-id="183be-119">This example checks out a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```

## <a name="response"></a><span data-ttu-id="183be-120">応答</span><span class="sxs-lookup"><span data-stu-id="183be-120">Response</span></span>

<span data-ttu-id="183be-121">成功すると、API 呼び出しは `204 No content` を返します。</span><span class="sxs-lookup"><span data-stu-id="183be-121">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="183be-122">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="183be-122">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="183be-123">Visual</span><span class="sxs-lookup"><span data-stu-id="183be-123">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/checkout-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="183be-124">Java</span><span class="sxs-lookup"><span data-stu-id="183be-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/checkout-item-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="remarks"></a><span data-ttu-id="183be-125">備考</span><span class="sxs-lookup"><span data-stu-id="183be-125">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-checkout.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-checkout.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
