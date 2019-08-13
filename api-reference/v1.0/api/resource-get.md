---
title: リソースを取得する
description: ファイルまたはイメージリソースオブジェクトのバイナリデータを取得します。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: ec2d7b21ecd2e6bc631bc6a630e7e3af399782ba
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320176"
---
# <a name="get-resource"></a><span data-ttu-id="e290f-103">リソースを取得する</span><span class="sxs-lookup"><span data-stu-id="e290f-103">Get resource</span></span>

<span data-ttu-id="e290f-104">ファイルまたはイメージ[リソース](../resources/resource.md)オブジェクトのバイナリデータを取得します。</span><span class="sxs-lookup"><span data-stu-id="e290f-104">Retrieve the binary data of a file or image [resource](../resources/resource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e290f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e290f-105">Permissions</span></span>
<span data-ttu-id="e290f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e290f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e290f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e290f-108">Permission type</span></span>      | <span data-ttu-id="e290f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e290f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e290f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e290f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e290f-111">メモ読み取り、メモ書き込み、メモ (すべて)、メモ (すべて)</span><span class="sxs-lookup"><span data-stu-id="e290f-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="e290f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e290f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e290f-113">メモ. 読み取り、メモ書き込み</span><span class="sxs-lookup"><span data-stu-id="e290f-113">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="e290f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e290f-114">Application</span></span> | <span data-ttu-id="e290f-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e290f-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e290f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e290f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="e290f-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e290f-117">Request headers</span></span>
| <span data-ttu-id="e290f-118">名前</span><span class="sxs-lookup"><span data-stu-id="e290f-118">Name</span></span>       | <span data-ttu-id="e290f-119">型</span><span class="sxs-lookup"><span data-stu-id="e290f-119">Type</span></span> | <span data-ttu-id="e290f-120">説明</span><span class="sxs-lookup"><span data-stu-id="e290f-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e290f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e290f-121">Authorization</span></span>  | <span data-ttu-id="e290f-122">string</span><span class="sxs-lookup"><span data-stu-id="e290f-122">string</span></span>  | <span data-ttu-id="e290f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e290f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e290f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="e290f-125">Request body</span></span>
<span data-ttu-id="e290f-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e290f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e290f-127">応答</span><span class="sxs-lookup"><span data-stu-id="e290f-127">Response</span></span>

<span data-ttu-id="e290f-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で画像またはファイルバイナリデータを返します。</span><span class="sxs-lookup"><span data-stu-id="e290f-128">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="e290f-129">注: 画像はブラウザーで直接表示されません。これは、残りのページコンテンツのように、それらを取得するために承認を必要とするからです。</span><span class="sxs-lookup"><span data-stu-id="e290f-129">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="e290f-130">例</span><span class="sxs-lookup"><span data-stu-id="e290f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e290f-131">要求</span><span class="sxs-lookup"><span data-stu-id="e290f-131">Request</span></span>
<span data-ttu-id="e290f-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e290f-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e290f-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e290f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/resources/{id}/content
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e290f-134">C#</span><span class="sxs-lookup"><span data-stu-id="e290f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-resource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e290f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e290f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-resource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e290f-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="e290f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-resource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e290f-137">Java</span><span class="sxs-lookup"><span data-stu-id="e290f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-resource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e290f-138">応答</span><span class="sxs-lookup"><span data-stu-id="e290f-138">Response</span></span>
<span data-ttu-id="e290f-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="e290f-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Edm.Stream"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

...binary data...
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
