---
title: ノートブックを取得する
description: ノートブック オブジェクトのプロパティとリレーションシップを取得します。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: befabbe46950b6b68819be992f0257cc121a2075
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927640"
---
# <a name="get-notebook"></a><span data-ttu-id="3ffe9-103">ノートブックを取得する</span><span class="sxs-lookup"><span data-stu-id="3ffe9-103">Get notebook</span></span>

> <span data-ttu-id="3ffe9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3ffe9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3ffe9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ffe9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3ffe9-106">[ノートブック](../resources/notebook.md) オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="3ffe9-106">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3ffe9-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3ffe9-107">Permissions</span></span>
<span data-ttu-id="3ffe9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3ffe9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ffe9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3ffe9-110">Permission type</span></span>      | <span data-ttu-id="3ffe9-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3ffe9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ffe9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3ffe9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3ffe9-113">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ffe9-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="3ffe9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3ffe9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ffe9-115">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ffe9-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="3ffe9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3ffe9-116">Application</span></span> | <span data-ttu-id="3ffe9-117">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ffe9-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ffe9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3ffe9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}
GET /groups/{id}/onenote/notebooks/{id}
GET /sites/{id}/onenote/notebooks/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3ffe9-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3ffe9-119">Optional query parameters</span></span>
<span data-ttu-id="3ffe9-120">このメソッドは、応答をカスタマイズするための `select` および `expand` [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3ffe9-120">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="3ffe9-121">ノートブックの有効な `expand` 値は `sections` および `sectionGroups` です。</span><span class="sxs-lookup"><span data-stu-id="3ffe9-121">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3ffe9-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3ffe9-122">Request headers</span></span>
| <span data-ttu-id="3ffe9-123">名前</span><span class="sxs-lookup"><span data-stu-id="3ffe9-123">Name</span></span>       | <span data-ttu-id="3ffe9-124">種類</span><span class="sxs-lookup"><span data-stu-id="3ffe9-124">Type</span></span> | <span data-ttu-id="3ffe9-125">説明</span><span class="sxs-lookup"><span data-stu-id="3ffe9-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3ffe9-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ffe9-126">Authorization</span></span>  | <span data-ttu-id="3ffe9-127">string</span><span class="sxs-lookup"><span data-stu-id="3ffe9-127">string</span></span>  | <span data-ttu-id="3ffe9-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3ffe9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3ffe9-130">承諾</span><span class="sxs-lookup"><span data-stu-id="3ffe9-130">Accept</span></span> | <span data-ttu-id="3ffe9-131">string</span><span class="sxs-lookup"><span data-stu-id="3ffe9-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="3ffe9-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="3ffe9-132">Request body</span></span>
<span data-ttu-id="3ffe9-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3ffe9-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ffe9-134">応答</span><span class="sxs-lookup"><span data-stu-id="3ffe9-134">Response</span></span>

<span data-ttu-id="3ffe9-135">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [notebook](../resources/notebook.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3ffe9-135">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3ffe9-136">例</span><span class="sxs-lookup"><span data-stu-id="3ffe9-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3ffe9-137">要求</span><span class="sxs-lookup"><span data-stu-id="3ffe9-137">Request</span></span>
<span data-ttu-id="3ffe9-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3ffe9-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebook"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/notebooks/{id}
```
##### <a name="response"></a><span data-ttu-id="3ffe9-139">応答</span><span class="sxs-lookup"><span data-stu-id="3ffe9-139">Response</span></span>
<span data-ttu-id="3ffe9-p104">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="3ffe9-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
