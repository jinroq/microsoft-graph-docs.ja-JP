---
title: リソースを取得する
description: ファイルまたは画像のリソース オブジェクトのバイナリ データを取得します。
ms.openlocfilehash: e96dcce0793b4d3faf4afcdb8d07204ebafd7444
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024056"
---
# <a name="get-resource"></a><span data-ttu-id="3670f-103">リソースを取得する</span><span class="sxs-lookup"><span data-stu-id="3670f-103">Get resource</span></span>

<span data-ttu-id="3670f-104">ファイルまたは画像の[リソース](../resources/resource.md) オブジェクトのバイナリ データを取得します。</span><span class="sxs-lookup"><span data-stu-id="3670f-104">Retrieve the binary data of a file or image [resource](../resources/resource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3670f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3670f-105">Permissions</span></span>
<span data-ttu-id="3670f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3670f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3670f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3670f-108">Permission type</span></span>      | <span data-ttu-id="3670f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3670f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3670f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3670f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3670f-111">Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3670f-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="3670f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3670f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3670f-113">Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3670f-113">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="3670f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3670f-114">Application</span></span> | <span data-ttu-id="3670f-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3670f-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3670f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3670f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="3670f-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3670f-117">Request headers</span></span>
| <span data-ttu-id="3670f-118">名前</span><span class="sxs-lookup"><span data-stu-id="3670f-118">Name</span></span>       | <span data-ttu-id="3670f-119">型</span><span class="sxs-lookup"><span data-stu-id="3670f-119">Type</span></span> | <span data-ttu-id="3670f-120">説明</span><span class="sxs-lookup"><span data-stu-id="3670f-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3670f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3670f-121">Authorization</span></span>  | <span data-ttu-id="3670f-122">string</span><span class="sxs-lookup"><span data-stu-id="3670f-122">string</span></span>  | <span data-ttu-id="3670f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3670f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3670f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="3670f-125">Request body</span></span>
<span data-ttu-id="3670f-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3670f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3670f-127">応答</span><span class="sxs-lookup"><span data-stu-id="3670f-127">Response</span></span>

<span data-ttu-id="3670f-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で画像またはファイルのバイナリ データを返します。</span><span class="sxs-lookup"><span data-stu-id="3670f-128">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="3670f-129">注:残りのページのコンテンツと同様、画像を取得するには承認が必要となるため、ブラウザーでは画像は直接表示されません。</span><span class="sxs-lookup"><span data-stu-id="3670f-129">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="3670f-130">例</span><span class="sxs-lookup"><span data-stu-id="3670f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3670f-131">要求</span><span class="sxs-lookup"><span data-stu-id="3670f-131">Request</span></span>
<span data-ttu-id="3670f-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3670f-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/resources/{id}/content
```
##### <a name="response"></a><span data-ttu-id="3670f-133">応答</span><span class="sxs-lookup"><span data-stu-id="3670f-133">Response</span></span>
<span data-ttu-id="3670f-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="3670f-134">Here is an example of the response.</span></span>
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
  "tocPath": ""
}-->