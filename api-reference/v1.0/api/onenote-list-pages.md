---
title: pages を一覧表示する
description: ページ オブジェクトの一覧を取得します。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 5a7796bad3afbb7f30b6200f20b667fe53cc0c89
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955647"
---
# <a name="list-pages"></a><span data-ttu-id="553e7-103">pages を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="553e7-103">List pages</span></span>

<span data-ttu-id="553e7-104">[ページ](../resources/page.md) オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="553e7-104">Retrieve a list of [page](../resources/page.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="553e7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="553e7-105">Permissions</span></span>
<span data-ttu-id="553e7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="553e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="553e7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="553e7-108">Permission type</span></span>      | <span data-ttu-id="553e7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="553e7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="553e7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="553e7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="553e7-111">Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="553e7-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="553e7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="553e7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="553e7-113">Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="553e7-113">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="553e7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="553e7-114">Application</span></span> | <span data-ttu-id="553e7-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="553e7-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="553e7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="553e7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages
GET /users/{id | userPrincipalName}/onenote/pages
GET /groups/{id}/onenote/pages
GET /sites/{id}/onenote/pages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="553e7-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="553e7-117">Optional query parameters</span></span>
<span data-ttu-id="553e7-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="553e7-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="553e7-p102">ページの既定のクエリは、`lastModifiedTime desc` の順に最初の 20 ページを返します。既定のクエリが 20 ページより多くのページを返す場合、応答には `@odata.nextLink` が含まれ、ユーザーはこれを使って結果セットのページを移動できます。`top` 要求に対して返されるページの最大数は 100 です。</span><span class="sxs-lookup"><span data-stu-id="553e7-p102">The default query for pages returns the top 20 pages ordered by `lastModifiedTime desc`. If the default query returns more than 20 pages, the response contains an `@odata.nextLink` that you can use to page through the result set. The maximum number of pages returned for a `top` request is 100.</span></span>

<span data-ttu-id="553e7-p103">既定の応答は、`parentSection` を展開し、セクションの `id`、`displayName`、`self` プロパティを選択します。ページの有効な `expand` 値は、`parentNotebook` と `parentSection` です。</span><span class="sxs-lookup"><span data-stu-id="553e7-p103">The default response expands `parentSection` and selects the section's `id`, `displayName`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="553e7-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="553e7-124">Request headers</span></span>
| <span data-ttu-id="553e7-125">名前</span><span class="sxs-lookup"><span data-stu-id="553e7-125">Name</span></span>       | <span data-ttu-id="553e7-126">型</span><span class="sxs-lookup"><span data-stu-id="553e7-126">Type</span></span> | <span data-ttu-id="553e7-127">説明</span><span class="sxs-lookup"><span data-stu-id="553e7-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="553e7-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="553e7-128">Authorization</span></span>  | <span data-ttu-id="553e7-129">string</span><span class="sxs-lookup"><span data-stu-id="553e7-129">string</span></span>  | <span data-ttu-id="553e7-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="553e7-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="553e7-132">承諾</span><span class="sxs-lookup"><span data-stu-id="553e7-132">Accept</span></span> | <span data-ttu-id="553e7-133">string</span><span class="sxs-lookup"><span data-stu-id="553e7-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="553e7-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="553e7-134">Request body</span></span>
<span data-ttu-id="553e7-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="553e7-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="553e7-136">応答</span><span class="sxs-lookup"><span data-stu-id="553e7-136">Response</span></span>

<span data-ttu-id="553e7-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [page](../resources/page.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="553e7-137">If successful, this method returns a `200 OK` response code and a collection of [page](../resources/page.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="553e7-138">例</span><span class="sxs-lookup"><span data-stu-id="553e7-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="553e7-139">要求</span><span class="sxs-lookup"><span data-stu-id="553e7-139">Request</span></span>
<span data-ttu-id="553e7-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="553e7-140">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/pages
```
##### <a name="response"></a><span data-ttu-id="553e7-141">応答</span><span class="sxs-lookup"><span data-stu-id="553e7-141">Response</span></span>
<span data-ttu-id="553e7-142">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="553e7-142">Here is an example of the response.</span></span> <span data-ttu-id="553e7-143">注: ここに示す応答オブジェクトは、簡潔にするため切り捨てられます。</span><span class="sxs-lookup"><span data-stu-id="553e7-143">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="553e7-144">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="553e7-144">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List pages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
