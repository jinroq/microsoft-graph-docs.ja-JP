---
title: リソースを取得する
description: ファイルまたはイメージリソースオブジェクトのバイナリデータを取得します。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 9937040d9e53213946df9eb31cf9136bcfda7c71
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568041"
---
# <a name="get-resource"></a><span data-ttu-id="b98e0-103">リソースを取得する</span><span class="sxs-lookup"><span data-stu-id="b98e0-103">Get resource</span></span>

<span data-ttu-id="b98e0-104">ファイルまたはイメージ[リソース](../resources/resource.md)オブジェクトのバイナリデータを取得します。</span><span class="sxs-lookup"><span data-stu-id="b98e0-104">Retrieve the binary data of a file or image [resource](../resources/resource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b98e0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b98e0-105">Permissions</span></span>
<span data-ttu-id="b98e0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b98e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b98e0-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b98e0-108">Permission type</span></span>      | <span data-ttu-id="b98e0-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b98e0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b98e0-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b98e0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b98e0-111">メモ読み取り、メモ書き込み、メモ (すべて)、メモ (すべて)</span><span class="sxs-lookup"><span data-stu-id="b98e0-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="b98e0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b98e0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b98e0-113">メモ. 読み取り、メモ書き込み</span><span class="sxs-lookup"><span data-stu-id="b98e0-113">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="b98e0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b98e0-114">Application</span></span> | <span data-ttu-id="b98e0-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b98e0-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b98e0-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b98e0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="b98e0-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b98e0-117">Request headers</span></span>
| <span data-ttu-id="b98e0-118">名前</span><span class="sxs-lookup"><span data-stu-id="b98e0-118">Name</span></span>       | <span data-ttu-id="b98e0-119">型</span><span class="sxs-lookup"><span data-stu-id="b98e0-119">Type</span></span> | <span data-ttu-id="b98e0-120">説明</span><span class="sxs-lookup"><span data-stu-id="b98e0-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b98e0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b98e0-121">Authorization</span></span>  | <span data-ttu-id="b98e0-122">string</span><span class="sxs-lookup"><span data-stu-id="b98e0-122">string</span></span>  | <span data-ttu-id="b98e0-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b98e0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b98e0-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b98e0-125">Request body</span></span>
<span data-ttu-id="b98e0-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b98e0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b98e0-127">応答</span><span class="sxs-lookup"><span data-stu-id="b98e0-127">Response</span></span>

<span data-ttu-id="b98e0-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で画像またはファイルバイナリデータを返します。</span><span class="sxs-lookup"><span data-stu-id="b98e0-128">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="b98e0-129">注: 画像はブラウザーで直接表示されません。これは、残りのページコンテンツのように、それらを取得するために承認を必要とするからです。</span><span class="sxs-lookup"><span data-stu-id="b98e0-129">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="b98e0-130">例</span><span class="sxs-lookup"><span data-stu-id="b98e0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b98e0-131">要求</span><span class="sxs-lookup"><span data-stu-id="b98e0-131">Request</span></span>
<span data-ttu-id="b98e0-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b98e0-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/resources/{id}/content
```
##### <a name="response"></a><span data-ttu-id="b98e0-133">応答</span><span class="sxs-lookup"><span data-stu-id="b98e0-133">Response</span></span>
<span data-ttu-id="b98e0-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b98e0-134">Here is an example of the response.</span></span>
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
