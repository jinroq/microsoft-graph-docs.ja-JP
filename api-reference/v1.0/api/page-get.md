---
title: ページを取得する
description: Page オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: a4605242ca911e9634e79fa5b9761ae2bb8e0ab6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36022552"
---
# <a name="get-page"></a><span data-ttu-id="a0743-103">ページを取得する</span><span class="sxs-lookup"><span data-stu-id="a0743-103">Get page</span></span>

<span data-ttu-id="a0743-104">[Page](../resources/page.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="a0743-104">Retrieve the properties and relationships of a [page](../resources/page.md) object.</span></span>

<span data-ttu-id="a0743-105">**ページ情報を取得する**</span><span class="sxs-lookup"><span data-stu-id="a0743-105">**Getting page information**</span></span>

<span data-ttu-id="a0743-106">ページの識別子によってページのメタデータにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="a0743-106">Access a page's metadata by page identifier:</span></span>

```
GET /me/onenote/pages/{id}
```

<span data-ttu-id="a0743-107">**ページコンテンツを取得する**</span><span class="sxs-lookup"><span data-stu-id="a0743-107">**Getting page content**</span></span>

<span data-ttu-id="a0743-108">ページの`content`エンドポイントを使用して、ページの HTML コンテンツを取得できます。</span><span class="sxs-lookup"><span data-stu-id="a0743-108">You can use the page's `content` endpoint to get the HTML content of a page:</span></span>

```
GET /me/onenote/pages/{id}/content[?includeIDs=true]
GET /me/onenote/pages/{id}/$value[?includeIDs=true]
```

<span data-ttu-id="a0743-109">クエリ`includeIDs=true`オプションを使用して、[ページを更新](../api/page-update.md)します。</span><span class="sxs-lookup"><span data-stu-id="a0743-109">The `includeIDs=true` query option is used to [update pages](../api/page-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a0743-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a0743-110">Permissions</span></span>
<span data-ttu-id="a0743-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a0743-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0743-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a0743-113">Permission type</span></span>      | <span data-ttu-id="a0743-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a0743-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0743-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a0743-115">Delegated (work or school account)</span></span> | <span data-ttu-id="a0743-116">メモ読み取り、メモ書き込み、メモ (すべて)、メモ (すべて)</span><span class="sxs-lookup"><span data-stu-id="a0743-116">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="a0743-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a0743-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0743-118">メモ. 読み取り、メモ書き込み</span><span class="sxs-lookup"><span data-stu-id="a0743-118">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="a0743-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a0743-119">Application</span></span> | <span data-ttu-id="a0743-120">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0743-120">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0743-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a0743-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages/{id}
GET /users/{id | userPrincipalName}/onenote/pages/{id}
GET /groups/{id}/onenote/pages/{id}
GET /sites/{id}/onenote/pages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a0743-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a0743-122">Optional query parameters</span></span>
<span data-ttu-id="a0743-123">このメソッドは、 `select`応答`expand`をカスタマイズするためのおよび[OData クエリパラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a0743-123">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="a0743-124">既定の応答は`parentSection` 、セクションの`id`、 `name`、および`self`プロパティを展開して選択します。</span><span class="sxs-lookup"><span data-stu-id="a0743-124">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties.</span></span> <span data-ttu-id="a0743-125">ページ`expand`の有効な値`parentNotebook`は`parentSection`、とです。</span><span class="sxs-lookup"><span data-stu-id="a0743-125">Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0743-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a0743-126">Request headers</span></span>
| <span data-ttu-id="a0743-127">名前</span><span class="sxs-lookup"><span data-stu-id="a0743-127">Name</span></span>       | <span data-ttu-id="a0743-128">型</span><span class="sxs-lookup"><span data-stu-id="a0743-128">Type</span></span> | <span data-ttu-id="a0743-129">説明</span><span class="sxs-lookup"><span data-stu-id="a0743-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a0743-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0743-130">Authorization</span></span>  | <span data-ttu-id="a0743-131">string</span><span class="sxs-lookup"><span data-stu-id="a0743-131">string</span></span>  | <span data-ttu-id="a0743-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a0743-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a0743-134">承諾</span><span class="sxs-lookup"><span data-stu-id="a0743-134">Accept</span></span> | <span data-ttu-id="a0743-135">string</span><span class="sxs-lookup"><span data-stu-id="a0743-135">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="a0743-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="a0743-136">Request body</span></span>
<span data-ttu-id="a0743-137">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a0743-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0743-138">応答</span><span class="sxs-lookup"><span data-stu-id="a0743-138">Response</span></span>

<span data-ttu-id="a0743-139">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[page](../resources/page.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a0743-139">If successful, this method returns a `200 OK` response code and the [page](../resources/page.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a0743-140">例</span><span class="sxs-lookup"><span data-stu-id="a0743-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a0743-141">要求</span><span class="sxs-lookup"><span data-stu-id="a0743-141">Request</span></span>
<span data-ttu-id="a0743-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a0743-142">Here is an example of the request.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="a0743-143">応答</span><span class="sxs-lookup"><span data-stu-id="a0743-143">Response</span></span>
<span data-ttu-id="a0743-144">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="a0743-144">Here is an example of the response.</span></span> <span data-ttu-id="a0743-145">注: 簡潔にするために、ここに示す response オブジェクトは切り詰められています。</span><span class="sxs-lookup"><span data-stu-id="a0743-145">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="a0743-146">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a0743-146">All of the properties will be returned from an actual call.</span></span>
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
  "description": "Get page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
