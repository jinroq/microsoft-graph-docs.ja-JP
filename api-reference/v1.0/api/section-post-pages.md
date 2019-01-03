---
title: page を作成する
description: 指定されたセクションに新しいページを作成します。
ms.openlocfilehash: ec4373af59ef8a324e8da8f685fc2ff01bde4a2f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023542"
---
# <a name="create-page"></a><span data-ttu-id="3d9e7-103">page を作成する</span><span class="sxs-lookup"><span data-stu-id="3d9e7-103">Create page</span></span>

<span data-ttu-id="3d9e7-104">指定されたセクションに新しい[ページ](../resources/page.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="3d9e7-104">Create a new [page](../resources/page.md) in the specified section.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d9e7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3d9e7-105">Permissions</span></span>
<span data-ttu-id="3d9e7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3d9e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d9e7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3d9e7-108">Permission type</span></span>      | <span data-ttu-id="3d9e7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3d9e7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d9e7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3d9e7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3d9e7-111">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d9e7-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="3d9e7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3d9e7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d9e7-113">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3d9e7-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="3d9e7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3d9e7-114">Application</span></span> | <span data-ttu-id="3d9e7-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d9e7-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d9e7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3d9e7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/pages
POST /users/{id | userPrincipalName}/onenote/sections/{id}/pages
POST /groups/{id}/onenote/sections/{id}/pages
POST /sites/{id}/onenote/sections/{id}/pages
```
## <a name="request-headers"></a><span data-ttu-id="3d9e7-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3d9e7-117">Request headers</span></span>
| <span data-ttu-id="3d9e7-118">名前</span><span class="sxs-lookup"><span data-stu-id="3d9e7-118">Name</span></span>       | <span data-ttu-id="3d9e7-119">型</span><span class="sxs-lookup"><span data-stu-id="3d9e7-119">Type</span></span> | <span data-ttu-id="3d9e7-120">説明</span><span class="sxs-lookup"><span data-stu-id="3d9e7-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3d9e7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d9e7-121">Authorization</span></span>  | <span data-ttu-id="3d9e7-122">string</span><span class="sxs-lookup"><span data-stu-id="3d9e7-122">string</span></span>  | <span data-ttu-id="3d9e7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3d9e7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3d9e7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3d9e7-125">Content-Type</span></span> | <span data-ttu-id="3d9e7-126">string</span><span class="sxs-lookup"><span data-stu-id="3d9e7-126">string</span></span> | <span data-ttu-id="3d9e7-p103">HTML コンテンツを表す `text/html` または `application/xhtml+xml` (マルチパート要求の必須の "Presentation" パートを含む)。マルチパート要求では `multipart/form-data; boundary=your-boundary` コンテンツ タイプを使用します。</span><span class="sxs-lookup"><span data-stu-id="3d9e7-p103">`text/html` or `application/xhtml+xml` for the HTML content, including for the required "Presentation" part of multipart requests. Multipart requests use the `multipart/form-data; boundary=your-boundary` content type.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d9e7-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="3d9e7-129">Request body</span></span>
<span data-ttu-id="3d9e7-130">要求本文には、ページの HTML コンテンツを指定します。</span><span class="sxs-lookup"><span data-stu-id="3d9e7-130">In the request body, supply the page HTML content.</span></span>

<span data-ttu-id="3d9e7-p104">本文には、要求本文に直接入力した HTML を含めることができます。または、例に示すようにマルチパート メッセージ形式を含めることもできます。バイナリ データを送信する場合は、マルチパート要求を送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3d9e7-p104">The body can contain HTML placed directly in the request body, or it can contain a multipart message format as shown in the example. If you're sending binary data, then you must send a multipart request.</span></span>

## <a name="response"></a><span data-ttu-id="3d9e7-133">応答</span><span class="sxs-lookup"><span data-stu-id="3d9e7-133">Response</span></span>

<span data-ttu-id="3d9e7-134">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で新規 [page](../resources/page.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3d9e7-134">If successful, this method returns `201 Created` response code and the new [page](../resources/page.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d9e7-135">例</span><span class="sxs-lookup"><span data-stu-id="3d9e7-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3d9e7-136">要求</span><span class="sxs-lookup"><span data-stu-id="3d9e7-136">Request</span></span>
<span data-ttu-id="3d9e7-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3d9e7-137">Here is an example of the request.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/pages
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
##### <a name="response"></a><span data-ttu-id="3d9e7-138">応答</span><span class="sxs-lookup"><span data-stu-id="3d9e7-138">Response</span></span>
<span data-ttu-id="3d9e7-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="3d9e7-139">Here is an example of the response.</span></span> <span data-ttu-id="3d9e7-140">注: ここに示す応答オブジェクトは、簡潔にするため切り捨てられます。</span><span class="sxs-lookup"><span data-stu-id="3d9e7-140">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="3d9e7-141">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="3d9e7-141">All of the properties will be returned from an actual call.</span></span>
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