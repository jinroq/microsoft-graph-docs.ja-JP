---
title: セクションを取得する
description: OnenoteSection オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 8f1a66c85835fab94541553843e45109f61e4bf5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35461520"
---
# <a name="get-section"></a><span data-ttu-id="c3cb3-103">セクションを取得する</span><span class="sxs-lookup"><span data-stu-id="c3cb3-103">Get section</span></span>

<span data-ttu-id="c3cb3-104">[OnenoteSection](../resources/section.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="c3cb3-104">Retrieve the properties and relationships of a [onenoteSection](../resources/section.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c3cb3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c3cb3-105">Permissions</span></span>
<span data-ttu-id="c3cb3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c3cb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3cb3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c3cb3-108">Permission type</span></span>      | <span data-ttu-id="c3cb3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c3cb3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3cb3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c3cb3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c3cb3-111">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3cb3-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="c3cb3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c3cb3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3cb3-113">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c3cb3-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="c3cb3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c3cb3-114">Application</span></span> | <span data-ttu-id="c3cb3-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3cb3-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3cb3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c3cb3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}
GET /users/{id | userPrincipalName}/onenote/sections/{id}
GET /groups/{id}/onenote/sections/{id}
GET /sites/{id}/onenote/sections/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c3cb3-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c3cb3-117">Optional query parameters</span></span>
<span data-ttu-id="c3cb3-118">このメソッドは、 `select`応答`expand`をカスタマイズするためのおよび[OData クエリパラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c3cb3-118">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="c3cb3-119">既定のクエリは`parentNotebook` 、、 `id` `displayName`、および`self`プロパティを展開して選択します。</span><span class="sxs-lookup"><span data-stu-id="c3cb3-119">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="c3cb3-120">セクション`expand`の有効な値`parentNotebook`は`parentSectionGroup`、とです。</span><span class="sxs-lookup"><span data-stu-id="c3cb3-120">Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3cb3-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3cb3-121">Request headers</span></span>
| <span data-ttu-id="c3cb3-122">名前</span><span class="sxs-lookup"><span data-stu-id="c3cb3-122">Name</span></span>       | <span data-ttu-id="c3cb3-123">型</span><span class="sxs-lookup"><span data-stu-id="c3cb3-123">Type</span></span> | <span data-ttu-id="c3cb3-124">説明</span><span class="sxs-lookup"><span data-stu-id="c3cb3-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c3cb3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3cb3-125">Authorization</span></span>  | <span data-ttu-id="c3cb3-126">string</span><span class="sxs-lookup"><span data-stu-id="c3cb3-126">string</span></span>  | <span data-ttu-id="c3cb3-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c3cb3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c3cb3-129">承諾</span><span class="sxs-lookup"><span data-stu-id="c3cb3-129">Accept</span></span> | <span data-ttu-id="c3cb3-130">string</span><span class="sxs-lookup"><span data-stu-id="c3cb3-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="c3cb3-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="c3cb3-131">Request body</span></span>
<span data-ttu-id="c3cb3-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c3cb3-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3cb3-133">応答</span><span class="sxs-lookup"><span data-stu-id="c3cb3-133">Response</span></span>

<span data-ttu-id="c3cb3-134">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[onenoteSection](../resources/section.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c3cb3-134">If successful, this method returns a `200 OK` response code and a [onenoteSection](../resources/section.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c3cb3-135">例</span><span class="sxs-lookup"><span data-stu-id="c3cb3-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c3cb3-136">要求</span><span class="sxs-lookup"><span data-stu-id="c3cb3-136">Request</span></span>
<span data-ttu-id="c3cb3-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c3cb3-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c3cb3-138">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c3cb3-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_section"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sections/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c3cb3-139">C#</span><span class="sxs-lookup"><span data-stu-id="c3cb3-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-section-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c3cb3-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="c3cb3-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-section-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c3cb3-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="c3cb3-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-section-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c3cb3-142">応答</span><span class="sxs-lookup"><span data-stu-id="c3cb3-142">Response</span></span>
<span data-ttu-id="c3cb3-p104">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c3cb3-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get section",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
