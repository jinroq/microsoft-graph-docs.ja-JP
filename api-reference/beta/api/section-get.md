---
title: Get section
description: セクション オブジェクトのプロパティとリレーションシップを取得します。
ms.openlocfilehash: e4e46a220e02b5fe98e18a1f62125c7697efe052
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066747"
---
# <a name="get-section"></a><span data-ttu-id="19953-103">Get section</span><span class="sxs-lookup"><span data-stu-id="19953-103">Get section</span></span>

> <span data-ttu-id="19953-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="19953-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19953-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19953-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="19953-106">[セクション](../resources/section.md) オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="19953-106">Retrieve the properties and relationships of a [section](../resources/section.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="19953-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="19953-107">Permissions</span></span>
<span data-ttu-id="19953-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="19953-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19953-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="19953-110">Permission type</span></span>      | <span data-ttu-id="19953-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="19953-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19953-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="19953-112">Delegated (work or school account)</span></span> | <span data-ttu-id="19953-113">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19953-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="19953-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="19953-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19953-115">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19953-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="19953-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="19953-116">Application</span></span> | <span data-ttu-id="19953-117">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19953-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="19953-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="19953-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}
GET /users/{id | userPrincipalName}/onenote/sections/{id}
GET /groups/{id}/onenote/sections/{id}
GET /sites/{id}/onenote/sections/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="19953-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="19953-119">Optional query parameters</span></span>
<span data-ttu-id="19953-120">このメソッドは、応答をカスタマイズするための `select` および `expand` [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="19953-120">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="19953-p103">既定のクエリが `parentNotebook` を展開し、`id`、`displayName`、`self` プロパティを選択します。セクションの有効な `expand` 値は、`parentNotebook` と `parentSectionGroup` です。</span><span class="sxs-lookup"><span data-stu-id="19953-p103">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="19953-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="19953-123">Request headers</span></span>
| <span data-ttu-id="19953-124">名前</span><span class="sxs-lookup"><span data-stu-id="19953-124">Name</span></span>       | <span data-ttu-id="19953-125">型</span><span class="sxs-lookup"><span data-stu-id="19953-125">Type</span></span> | <span data-ttu-id="19953-126">説明</span><span class="sxs-lookup"><span data-stu-id="19953-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="19953-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="19953-127">Authorization</span></span>  | <span data-ttu-id="19953-128">string</span><span class="sxs-lookup"><span data-stu-id="19953-128">string</span></span>  | <span data-ttu-id="19953-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="19953-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="19953-131">承諾</span><span class="sxs-lookup"><span data-stu-id="19953-131">Accept</span></span> | <span data-ttu-id="19953-132">string</span><span class="sxs-lookup"><span data-stu-id="19953-132">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="19953-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="19953-133">Request body</span></span>
<span data-ttu-id="19953-134">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="19953-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19953-135">応答</span><span class="sxs-lookup"><span data-stu-id="19953-135">Response</span></span>

<span data-ttu-id="19953-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [section](../resources/section.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="19953-136">If successful, this method returns a `200 OK` response code and a [section](../resources/section.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="19953-137">例</span><span class="sxs-lookup"><span data-stu-id="19953-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="19953-138">要求</span><span class="sxs-lookup"><span data-stu-id="19953-138">Request</span></span>
<span data-ttu-id="19953-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="19953-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_section"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/sections/{id}
```
##### <a name="response"></a><span data-ttu-id="19953-140">応答</span><span class="sxs-lookup"><span data-stu-id="19953-140">Response</span></span>
<span data-ttu-id="19953-p105">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="19953-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->