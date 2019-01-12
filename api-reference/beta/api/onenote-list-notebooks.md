---
title: ノートブックを一覧表示する
description: ノートブック オブジェクトの一覧を取得します。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: e6dca171be7c19ab3e70813fcfe21016c73faf77
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929019"
---
# <a name="list-notebooks"></a><span data-ttu-id="a2034-103">ノートブックを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a2034-103">List notebooks</span></span>

> <span data-ttu-id="a2034-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a2034-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2034-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2034-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a2034-106">[ノートブック](../resources/notebook.md) オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="a2034-106">Retrieve a list of [notebook](../resources/notebook.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="a2034-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a2034-107">Permissions</span></span>
<span data-ttu-id="a2034-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2034-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2034-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a2034-110">Permission type</span></span>      | <span data-ttu-id="a2034-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a2034-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2034-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a2034-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a2034-113">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2034-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="a2034-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a2034-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2034-115">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2034-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="a2034-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a2034-116">Application</span></span> | <span data-ttu-id="a2034-117">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2034-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2034-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a2034-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks
GET /users/{id | userPrincipalName}/onenote/notebooks
GET /groups/{id}/onenote/notebooks
GET /sites/{id}/onenote/notebooks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a2034-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a2034-119">Optional query parameters</span></span>
<span data-ttu-id="a2034-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a2034-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="a2034-121">既定の並べ替え順序は `name asc` です。</span><span class="sxs-lookup"><span data-stu-id="a2034-121">The default sort order is `name asc`.</span></span> 

<span data-ttu-id="a2034-122">ノートブックの有効な `expand` 値は `sections` および `sectionGroups` です。</span><span class="sxs-lookup"><span data-stu-id="a2034-122">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2034-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2034-123">Request headers</span></span>
| <span data-ttu-id="a2034-124">名前</span><span class="sxs-lookup"><span data-stu-id="a2034-124">Name</span></span>       | <span data-ttu-id="a2034-125">種類</span><span class="sxs-lookup"><span data-stu-id="a2034-125">Type</span></span> | <span data-ttu-id="a2034-126">説明</span><span class="sxs-lookup"><span data-stu-id="a2034-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a2034-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2034-127">Authorization</span></span>  | <span data-ttu-id="a2034-128">string</span><span class="sxs-lookup"><span data-stu-id="a2034-128">string</span></span>  | <span data-ttu-id="a2034-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a2034-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a2034-131">承諾</span><span class="sxs-lookup"><span data-stu-id="a2034-131">Accept</span></span> | <span data-ttu-id="a2034-132">string</span><span class="sxs-lookup"><span data-stu-id="a2034-132">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="a2034-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="a2034-133">Request body</span></span>
<span data-ttu-id="a2034-134">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a2034-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2034-135">応答</span><span class="sxs-lookup"><span data-stu-id="a2034-135">Response</span></span>

<span data-ttu-id="a2034-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [notebook](../resources/notebook.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a2034-136">If successful, this method returns a `200 OK` response code and collection of [notebook](../resources/notebook.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a2034-137">例</span><span class="sxs-lookup"><span data-stu-id="a2034-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a2034-138">要求</span><span class="sxs-lookup"><span data-stu-id="a2034-138">Request</span></span>
<span data-ttu-id="a2034-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a2034-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebooks"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/notebooks
```
##### <a name="response"></a><span data-ttu-id="a2034-140">応答</span><span class="sxs-lookup"><span data-stu-id="a2034-140">Response</span></span>
<span data-ttu-id="a2034-p104">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a2034-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List notebooks",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
