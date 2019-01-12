---
title: リソースを取得する
description: ファイルまたは画像のリソース オブジェクトのバイナリ データを取得します。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: fd7b5e48134cd0d6b8cc1282815beda0e50ef9c3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949956"
---
# <a name="get-resource"></a><span data-ttu-id="33ea3-103">リソースを取得する</span><span class="sxs-lookup"><span data-stu-id="33ea3-103">Get resource</span></span>

> <span data-ttu-id="33ea3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="33ea3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33ea3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33ea3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="33ea3-106">ファイルまたは画像の[リソース](../resources/resource.md) オブジェクトのバイナリ データを取得します。</span><span class="sxs-lookup"><span data-stu-id="33ea3-106">Retrieve the binary data of a file or image [resource](../resources/resource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="33ea3-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="33ea3-107">Permissions</span></span>
<span data-ttu-id="33ea3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="33ea3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33ea3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="33ea3-110">Permission type</span></span>      | <span data-ttu-id="33ea3-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="33ea3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33ea3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="33ea3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="33ea3-113">Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33ea3-113">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="33ea3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="33ea3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33ea3-115">Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33ea3-115">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="33ea3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="33ea3-116">Application</span></span> | <span data-ttu-id="33ea3-117">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33ea3-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33ea3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="33ea3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="33ea3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="33ea3-119">Request headers</span></span>
| <span data-ttu-id="33ea3-120">名前</span><span class="sxs-lookup"><span data-stu-id="33ea3-120">Name</span></span>       | <span data-ttu-id="33ea3-121">種類</span><span class="sxs-lookup"><span data-stu-id="33ea3-121">Type</span></span> | <span data-ttu-id="33ea3-122">説明</span><span class="sxs-lookup"><span data-stu-id="33ea3-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="33ea3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="33ea3-123">Authorization</span></span>  | <span data-ttu-id="33ea3-124">string</span><span class="sxs-lookup"><span data-stu-id="33ea3-124">string</span></span>  | <span data-ttu-id="33ea3-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="33ea3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="33ea3-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="33ea3-127">Request body</span></span>
<span data-ttu-id="33ea3-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="33ea3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33ea3-129">応答</span><span class="sxs-lookup"><span data-stu-id="33ea3-129">Response</span></span>

<span data-ttu-id="33ea3-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で画像またはファイルのバイナリ データを返します。</span><span class="sxs-lookup"><span data-stu-id="33ea3-130">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="33ea3-131">注:残りのページのコンテンツと同様、画像を取得するには承認が必要となるため、ブラウザーでは画像は直接表示されません。</span><span class="sxs-lookup"><span data-stu-id="33ea3-131">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="33ea3-132">例</span><span class="sxs-lookup"><span data-stu-id="33ea3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="33ea3-133">要求</span><span class="sxs-lookup"><span data-stu-id="33ea3-133">Request</span></span>
<span data-ttu-id="33ea3-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="33ea3-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/resources/{id}/content
```
##### <a name="response"></a><span data-ttu-id="33ea3-135">応答</span><span class="sxs-lookup"><span data-stu-id="33ea3-135">Response</span></span>
<span data-ttu-id="33ea3-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="33ea3-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->
```http
HTTP/1.1 200 OK

...binary data...
```
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.onenoteResource"
} -->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
