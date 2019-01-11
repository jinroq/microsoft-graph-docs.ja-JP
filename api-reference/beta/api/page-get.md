---
title: ページを取得する
description: ページ オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
ms.openlocfilehash: 117f4d15d676f0be26e75a610d87b2de2581b17a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890826"
---
# <a name="get-page"></a><span data-ttu-id="dcf73-103">ページを取得する</span><span class="sxs-lookup"><span data-stu-id="dcf73-103">Get page</span></span>

> <span data-ttu-id="dcf73-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dcf73-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dcf73-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dcf73-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dcf73-106">[ページ](../resources/page.md) オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="dcf73-106">Retrieve the properties and relationships of a [page](../resources/page.md) object.</span></span>

<span data-ttu-id="dcf73-107">**ページ情報を取得する**</span><span class="sxs-lookup"><span data-stu-id="dcf73-107">**Getting page information**</span></span>

<span data-ttu-id="dcf73-108">ページ識別子によって、ページのメタデータにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="dcf73-108">Access a page's metadata by page identifier:</span></span>

```
GET /me/onenote/pages/{id}
```

<span data-ttu-id="dcf73-109">**ページ コンテンツを取得する**</span><span class="sxs-lookup"><span data-stu-id="dcf73-109">**Getting page content**</span></span>

<span data-ttu-id="dcf73-110">ページの `content` エンドポイントを使用して、ページの HTML コンテンツを取得できます。</span><span class="sxs-lookup"><span data-stu-id="dcf73-110">You can use the page's `content` endpoint to get the HTML content of a page:</span></span>

```
GET /me/onenote/pages/{id}/content[?includeIDs=true]
GET /me/onenote/pages/{id}/$value[?includeIDs=true]
```

<span data-ttu-id="dcf73-111">`includeIDs=true` クエリ オプションを使用して[ページを更新します](../api/page-update.md)。</span><span class="sxs-lookup"><span data-stu-id="dcf73-111">The `includeIDs=true` query option is used to [update pages](../api/page-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dcf73-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dcf73-112">Permissions</span></span>
<span data-ttu-id="dcf73-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dcf73-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcf73-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dcf73-115">Permission type</span></span>      | <span data-ttu-id="dcf73-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dcf73-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dcf73-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dcf73-117">Delegated (work or school account)</span></span> | <span data-ttu-id="dcf73-118">Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcf73-118">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="dcf73-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dcf73-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcf73-120">Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dcf73-120">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="dcf73-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dcf73-121">Application</span></span> | <span data-ttu-id="dcf73-122">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcf73-122">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dcf73-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dcf73-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages/{id}
GET /users/{id | userPrincipalName}/onenote/pages/{id}
GET /groups/{id}/onenote/pages/{id}
GET /sites/{id}/onenote/pages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dcf73-124">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="dcf73-124">Optional query parameters</span></span>
<span data-ttu-id="dcf73-125">このメソッドは、応答をカスタマイズするための `select` および `expand` [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="dcf73-125">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="dcf73-p103">既定の応答は、`parentSection` を展開し、セクションの `id`、`name`、`self` プロパティを選択します。ページの有効な `expand` 値は、`parentNotebook` と `parentSection` です。</span><span class="sxs-lookup"><span data-stu-id="dcf73-p103">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dcf73-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dcf73-128">Request headers</span></span>
| <span data-ttu-id="dcf73-129">名前</span><span class="sxs-lookup"><span data-stu-id="dcf73-129">Name</span></span>       | <span data-ttu-id="dcf73-130">種類</span><span class="sxs-lookup"><span data-stu-id="dcf73-130">Type</span></span> | <span data-ttu-id="dcf73-131">説明</span><span class="sxs-lookup"><span data-stu-id="dcf73-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="dcf73-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="dcf73-132">Authorization</span></span>  | <span data-ttu-id="dcf73-133">string</span><span class="sxs-lookup"><span data-stu-id="dcf73-133">string</span></span>  | <span data-ttu-id="dcf73-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="dcf73-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dcf73-136">承諾</span><span class="sxs-lookup"><span data-stu-id="dcf73-136">Accept</span></span> | <span data-ttu-id="dcf73-137">string</span><span class="sxs-lookup"><span data-stu-id="dcf73-137">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="dcf73-138">要求本文</span><span class="sxs-lookup"><span data-stu-id="dcf73-138">Request body</span></span>
<span data-ttu-id="dcf73-139">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="dcf73-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcf73-140">応答</span><span class="sxs-lookup"><span data-stu-id="dcf73-140">Response</span></span>

<span data-ttu-id="dcf73-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [page](../resources/page.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dcf73-141">If successful, this method returns a `200 OK` response code and the [page](../resources/page.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dcf73-142">例</span><span class="sxs-lookup"><span data-stu-id="dcf73-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dcf73-143">要求</span><span class="sxs-lookup"><span data-stu-id="dcf73-143">Request</span></span>
<span data-ttu-id="dcf73-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dcf73-144">Here is an example of the request.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="dcf73-145">応答</span><span class="sxs-lookup"><span data-stu-id="dcf73-145">Response</span></span>
<span data-ttu-id="dcf73-146">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="dcf73-146">Here is an example of the response.</span></span> <span data-ttu-id="dcf73-147">注: ここに示す応答オブジェクトは、簡潔にするため切り捨てられます。</span><span class="sxs-lookup"><span data-stu-id="dcf73-147">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="dcf73-148">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="dcf73-148">All of the properties will be returned from an actual call.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 312

{
  "title": "title-value",
  "createdByAppId": "createdByAppId-value",
  "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
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
  "description": "Get page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
