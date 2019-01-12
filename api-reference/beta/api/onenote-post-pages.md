---
title: page を作成する
description: 既定のノートブックの既定のセクションで OneNote の新しいページを作成します。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: d82971bdb3b1e8db4c89e69880681c43ab913939
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965209"
---
# <a name="create-page"></a><span data-ttu-id="d1685-103">page を作成する</span><span class="sxs-lookup"><span data-stu-id="d1685-103">Create page</span></span>

> <span data-ttu-id="d1685-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d1685-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1685-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1685-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d1685-106">既定のノートブックの既定のセクションで OneNote の新しいページを作成します。</span><span class="sxs-lookup"><span data-stu-id="d1685-106">Create a new OneNote page in the default section of the default notebook.</span></span>

<span data-ttu-id="d1685-p102">既定のノートブックの別のセクションにページを作成する場合は、`sectionName` クエリ パラメーターを使用できます。例: `../onenote/pages?sectionName=My%20section`</span><span class="sxs-lookup"><span data-stu-id="d1685-p102">To create a page in a different section in the default notebook, you can use the `sectionName` query parameter.  Example: `../onenote/pages?sectionName=My%20section`</span></span>

<span data-ttu-id="d1685-p103">`POST /onenote/pages` の操作は、現在のユーザーの既定のノートブックでページを作成する場合のみに使用します。他のノートブックを対象とする場合は、[指定されたセクションでページを作成](../api/section-post-pages.md)できます。</span><span class="sxs-lookup"><span data-stu-id="d1685-p103">The `POST /onenote/pages` operation is used only to create pages in the current user's default notebook. If you're targeting other notebooks, you can [create pages in a specified section](../api/section-post-pages.md).</span></span>           
## <a name="permissions"></a><span data-ttu-id="d1685-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d1685-111">Permissions</span></span>
<span data-ttu-id="d1685-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d1685-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1685-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d1685-114">Permission type</span></span>      | <span data-ttu-id="d1685-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d1685-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1685-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d1685-116">Delegated (work or school account)</span></span> | <span data-ttu-id="d1685-117">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1685-117">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="d1685-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d1685-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1685-119">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1685-119">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="d1685-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d1685-120">Application</span></span> | <span data-ttu-id="d1685-121">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1685-121">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1685-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d1685-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /me/onenote/pages
POST /users/{id | userPrincipalName}/onenote/pages
POST /groups/{id}/onenote/pages
POST /sites/{id}/onenote/pages
```

## <a name="request-headers"></a><span data-ttu-id="d1685-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d1685-123">Request headers</span></span>  
| <span data-ttu-id="d1685-124">名前</span><span class="sxs-lookup"><span data-stu-id="d1685-124">Name</span></span>       | <span data-ttu-id="d1685-125">種類</span><span class="sxs-lookup"><span data-stu-id="d1685-125">Type</span></span> | <span data-ttu-id="d1685-126">説明</span><span class="sxs-lookup"><span data-stu-id="d1685-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d1685-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1685-127">Authorization</span></span>  | <span data-ttu-id="d1685-128">string</span><span class="sxs-lookup"><span data-stu-id="d1685-128">string</span></span>  | <span data-ttu-id="d1685-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d1685-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d1685-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d1685-131">Content-Type</span></span> | <span data-ttu-id="d1685-132">string</span><span class="sxs-lookup"><span data-stu-id="d1685-132">string</span></span> | <span data-ttu-id="d1685-p106">HTML コンテンツを表す `text/html` または `application/xhtml+xml` (マルチパート要求の必須の "Presentation" パートを含む)。マルチパート要求では `multipart/form-data; boundary=your-boundary` コンテンツ タイプを使用します。</span><span class="sxs-lookup"><span data-stu-id="d1685-p106">`text/html` or `application/xhtml+xml` for the HTML content, including for the required "Presentation" part of multipart requests. Multipart requests use the `multipart/form-data; boundary=your-boundary` content type.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1685-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="d1685-135">Request body</span></span>
<span data-ttu-id="d1685-136">要求本文には、ページの HTML コンテンツを指定します。</span><span class="sxs-lookup"><span data-stu-id="d1685-136">In the request body, supply the HTML content for the page.</span></span>

<span data-ttu-id="d1685-p107">本文には、要求本文に直接入力した HTML を含めることができます。または、例に示すようにマルチパート メッセージ形式を含めることもできます。バイナリ データを送信する場合は、マルチパート要求を送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d1685-p107">The body can contain HTML placed directly in the request body, or it can contain a multipart message format as shown in the example. If you're sending binary data, then you must send a multipart request.</span></span>

## <a name="response"></a><span data-ttu-id="d1685-139">応答</span><span class="sxs-lookup"><span data-stu-id="d1685-139">Response</span></span>

<span data-ttu-id="d1685-140">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で新規 [page](../resources/page.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d1685-140">If successful, this method returns a `201 Created` response code and the new [page](../resources/page.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1685-141">例</span><span class="sxs-lookup"><span data-stu-id="d1685-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d1685-142">要求</span><span class="sxs-lookup"><span data-stu-id="d1685-142">Request</span></span>
<span data-ttu-id="d1685-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d1685-143">Here is an example of the request.</span></span>

<span data-ttu-id="d1685-p108">`../onenote/pages` のパスで、`sectionName` クエリ パラメーターを使用して、特定のノートブックの指定したセクションにページを作成できます。例: `../onenote/pages?sectionName=My%20section`。セクションが存在しない (または名前が変更された) 場合、API は新しいセクションを作成します。</span><span class="sxs-lookup"><span data-stu-id="d1685-p108">In the `../onenote/pages` path, you can use the `sectionName` query parameter to create a page in a specific section in the default notebook. Example: `../onenote/pages?sectionName=My%20section`. If the section doesn't exist (or was renamed), the API will create a new section.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/me/onenote/pages
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
##### <a name="response"></a><span data-ttu-id="d1685-147">応答</span><span class="sxs-lookup"><span data-stu-id="d1685-147">Response</span></span>
<span data-ttu-id="d1685-148">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d1685-148">Here is an example of the response.</span></span> <span data-ttu-id="d1685-149">注: ここに示す応答オブジェクトは、簡潔にするため切り捨てられます。</span><span class="sxs-lookup"><span data-stu-id="d1685-149">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="d1685-150">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d1685-150">All of the properties will be returned from an actual call.</span></span>
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
  "content": "content-value",
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
