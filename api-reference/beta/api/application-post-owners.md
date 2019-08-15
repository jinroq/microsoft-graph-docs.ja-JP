---
title: 所有者を作成する
description: この API を使用して、新しい所有者を作成します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2dbfaf498b8b0726da1de3ee35fafd547747e990
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408280"
---
# <a name="create-owner"></a><span data-ttu-id="4de2c-103">所有者を作成する</span><span class="sxs-lookup"><span data-stu-id="4de2c-103">Create owner</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4de2c-104">この API を使用して、新しい所有者を作成します。</span><span class="sxs-lookup"><span data-stu-id="4de2c-104">Use this API to create a new owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="4de2c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4de2c-105">Permissions</span></span>
<span data-ttu-id="4de2c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4de2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4de2c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4de2c-108">Permission type</span></span>      | <span data-ttu-id="4de2c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4de2c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4de2c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4de2c-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="4de2c-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4de2c-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4de2c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4de2c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4de2c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4de2c-113">Not supported.</span></span>    |
|<span data-ttu-id="4de2c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4de2c-114">Application</span></span> | <span data-ttu-id="4de2c-115">Application.readwrite.ownedby とディレクトリ。すべての、およびすべてのディレクトリを取得します。すべてのアプリケーション</span><span class="sxs-lookup"><span data-stu-id="4de2c-115">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4de2c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4de2c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="4de2c-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4de2c-117">Request headers</span></span>
| <span data-ttu-id="4de2c-118">名前</span><span class="sxs-lookup"><span data-stu-id="4de2c-118">Name</span></span> | <span data-ttu-id="4de2c-119">説明</span><span class="sxs-lookup"><span data-stu-id="4de2c-119">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="4de2c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4de2c-120">Authorization</span></span> | <span data-ttu-id="4de2c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4de2c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4de2c-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="4de2c-123">Request body</span></span>
<span data-ttu-id="4de2c-124">要求本文で、owner として割り当てられるディレクトリオブジェクトの識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="4de2c-124">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="4de2c-125">応答</span><span class="sxs-lookup"><span data-stu-id="4de2c-125">Response</span></span>

<span data-ttu-id="4de2c-126">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="4de2c-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4de2c-127">例</span><span class="sxs-lookup"><span data-stu-id="4de2c-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="4de2c-128">要求</span><span class="sxs-lookup"><span data-stu-id="4de2c-128">Request</span></span>
<span data-ttu-id="4de2c-129">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="4de2c-129">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4de2c-130">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4de2c-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_application"
}-->
```http
POST https://graph.microsoft.com/beta/applications/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
"@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}

```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4de2c-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4de2c-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="4de2c-132">C#</span><span class="sxs-lookup"><span data-stu-id="4de2c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4de2c-133">目的-C</span><span class="sxs-lookup"><span data-stu-id="4de2c-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="4de2c-134">応答</span><span class="sxs-lookup"><span data-stu-id="4de2c-134">Response</span></span>

<span data-ttu-id="4de2c-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4de2c-135">The following is an example of the response.</span></span>

><span data-ttu-id="4de2c-136">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="4de2c-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4de2c-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4de2c-137">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
