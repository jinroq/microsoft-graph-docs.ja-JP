---
title: ノートブックを一覧表示する
description: ノートブック オブジェクトの一覧を取得します。
author: Jewan-microsoft
ms.openlocfilehash: c5925d858b7cbd567b018bd5d8491f2f20b33f66
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309829"
---
# <a name="list-notebooks"></a><span data-ttu-id="c5a5c-103">ノートブックを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c5a5c-103">List notebooks</span></span>

<span data-ttu-id="c5a5c-104">[ノートブック](../resources/notebook.md) オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="c5a5c-104">Retrieve a list of [notebook](../resources/notebook.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="c5a5c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c5a5c-105">Permissions</span></span>
<span data-ttu-id="c5a5c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c5a5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5a5c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c5a5c-108">Permission type</span></span>      | <span data-ttu-id="c5a5c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c5a5c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5a5c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c5a5c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c5a5c-111">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5a5c-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="c5a5c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c5a5c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5a5c-113">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5a5c-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="c5a5c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c5a5c-114">Application</span></span> | <span data-ttu-id="c5a5c-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5a5c-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5a5c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c5a5c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks
GET /users/{id | userPrincipalName}/onenote/notebooks
GET /groups/{id}/onenote/notebooks
GET /sites/{id}/onenote/notebooks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c5a5c-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c5a5c-117">Optional query parameters</span></span>
<span data-ttu-id="c5a5c-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c5a5c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="c5a5c-119">既定の並べ替え順序は `name asc` です。</span><span class="sxs-lookup"><span data-stu-id="c5a5c-119">The default sort order is `name asc`.</span></span> 

<span data-ttu-id="c5a5c-120">ノートブックの有効な `expand` 値は `sections` および `sectionGroups` です。</span><span class="sxs-lookup"><span data-stu-id="c5a5c-120">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5a5c-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c5a5c-121">Request headers</span></span>
| <span data-ttu-id="c5a5c-122">名前</span><span class="sxs-lookup"><span data-stu-id="c5a5c-122">Name</span></span>       | <span data-ttu-id="c5a5c-123">種類</span><span class="sxs-lookup"><span data-stu-id="c5a5c-123">Type</span></span> | <span data-ttu-id="c5a5c-124">説明</span><span class="sxs-lookup"><span data-stu-id="c5a5c-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c5a5c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5a5c-125">Authorization</span></span>  | <span data-ttu-id="c5a5c-126">string</span><span class="sxs-lookup"><span data-stu-id="c5a5c-126">string</span></span>  | <span data-ttu-id="c5a5c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c5a5c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c5a5c-129">承諾</span><span class="sxs-lookup"><span data-stu-id="c5a5c-129">Accept</span></span> | <span data-ttu-id="c5a5c-130">string</span><span class="sxs-lookup"><span data-stu-id="c5a5c-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="c5a5c-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="c5a5c-131">Request body</span></span>
<span data-ttu-id="c5a5c-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c5a5c-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5a5c-133">応答</span><span class="sxs-lookup"><span data-stu-id="c5a5c-133">Response</span></span>

<span data-ttu-id="c5a5c-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [notebook](../resources/notebook.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="c5a5c-134">If successful, this method returns a `200 OK` response code and collection of [notebook](../resources/notebook.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c5a5c-135">例</span><span class="sxs-lookup"><span data-stu-id="c5a5c-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c5a5c-136">要求</span><span class="sxs-lookup"><span data-stu-id="c5a5c-136">Request</span></span>
<span data-ttu-id="c5a5c-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c5a5c-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebooks"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks
```
##### <a name="response"></a><span data-ttu-id="c5a5c-138">応答</span><span class="sxs-lookup"><span data-stu-id="c5a5c-138">Response</span></span>
<span data-ttu-id="c5a5c-p103">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c5a5c-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List notebooks",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->