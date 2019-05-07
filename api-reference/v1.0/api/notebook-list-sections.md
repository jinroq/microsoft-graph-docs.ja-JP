---
title: セクションを一覧表示する
description: 指定されたノートブックから onenoteSection オブジェクトのリストを取得します。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: ae0101c0d53f3a61d07cb83fe9297323272f6ef7
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33612019"
---
# <a name="list-sections"></a><span data-ttu-id="3a5ed-103">セクションを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="3a5ed-103">List sections</span></span>

<span data-ttu-id="3a5ed-104">指定されたノートブックから[onenoteSection](../resources/section.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="3a5ed-104">Retrieve a list of [onenoteSection](../resources/section.md) objects from the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="3a5ed-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3a5ed-105">Permissions</span></span>
<span data-ttu-id="3a5ed-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3a5ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a5ed-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3a5ed-108">Permission type</span></span>      | <span data-ttu-id="3a5ed-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3a5ed-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a5ed-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3a5ed-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3a5ed-111">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a5ed-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="3a5ed-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3a5ed-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a5ed-113">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a5ed-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="3a5ed-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3a5ed-114">Application</span></span> | <span data-ttu-id="3a5ed-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a5ed-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a5ed-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3a5ed-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}/sections
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}/sections
GET /groups/{id}/onenote/notebooks/{id}/sections
GET /sites/{id}/onenote/notebooks/{id}/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3a5ed-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3a5ed-117">Optional query parameters</span></span>
<span data-ttu-id="3a5ed-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3a5ed-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="3a5ed-119">既定の並べ替え順序は `name asc` です。</span><span class="sxs-lookup"><span data-stu-id="3a5ed-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="3a5ed-120">既定のクエリは`parentNotebook` 、、 `id` `displayName`、および`self`プロパティを展開して選択します。</span><span class="sxs-lookup"><span data-stu-id="3a5ed-120">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="3a5ed-121">セクション`expand`の有効な値`parentNotebook`は`parentSectionGroup`、とです。</span><span class="sxs-lookup"><span data-stu-id="3a5ed-121">Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="3a5ed-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3a5ed-122">Request headers</span></span>
| <span data-ttu-id="3a5ed-123">名前</span><span class="sxs-lookup"><span data-stu-id="3a5ed-123">Name</span></span>       | <span data-ttu-id="3a5ed-124">型</span><span class="sxs-lookup"><span data-stu-id="3a5ed-124">Type</span></span> | <span data-ttu-id="3a5ed-125">説明</span><span class="sxs-lookup"><span data-stu-id="3a5ed-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3a5ed-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a5ed-126">Authorization</span></span>  | <span data-ttu-id="3a5ed-127">string</span><span class="sxs-lookup"><span data-stu-id="3a5ed-127">string</span></span>  | <span data-ttu-id="3a5ed-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3a5ed-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3a5ed-130">承諾</span><span class="sxs-lookup"><span data-stu-id="3a5ed-130">Accept</span></span> | <span data-ttu-id="3a5ed-131">string</span><span class="sxs-lookup"><span data-stu-id="3a5ed-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="3a5ed-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="3a5ed-132">Request body</span></span>
<span data-ttu-id="3a5ed-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3a5ed-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a5ed-134">応答</span><span class="sxs-lookup"><span data-stu-id="3a5ed-134">Response</span></span>

<span data-ttu-id="3a5ed-135">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[onenoteSection](../resources/section.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="3a5ed-135">If successful, this method returns a `200 OK` response code and a collection of [onenoteSection](../resources/section.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3a5ed-136">例</span><span class="sxs-lookup"><span data-stu-id="3a5ed-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a5ed-137">要求</span><span class="sxs-lookup"><span data-stu-id="3a5ed-137">Request</span></span>
<span data-ttu-id="3a5ed-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3a5ed-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sections"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sections
```
##### <a name="response"></a><span data-ttu-id="3a5ed-139">応答</span><span class="sxs-lookup"><span data-stu-id="3a5ed-139">Response</span></span>
<span data-ttu-id="3a5ed-p104">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="3a5ed-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 345

{
  "value": [
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
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3a5ed-143">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="3a5ed-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3a5ed-144">Visual</span><span class="sxs-lookup"><span data-stu-id="3a5ed-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_sections-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3a5ed-145">Java</span><span class="sxs-lookup"><span data-stu-id="3a5ed-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_sections-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List sections",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/notebook-list-sections.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/notebook-list-sections.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
