---
title: page を作成する
description: 指定されたセクションに新しいページを作成します。
localization_priority: Normal
ms.openlocfilehash: e65118e6c2ef3396dc8bf16fa398bd4e237aa0ff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871464"
---
# <a name="create-page"></a><span data-ttu-id="6267b-103">page を作成する</span><span class="sxs-lookup"><span data-stu-id="6267b-103">Create page</span></span>

> <span data-ttu-id="6267b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6267b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6267b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6267b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6267b-106">指定されたセクションに新しい[ページ](../resources/page.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="6267b-106">Create a new [page](../resources/page.md) in the specified section.</span></span>
## <a name="permissions"></a><span data-ttu-id="6267b-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6267b-107">Permissions</span></span>
<span data-ttu-id="6267b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6267b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6267b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6267b-110">Permission type</span></span>      | <span data-ttu-id="6267b-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6267b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6267b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6267b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6267b-113">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6267b-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="6267b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6267b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6267b-115">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6267b-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="6267b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6267b-116">Application</span></span> | <span data-ttu-id="6267b-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6267b-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6267b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6267b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/pages
POST /users/{id | userPrincipalName}/onenote/sections/{id}/pages
POST /groups/{id}/onenote/sections/{id}/pages
POST /sites/{id}/onenote/sections/{id}/pages
```
## <a name="request-headers"></a><span data-ttu-id="6267b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6267b-119">Request headers</span></span>
| <span data-ttu-id="6267b-120">名前</span><span class="sxs-lookup"><span data-stu-id="6267b-120">Name</span></span>       | <span data-ttu-id="6267b-121">種類</span><span class="sxs-lookup"><span data-stu-id="6267b-121">Type</span></span> | <span data-ttu-id="6267b-122">説明</span><span class="sxs-lookup"><span data-stu-id="6267b-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6267b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6267b-123">Authorization</span></span>  | <span data-ttu-id="6267b-124">string</span><span class="sxs-lookup"><span data-stu-id="6267b-124">string</span></span>  | <span data-ttu-id="6267b-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6267b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6267b-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6267b-127">Content-Type</span></span> | <span data-ttu-id="6267b-128">string</span><span class="sxs-lookup"><span data-stu-id="6267b-128">string</span></span> | <span data-ttu-id="6267b-p104">HTML コンテンツを表す `text/html` または `application/xhtml+xml` (マルチパート要求の必須の "Presentation" パートを含む)。マルチパート要求では `multipart/form-data; boundary=your-boundary` コンテンツ タイプを使用します。</span><span class="sxs-lookup"><span data-stu-id="6267b-p104">`text/html` or `application/xhtml+xml` for the HTML content, including for the required "Presentation" part of multipart requests. Multipart requests use the `multipart/form-data; boundary=your-boundary` content type.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6267b-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="6267b-131">Request body</span></span>
<span data-ttu-id="6267b-132">要求本文には、ページの HTML コンテンツを指定します。</span><span class="sxs-lookup"><span data-stu-id="6267b-132">In the request body, supply the page HTML content.</span></span>

<span data-ttu-id="6267b-p105">本文には、要求本文に直接入力した HTML を含めることができます。または、例に示すようにマルチパート メッセージ形式を含めることもできます。バイナリ データを送信する場合は、マルチパート要求を送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6267b-p105">The body can contain HTML placed directly in the request body, or it can contain a multipart message format as shown in the example. If you're sending binary data, then you must send a multipart request.</span></span>

## <a name="response"></a><span data-ttu-id="6267b-135">応答</span><span class="sxs-lookup"><span data-stu-id="6267b-135">Response</span></span>

<span data-ttu-id="6267b-136">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で新規 [page](../resources/page.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6267b-136">If successful, this method returns `201 Created` response code and the new [page](../resources/page.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6267b-137">例</span><span class="sxs-lookup"><span data-stu-id="6267b-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6267b-138">要求</span><span class="sxs-lookup"><span data-stu-id="6267b-138">Request</span></span>
<span data-ttu-id="6267b-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6267b-139">Here is an example of the request.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/me/onenote/sections/{id}/pages
Content-length: 312
Content-type: multipart/form-data; boundary=MyPartBoundary198374

--MyPartBoundary198374
Content-Disposition:form-data; name="Presentation"
Content-Type:text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with <i>rendered</i> images and an <b>attached</b> file</title>
    <meta name="created" content="2015-07-22T09:00:00-08:00" />
  </head>
  <body>
    <p>Here's an image from an online source:</p>
    <img src="https://..." alt="an image on the page" width="500" />
    <p>Here's an image uploaded as binary data:</p>
    <img src="name:imageBlock1" alt="an image on the page" width="300" />
    <p>Here's a file attachment:</p>
    <object data-attachment="FileName.pdf" data="name:fileBlock1" type="application/pdf" />
  </body>
</html>

--MyPartBoundary198374
Content-Disposition:form-data; name="imageBlock1"
Content-Type:image/jpeg

... binary image data ...

--MyPartBoundary198374
Content-Disposition:form-data; name="fileBlock1"
Content-Type:application/pdf

... binary file data ...

--MyPartBoundary198374--
```
##### <a name="response"></a><span data-ttu-id="6267b-140">応答</span><span class="sxs-lookup"><span data-stu-id="6267b-140">Response</span></span>
<span data-ttu-id="6267b-141">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6267b-141">Here is an example of the response.</span></span> <span data-ttu-id="6267b-142">注: ここに示す応答オブジェクトは、簡潔にするため切り捨てられます。</span><span class="sxs-lookup"><span data-stu-id="6267b-142">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="6267b-143">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6267b-143">All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 312

{
  "title": "title-value",
  "createdByAppId": "createdByAppId-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  },
  "contentUrl": "contentUrl-value",
  "lastModifiedDateTime": "2016-10-19T10:37:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
