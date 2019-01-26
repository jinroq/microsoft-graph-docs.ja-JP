---
title: pages を一覧表示する
description: 指定されたセクションからページ オブジェクトの一覧を取得します。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: a68fef97f48c48f789317915dd2da0dacdd2f06f
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571213"
---
# <a name="list-pages"></a><span data-ttu-id="f696e-103">pages を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f696e-103">List pages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f696e-104">指定したセクションからには、 [onenotePage](../resources/onenotepage.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="f696e-104">Retrieve a list of [onenotePage](../resources/onenotepage.md) objects from the specified section.</span></span>
## <a name="permissions"></a><span data-ttu-id="f696e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f696e-105">Permissions</span></span>
<span data-ttu-id="f696e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f696e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f696e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f696e-108">Permission type</span></span>      | <span data-ttu-id="f696e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f696e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f696e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f696e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f696e-111">Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f696e-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="f696e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f696e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f696e-113">Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f696e-113">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="f696e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f696e-114">Application</span></span> | <span data-ttu-id="f696e-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f696e-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f696e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f696e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}/pages
GET /users/{id | userPrincipalName}/onenote/sections/{id}/pages
GET /groups/{id}/onenote/sections/{id}/pages
GET /sites/{id}/onenote/sections/{id}/pages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f696e-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f696e-117">Optional query parameters</span></span>
<span data-ttu-id="f696e-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f696e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="f696e-p102">ページの既定のクエリは、`lastModifiedTime desc` の順に最初の 20 ページを返します。既定のクエリが 20 ページより多くのページを返す場合、応答には `@odata.nextLink` が含まれ、ユーザーはこれを使って結果セットのページを移動できます。`top` 要求に対して返されるページの最大数は 100 です。</span><span class="sxs-lookup"><span data-stu-id="f696e-p102">The default query for pages returns the top 20 pages ordered by `lastModifiedTime desc`. If the default query returns more than 20 pages, the response contains an `@odata.nextLink` that you can use to page through the result set. The maximum number of pages returned for a `top` request is 100.</span></span>

<span data-ttu-id="f696e-p103">既定の応答は、`parentSection` を展開し、セクションの `id`、`name`、`self` プロパティを選択します。ページの有効な `expand` 値は、`parentNotebook` と `parentSection` です。</span><span class="sxs-lookup"><span data-stu-id="f696e-p103">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f696e-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f696e-124">Request headers</span></span>
| <span data-ttu-id="f696e-125">名前</span><span class="sxs-lookup"><span data-stu-id="f696e-125">Name</span></span>       | <span data-ttu-id="f696e-126">型</span><span class="sxs-lookup"><span data-stu-id="f696e-126">Type</span></span> | <span data-ttu-id="f696e-127">説明</span><span class="sxs-lookup"><span data-stu-id="f696e-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f696e-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="f696e-128">Authorization</span></span>  | <span data-ttu-id="f696e-129">string</span><span class="sxs-lookup"><span data-stu-id="f696e-129">string</span></span>  | <span data-ttu-id="f696e-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f696e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f696e-132">承諾</span><span class="sxs-lookup"><span data-stu-id="f696e-132">Accept</span></span> | <span data-ttu-id="f696e-133">string</span><span class="sxs-lookup"><span data-stu-id="f696e-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="f696e-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="f696e-134">Request body</span></span>
<span data-ttu-id="f696e-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f696e-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f696e-136">応答</span><span class="sxs-lookup"><span data-stu-id="f696e-136">Response</span></span>

<span data-ttu-id="f696e-137">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[onenotePage](../resources/onenotepage.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f696e-137">If successful, this method returns a `200 OK` response code and a collection of [onenotePage](../resources/onenotepage.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f696e-138">例</span><span class="sxs-lookup"><span data-stu-id="f696e-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f696e-139">要求</span><span class="sxs-lookup"><span data-stu-id="f696e-139">Request</span></span>
<span data-ttu-id="f696e-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f696e-140">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onenote/sections/{id}/pages
```
##### <a name="response"></a><span data-ttu-id="f696e-141">応答</span><span class="sxs-lookup"><span data-stu-id="f696e-141">Response</span></span>
<span data-ttu-id="f696e-142">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="f696e-142">Here is an example of the response.</span></span> <span data-ttu-id="f696e-143">注: ここに示す応答オブジェクトは、簡潔にするため切り捨てられます。</span><span class="sxs-lookup"><span data-stu-id="f696e-143">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="f696e-144">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f696e-144">All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 393

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List pages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/section-list-pages.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
