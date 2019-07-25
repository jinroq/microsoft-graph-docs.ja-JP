---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ファイルをチェックアウトする
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e92af4dea2e5b0678e72bc3311042acba9266a5b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861408"
---
# <a name="check-out-a-driveitem-resource"></a><span data-ttu-id="9a42f-102">DriveItem リソースをチェックアウトする</span><span class="sxs-lookup"><span data-stu-id="9a42f-102">Check-out a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a42f-103">driveItem リソースをチェックアウトして、他者がドキュメントを編集できないようにします。また、ドキュメントが[チェックイン](driveitem-checkin.md)されるまで、変更内容が表示されないようにします。</span><span class="sxs-lookup"><span data-stu-id="9a42f-103">Check-out a driveItem resource to prevent others from editing the document, and your changes from being visible until the documented is [checked-in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9a42f-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9a42f-104">Permissions</span></span>

<span data-ttu-id="9a42f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a42f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a42f-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9a42f-107">Permission type</span></span>      | <span data-ttu-id="9a42f-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9a42f-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a42f-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9a42f-109">Delegated (work or school account)</span></span> | <span data-ttu-id="9a42f-110">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a42f-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="9a42f-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9a42f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a42f-112">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a42f-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="9a42f-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9a42f-113">Application</span></span> | <span data-ttu-id="9a42f-114">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a42f-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a42f-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9a42f-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="9a42f-116">要求本文</span><span class="sxs-lookup"><span data-stu-id="9a42f-116">Request body</span></span>

<span data-ttu-id="9a42f-117">要求の本文は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="9a42f-117">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="9a42f-118">例</span><span class="sxs-lookup"><span data-stu-id="9a42f-118">Example</span></span>

<span data-ttu-id="9a42f-119">この例では、`{item-id}` で識別されるファイルをチェックアウトします。</span><span class="sxs-lookup"><span data-stu-id="9a42f-119">This example checks out a file identified by `{item-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9a42f-120">プロトコル</span><span class="sxs-lookup"><span data-stu-id="9a42f-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9a42f-121">C#</span><span class="sxs-lookup"><span data-stu-id="9a42f-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkout-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9a42f-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="9a42f-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkout-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9a42f-123">目的-C</span><span class="sxs-lookup"><span data-stu-id="9a42f-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkout-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9a42f-124">Java</span><span class="sxs-lookup"><span data-stu-id="9a42f-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/checkout-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="9a42f-125">応答</span><span class="sxs-lookup"><span data-stu-id="9a42f-125">Response</span></span>

<span data-ttu-id="9a42f-126">成功すると、API 呼び出しは `204 No content` を返します。</span><span class="sxs-lookup"><span data-stu-id="9a42f-126">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="9a42f-127">備考</span><span class="sxs-lookup"><span data-stu-id="9a42f-127">Remarks</span></span>


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
