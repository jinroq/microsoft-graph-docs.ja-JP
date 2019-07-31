---
title: リソースを取得する
description: ファイルまたはイメージリソースオブジェクトのバイナリデータを取得します。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: fdbdec1dec2feea038444977820e68e1d786172c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35982992"
---
# <a name="get-resource"></a><span data-ttu-id="53aaf-103">リソースを取得する</span><span class="sxs-lookup"><span data-stu-id="53aaf-103">Get resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53aaf-104">ファイルまたはイメージ[リソース](../resources/onenoteresource.md)オブジェクトのバイナリデータを取得します。</span><span class="sxs-lookup"><span data-stu-id="53aaf-104">Retrieve the binary data of a file or image [resource](../resources/onenoteresource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="53aaf-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="53aaf-105">Permissions</span></span>
<span data-ttu-id="53aaf-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="53aaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53aaf-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="53aaf-108">Permission type</span></span>      | <span data-ttu-id="53aaf-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="53aaf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53aaf-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="53aaf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="53aaf-111">メモ読み取り、メモ書き込み、メモ (すべて)、メモ (すべて)</span><span class="sxs-lookup"><span data-stu-id="53aaf-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="53aaf-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="53aaf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53aaf-113">メモ. 読み取り、メモ書き込み</span><span class="sxs-lookup"><span data-stu-id="53aaf-113">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="53aaf-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="53aaf-114">Application</span></span> | <span data-ttu-id="53aaf-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53aaf-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="53aaf-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="53aaf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="53aaf-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53aaf-117">Request headers</span></span>
| <span data-ttu-id="53aaf-118">名前</span><span class="sxs-lookup"><span data-stu-id="53aaf-118">Name</span></span>       | <span data-ttu-id="53aaf-119">型</span><span class="sxs-lookup"><span data-stu-id="53aaf-119">Type</span></span> | <span data-ttu-id="53aaf-120">説明</span><span class="sxs-lookup"><span data-stu-id="53aaf-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="53aaf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="53aaf-121">Authorization</span></span>  | <span data-ttu-id="53aaf-122">string</span><span class="sxs-lookup"><span data-stu-id="53aaf-122">string</span></span>  | <span data-ttu-id="53aaf-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="53aaf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53aaf-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="53aaf-125">Request body</span></span>
<span data-ttu-id="53aaf-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="53aaf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53aaf-127">応答</span><span class="sxs-lookup"><span data-stu-id="53aaf-127">Response</span></span>

<span data-ttu-id="53aaf-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で画像またはファイルバイナリデータを返します。</span><span class="sxs-lookup"><span data-stu-id="53aaf-128">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="53aaf-129">注: 画像はブラウザーで直接表示されません。これは、残りのページコンテンツのように、それらを取得するために承認を必要とするからです。</span><span class="sxs-lookup"><span data-stu-id="53aaf-129">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="53aaf-130">例</span><span class="sxs-lookup"><span data-stu-id="53aaf-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53aaf-131">要求</span><span class="sxs-lookup"><span data-stu-id="53aaf-131">Request</span></span>
<span data-ttu-id="53aaf-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="53aaf-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="53aaf-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="53aaf-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/resources/{id}/content
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="53aaf-134">C#</span><span class="sxs-lookup"><span data-stu-id="53aaf-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-resource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="53aaf-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="53aaf-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-resource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="53aaf-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="53aaf-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-resource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="53aaf-137">Java</span><span class="sxs-lookup"><span data-stu-id="53aaf-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-resource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="53aaf-138">応答</span><span class="sxs-lookup"><span data-stu-id="53aaf-138">Response</span></span>
<span data-ttu-id="53aaf-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="53aaf-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

...binary data...
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
