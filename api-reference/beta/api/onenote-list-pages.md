---
title: ページを一覧表示する
description: ページオブジェクトのリストを取得します。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 4717428dc7b45d893993dd366eb33137000d3bb3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540402"
---
# <a name="list-pages"></a><span data-ttu-id="f1cc1-103">ページを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f1cc1-103">List pages</span></span>

<span data-ttu-id="f1cc1-104">[ページ](../resources/page.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="f1cc1-104">Retrieve a list of [page](../resources/page.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="f1cc1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f1cc1-105">Permissions</span></span>
<span data-ttu-id="f1cc1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f1cc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1cc1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f1cc1-108">Permission type</span></span>      | <span data-ttu-id="f1cc1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f1cc1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1cc1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f1cc1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f1cc1-111">メモ読み取り、メモ書き込み、メモ (すべて)、メモ (すべて)</span><span class="sxs-lookup"><span data-stu-id="f1cc1-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="f1cc1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f1cc1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1cc1-113">メモ. 読み取り、メモ書き込み</span><span class="sxs-lookup"><span data-stu-id="f1cc1-113">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="f1cc1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f1cc1-114">Application</span></span> | <span data-ttu-id="f1cc1-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1cc1-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1cc1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f1cc1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages
GET /users/{id | userPrincipalName}/onenote/pages
GET /groups/{id}/onenote/pages
GET /sites/{id}/onenote/pages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f1cc1-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f1cc1-117">Optional query parameters</span></span>
<span data-ttu-id="f1cc1-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f1cc1-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="f1cc1-119">ページの既定のクエリは、並べ替えられた上位`lastModifiedTime desc`20 ページを返します。</span><span class="sxs-lookup"><span data-stu-id="f1cc1-119">The default query for pages returns the top 20 pages ordered by `lastModifiedTime desc`.</span></span> <span data-ttu-id="f1cc1-120">既定のクエリが20ページを超える場合、応答には、 `@odata.nextLink`結果セットのページを取得するために使用できるが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f1cc1-120">If the default query returns more than 20 pages, the response contains an `@odata.nextLink` that you can use to page through the result set.</span></span> <span data-ttu-id="f1cc1-121">`top`要求に対して返されるページの最大数は100です。</span><span class="sxs-lookup"><span data-stu-id="f1cc1-121">The maximum number of pages returned for a `top` request is 100.</span></span>

<span data-ttu-id="f1cc1-122">既定の応答は`parentSection` 、セクションの`id`、 `displayName`、および`self`プロパティを展開して選択します。</span><span class="sxs-lookup"><span data-stu-id="f1cc1-122">The default response expands `parentSection` and selects the section's `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="f1cc1-123">ページ`expand`の有効な値`parentNotebook`は`parentSection`、とです。</span><span class="sxs-lookup"><span data-stu-id="f1cc1-123">Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f1cc1-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f1cc1-124">Request headers</span></span>
| <span data-ttu-id="f1cc1-125">名前</span><span class="sxs-lookup"><span data-stu-id="f1cc1-125">Name</span></span>       | <span data-ttu-id="f1cc1-126">型</span><span class="sxs-lookup"><span data-stu-id="f1cc1-126">Type</span></span> | <span data-ttu-id="f1cc1-127">説明</span><span class="sxs-lookup"><span data-stu-id="f1cc1-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f1cc1-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1cc1-128">Authorization</span></span>  | <span data-ttu-id="f1cc1-129">string</span><span class="sxs-lookup"><span data-stu-id="f1cc1-129">string</span></span>  | <span data-ttu-id="f1cc1-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f1cc1-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f1cc1-132">承諾</span><span class="sxs-lookup"><span data-stu-id="f1cc1-132">Accept</span></span> | <span data-ttu-id="f1cc1-133">string</span><span class="sxs-lookup"><span data-stu-id="f1cc1-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="f1cc1-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="f1cc1-134">Request body</span></span>
<span data-ttu-id="f1cc1-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f1cc1-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1cc1-136">応答</span><span class="sxs-lookup"><span data-stu-id="f1cc1-136">Response</span></span>

<span data-ttu-id="f1cc1-137">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[page](../resources/page.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f1cc1-137">If successful, this method returns a `200 OK` response code and a collection of [page](../resources/page.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f1cc1-138">例</span><span class="sxs-lookup"><span data-stu-id="f1cc1-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1cc1-139">要求</span><span class="sxs-lookup"><span data-stu-id="f1cc1-139">Request</span></span>
<span data-ttu-id="f1cc1-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f1cc1-140">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/pages
```
##### <a name="response"></a><span data-ttu-id="f1cc1-141">応答</span><span class="sxs-lookup"><span data-stu-id="f1cc1-141">Response</span></span>
<span data-ttu-id="f1cc1-p105">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f1cc1-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call. </span></span><!-- { "blockType": "ignored" } -->
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
