---
title: ノートブックを一覧表示する
description: ノートブック オブジェクトの一覧を取得します。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: ffb39628bf9d2c73389835f435050b0f106e7c65
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35988931"
---
# <a name="list-notebooks"></a><span data-ttu-id="acbed-103">ノートブックを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="acbed-103">List notebooks</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acbed-104">[ノートブック](../resources/notebook.md) オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="acbed-104">Retrieve a list of [notebook](../resources/notebook.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="acbed-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="acbed-105">Permissions</span></span>
<span data-ttu-id="acbed-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="acbed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acbed-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="acbed-108">Permission type</span></span>      | <span data-ttu-id="acbed-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="acbed-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="acbed-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="acbed-110">Delegated (work or school account)</span></span> | <span data-ttu-id="acbed-111">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acbed-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="acbed-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="acbed-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="acbed-113">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="acbed-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="acbed-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="acbed-114">Application</span></span> | <span data-ttu-id="acbed-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acbed-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="acbed-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="acbed-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks
GET /users/{id | userPrincipalName}/onenote/notebooks
GET /groups/{id}/onenote/notebooks
GET /sites/{id}/onenote/notebooks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="acbed-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="acbed-117">Optional query parameters</span></span>
<span data-ttu-id="acbed-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="acbed-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="acbed-119">既定の並べ替え順序は `name asc` です。</span><span class="sxs-lookup"><span data-stu-id="acbed-119">The default sort order is `name asc`.</span></span> 

<span data-ttu-id="acbed-120">ノートブックの有効な `expand` 値は `sections` および `sectionGroups` です。</span><span class="sxs-lookup"><span data-stu-id="acbed-120">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="acbed-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="acbed-121">Request headers</span></span>
| <span data-ttu-id="acbed-122">名前</span><span class="sxs-lookup"><span data-stu-id="acbed-122">Name</span></span>       | <span data-ttu-id="acbed-123">型</span><span class="sxs-lookup"><span data-stu-id="acbed-123">Type</span></span> | <span data-ttu-id="acbed-124">説明</span><span class="sxs-lookup"><span data-stu-id="acbed-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="acbed-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="acbed-125">Authorization</span></span>  | <span data-ttu-id="acbed-126">string</span><span class="sxs-lookup"><span data-stu-id="acbed-126">string</span></span>  | <span data-ttu-id="acbed-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="acbed-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="acbed-129">承諾</span><span class="sxs-lookup"><span data-stu-id="acbed-129">Accept</span></span> | <span data-ttu-id="acbed-130">string</span><span class="sxs-lookup"><span data-stu-id="acbed-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="acbed-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="acbed-131">Request body</span></span>
<span data-ttu-id="acbed-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="acbed-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="acbed-133">応答</span><span class="sxs-lookup"><span data-stu-id="acbed-133">Response</span></span>

<span data-ttu-id="acbed-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [notebook](../resources/notebook.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="acbed-134">If successful, this method returns a `200 OK` response code and collection of [notebook](../resources/notebook.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="acbed-135">例</span><span class="sxs-lookup"><span data-stu-id="acbed-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="acbed-136">要求</span><span class="sxs-lookup"><span data-stu-id="acbed-136">Request</span></span>
<span data-ttu-id="acbed-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="acbed-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="acbed-138">プロトコル</span><span class="sxs-lookup"><span data-stu-id="acbed-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_notebooks"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/notebooks
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="acbed-139">C#</span><span class="sxs-lookup"><span data-stu-id="acbed-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-notebooks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="acbed-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="acbed-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-notebooks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="acbed-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="acbed-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-notebooks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="acbed-142">Java</span><span class="sxs-lookup"><span data-stu-id="acbed-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-notebooks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="acbed-143">応答</span><span class="sxs-lookup"><span data-stu-id="acbed-143">Response</span></span>
<span data-ttu-id="acbed-p103">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="acbed-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 369

{
  "value": [
    {
      "isDefault": true,
      "userRole": {
      },
      "isShared": true,
      "sectionsUrl": "sectionsUrl-value",
      "sectionGroupsUrl": "sectionGroupsUrl-value",
      "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
      "links": {
        "oneNoteClientUrl": {
          "href": "href-value"
        },
        "oneNoteWebUrl": {
          "href": "href-value"
        }
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List notebooks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
