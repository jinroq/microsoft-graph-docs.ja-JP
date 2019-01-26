---
title: page を作成する
description: 既定のノートブックの既定のセクションで OneNote の新しいページを作成します。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: c55a3f023ddaa50e7917aed8f1ec1b8bc9b8b6e7
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573460"
---
# <a name="create-page"></a><span data-ttu-id="6978f-103">page を作成する</span><span class="sxs-lookup"><span data-stu-id="6978f-103">Create page</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6978f-104">既定のノートブックの既定のセクションで OneNote の新しいページを作成します。</span><span class="sxs-lookup"><span data-stu-id="6978f-104">Create a new OneNote page in the default section of the default notebook.</span></span>

<span data-ttu-id="6978f-p101">既定のノートブックの別のセクションにページを作成する場合は、`sectionName` クエリ パラメーターを使用できます。例: `../onenote/pages?sectionName=My%20section`</span><span class="sxs-lookup"><span data-stu-id="6978f-p101">To create a page in a different section in the default notebook, you can use the `sectionName` query parameter.  Example: `../onenote/pages?sectionName=My%20section`</span></span>

<span data-ttu-id="6978f-p102">`POST /onenote/pages` の操作は、現在のユーザーの既定のノートブックでページを作成する場合のみに使用します。他のノートブックを対象とする場合は、[指定されたセクションでページを作成](../api/section-post-pages.md)できます。</span><span class="sxs-lookup"><span data-stu-id="6978f-p102">The `POST /onenote/pages` operation is used only to create pages in the current user's default notebook. If you're targeting other notebooks, you can [create pages in a specified section](../api/section-post-pages.md).</span></span>           
## <a name="permissions"></a><span data-ttu-id="6978f-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6978f-109">Permissions</span></span>
<span data-ttu-id="6978f-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6978f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6978f-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6978f-112">Permission type</span></span>      | <span data-ttu-id="6978f-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6978f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6978f-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6978f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6978f-115">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6978f-115">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="6978f-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6978f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6978f-117">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6978f-117">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="6978f-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6978f-118">Application</span></span> | <span data-ttu-id="6978f-119">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6978f-119">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6978f-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6978f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /me/onenote/pages
POST /users/{id | userPrincipalName}/onenote/pages
POST /groups/{id}/onenote/pages
POST /sites/{id}/onenote/pages
```

## <a name="request-headers"></a><span data-ttu-id="6978f-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6978f-121">Request headers</span></span>  
| <span data-ttu-id="6978f-122">名前</span><span class="sxs-lookup"><span data-stu-id="6978f-122">Name</span></span>       | <span data-ttu-id="6978f-123">型</span><span class="sxs-lookup"><span data-stu-id="6978f-123">Type</span></span> | <span data-ttu-id="6978f-124">説明</span><span class="sxs-lookup"><span data-stu-id="6978f-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6978f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6978f-125">Authorization</span></span>  | <span data-ttu-id="6978f-126">string</span><span class="sxs-lookup"><span data-stu-id="6978f-126">string</span></span>  | <span data-ttu-id="6978f-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6978f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6978f-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6978f-129">Content-Type</span></span> | <span data-ttu-id="6978f-130">string</span><span class="sxs-lookup"><span data-stu-id="6978f-130">string</span></span> | <span data-ttu-id="6978f-p105">HTML コンテンツを表す `text/html` または `application/xhtml+xml` (マルチパート要求の必須の "Presentation" パートを含む)。マルチパート要求では `multipart/form-data; boundary=your-boundary` コンテンツ タイプを使用します。</span><span class="sxs-lookup"><span data-stu-id="6978f-p105">`text/html` or `application/xhtml+xml` for the HTML content, including for the required "Presentation" part of multipart requests. Multipart requests use the `multipart/form-data; boundary=your-boundary` content type.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6978f-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="6978f-133">Request body</span></span>
<span data-ttu-id="6978f-134">要求本文には、ページの HTML コンテンツを指定します。</span><span class="sxs-lookup"><span data-stu-id="6978f-134">In the request body, supply the HTML content for the page.</span></span>

<span data-ttu-id="6978f-p106">本文には、要求本文に直接入力した HTML を含めることができます。または、例に示すようにマルチパート メッセージ形式を含めることもできます。バイナリ データを送信する場合は、マルチパート要求を送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6978f-p106">The body can contain HTML placed directly in the request body, or it can contain a multipart message format as shown in the example. If you're sending binary data, then you must send a multipart request.</span></span>

## <a name="response"></a><span data-ttu-id="6978f-137">応答</span><span class="sxs-lookup"><span data-stu-id="6978f-137">Response</span></span>

<span data-ttu-id="6978f-138">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に新しい[onenotePage](../resources/onenotepage.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="6978f-138">If successful, this method returns a `201 Created` response code and the new [onenotePage](../resources/onenotepage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6978f-139">例</span><span class="sxs-lookup"><span data-stu-id="6978f-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6978f-140">要求</span><span class="sxs-lookup"><span data-stu-id="6978f-140">Request</span></span>
<span data-ttu-id="6978f-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6978f-141">Here is an example of the request.</span></span>

<span data-ttu-id="6978f-p107">`../onenote/pages` のパスで、`sectionName` クエリ パラメーターを使用して、特定のノートブックの指定したセクションにページを作成できます。例: `../onenote/pages?sectionName=My%20section`。セクションが存在しない (または名前が変更された) 場合、API は新しいセクションを作成します。</span><span class="sxs-lookup"><span data-stu-id="6978f-p107">In the `../onenote/pages` path, you can use the `sectionName` query parameter to create a page in a specific section in the default notebook. Example: `../onenote/pages?sectionName=My%20section`. If the section doesn't exist (or was renamed), the API will create a new section.</span></span>

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
##### <a name="response"></a><span data-ttu-id="6978f-145">応答</span><span class="sxs-lookup"><span data-stu-id="6978f-145">Response</span></span>
<span data-ttu-id="6978f-146">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6978f-146">Here is an example of the response.</span></span> <span data-ttu-id="6978f-147">注: ここに示す応答オブジェクトは、簡潔にするため切り捨てられます。</span><span class="sxs-lookup"><span data-stu-id="6978f-147">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="6978f-148">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6978f-148">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/onenote-post-pages.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
