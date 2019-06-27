---
title: ノートブックを取得する
description: ノートブックオブジェクトのプロパティとリレーションシップを取得します。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 360478d78ffe3cb1833fa3de29eeac1e65dabc1c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274565"
---
# <a name="get-notebook"></a><span data-ttu-id="77e2a-103">ノートブックを取得する</span><span class="sxs-lookup"><span data-stu-id="77e2a-103">Get notebook</span></span>

<span data-ttu-id="77e2a-104">[ノートブック](../resources/notebook.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="77e2a-104">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="77e2a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="77e2a-105">Permissions</span></span>
<span data-ttu-id="77e2a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="77e2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77e2a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="77e2a-108">Permission type</span></span>      | <span data-ttu-id="77e2a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="77e2a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77e2a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="77e2a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="77e2a-111">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77e2a-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="77e2a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="77e2a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77e2a-113">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="77e2a-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="77e2a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="77e2a-114">Application</span></span> | <span data-ttu-id="77e2a-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77e2a-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="77e2a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="77e2a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}
GET /groups/{id}/onenote/notebooks/{id}
GET /sites/{id}/onenote/notebooks/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="77e2a-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="77e2a-117">Optional query parameters</span></span>
<span data-ttu-id="77e2a-118">このメソッドは、 `select`応答`expand`をカスタマイズするためのおよび[OData クエリパラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="77e2a-118">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="77e2a-119">ノートブックの有効な `expand` 値は `sections` および `sectionGroups` です。</span><span class="sxs-lookup"><span data-stu-id="77e2a-119">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="77e2a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="77e2a-120">Request headers</span></span>
| <span data-ttu-id="77e2a-121">名前</span><span class="sxs-lookup"><span data-stu-id="77e2a-121">Name</span></span>       | <span data-ttu-id="77e2a-122">型</span><span class="sxs-lookup"><span data-stu-id="77e2a-122">Type</span></span> | <span data-ttu-id="77e2a-123">説明</span><span class="sxs-lookup"><span data-stu-id="77e2a-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="77e2a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="77e2a-124">Authorization</span></span>  | <span data-ttu-id="77e2a-125">string</span><span class="sxs-lookup"><span data-stu-id="77e2a-125">string</span></span>  | <span data-ttu-id="77e2a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="77e2a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="77e2a-128">承諾</span><span class="sxs-lookup"><span data-stu-id="77e2a-128">Accept</span></span> | <span data-ttu-id="77e2a-129">string</span><span class="sxs-lookup"><span data-stu-id="77e2a-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="77e2a-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="77e2a-130">Request body</span></span>
<span data-ttu-id="77e2a-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="77e2a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77e2a-132">応答</span><span class="sxs-lookup"><span data-stu-id="77e2a-132">Response</span></span>

<span data-ttu-id="77e2a-133">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[notebook](../resources/notebook.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="77e2a-133">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="77e2a-134">例</span><span class="sxs-lookup"><span data-stu-id="77e2a-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="77e2a-135">要求</span><span class="sxs-lookup"><span data-stu-id="77e2a-135">Request</span></span>
<span data-ttu-id="77e2a-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="77e2a-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebook"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}
```
##### <a name="response"></a><span data-ttu-id="77e2a-137">応答</span><span class="sxs-lookup"><span data-stu-id="77e2a-137">Response</span></span>
<span data-ttu-id="77e2a-p103">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="77e2a-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 284

{
  "isDefault": true,
  "userRole": {
  },
  "isShared": true,
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="77e2a-141">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="77e2a-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="77e2a-142">C#</span><span class="sxs-lookup"><span data-stu-id="77e2a-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_notebook-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="77e2a-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="77e2a-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_notebook-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="77e2a-144">目的-C</span><span class="sxs-lookup"><span data-stu-id="77e2a-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_notebook-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/notebook-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/notebook-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/notebook-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
