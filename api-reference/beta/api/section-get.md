---
title: セクションを取得する
description: Section オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: df73036ca65ce0038430aed0f0c55635f02605a7
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638859"
---
# <a name="get-section"></a><span data-ttu-id="93aca-103">セクションを取得する</span><span class="sxs-lookup"><span data-stu-id="93aca-103">Get section</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93aca-104">[Section](../resources/onenotesection.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="93aca-104">Retrieve the properties and relationships of a [section](../resources/onenotesection.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="93aca-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="93aca-105">Permissions</span></span>
<span data-ttu-id="93aca-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="93aca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93aca-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="93aca-108">Permission type</span></span>      | <span data-ttu-id="93aca-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="93aca-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93aca-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="93aca-110">Delegated (work or school account)</span></span> | <span data-ttu-id="93aca-111">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93aca-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="93aca-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="93aca-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93aca-113">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93aca-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="93aca-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="93aca-114">Application</span></span> | <span data-ttu-id="93aca-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93aca-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="93aca-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="93aca-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}
GET /users/{id | userPrincipalName}/onenote/sections/{id}
GET /groups/{id}/onenote/sections/{id}
GET /sites/{id}/onenote/sections/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="93aca-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="93aca-117">Optional query parameters</span></span>
<span data-ttu-id="93aca-118">このメソッドは、 `select`応答`expand`をカスタマイズするためのおよび[OData クエリパラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="93aca-118">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="93aca-119">既定のクエリは`parentNotebook` 、、 `id` `displayName`、および`self`プロパティを展開して選択します。</span><span class="sxs-lookup"><span data-stu-id="93aca-119">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="93aca-120">セクション`expand`の有効な値`parentNotebook`は`parentSectionGroup`、とです。</span><span class="sxs-lookup"><span data-stu-id="93aca-120">Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="93aca-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="93aca-121">Request headers</span></span>
| <span data-ttu-id="93aca-122">名前</span><span class="sxs-lookup"><span data-stu-id="93aca-122">Name</span></span>       | <span data-ttu-id="93aca-123">型</span><span class="sxs-lookup"><span data-stu-id="93aca-123">Type</span></span> | <span data-ttu-id="93aca-124">説明</span><span class="sxs-lookup"><span data-stu-id="93aca-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="93aca-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="93aca-125">Authorization</span></span>  | <span data-ttu-id="93aca-126">string</span><span class="sxs-lookup"><span data-stu-id="93aca-126">string</span></span>  | <span data-ttu-id="93aca-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="93aca-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="93aca-129">承諾</span><span class="sxs-lookup"><span data-stu-id="93aca-129">Accept</span></span> | <span data-ttu-id="93aca-130">string</span><span class="sxs-lookup"><span data-stu-id="93aca-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="93aca-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="93aca-131">Request body</span></span>
<span data-ttu-id="93aca-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="93aca-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93aca-133">応答</span><span class="sxs-lookup"><span data-stu-id="93aca-133">Response</span></span>

<span data-ttu-id="93aca-134">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[onenoteSection](../resources/onenotesection.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="93aca-134">If successful, this method returns a `200 OK` response code and a [onenoteSection](../resources/onenotesection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="93aca-135">例</span><span class="sxs-lookup"><span data-stu-id="93aca-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93aca-136">要求</span><span class="sxs-lookup"><span data-stu-id="93aca-136">Request</span></span>
<span data-ttu-id="93aca-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="93aca-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_section"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/sections/{id}
```
##### <a name="response"></a><span data-ttu-id="93aca-138">応答</span><span class="sxs-lookup"><span data-stu-id="93aca-138">Response</span></span>
<span data-ttu-id="93aca-p104">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="93aca-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 272

{
  "isDefault": true,
  "pagesUrl": "pagesUrl-value",
  "displayName": "name-value",
  "createdBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  },
  "lastModifiedBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="93aca-142">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="93aca-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="93aca-143">Visual</span><span class="sxs-lookup"><span data-stu-id="93aca-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_section-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="93aca-144">Java</span><span class="sxs-lookup"><span data-stu-id="93aca-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_section-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get section",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/section-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/section-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
