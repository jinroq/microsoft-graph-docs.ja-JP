---
title: セクションを一覧表示する
description: 指定されたセクション グループからセクション オブジェクトの一覧を取得します。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 66ffe610df5479eac78a943b1eefac0a41ecd37e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953358"
---
# <a name="list-sections"></a><span data-ttu-id="66dad-103">セクションを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="66dad-103">List sections</span></span>

> <span data-ttu-id="66dad-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="66dad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66dad-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66dad-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="66dad-106">指定されたセクション グループから[セクション](../resources/section.md) オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="66dad-106">Retrieve a list of [section](../resources/section.md) objects from the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="66dad-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="66dad-107">Permissions</span></span>
<span data-ttu-id="66dad-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="66dad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66dad-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="66dad-110">Permission type</span></span>      | <span data-ttu-id="66dad-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="66dad-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66dad-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="66dad-112">Delegated (work or school account)</span></span> | <span data-ttu-id="66dad-113">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66dad-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="66dad-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="66dad-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66dad-115">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66dad-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="66dad-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="66dad-116">Application</span></span> | <span data-ttu-id="66dad-117">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66dad-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="66dad-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="66dad-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}/sections
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sections
GET /groups/{id}/onenote/sectionGroups/{id}/sections
GET /sites/{id}/onenote/sectionGroups/{id}/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="66dad-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="66dad-119">Optional query parameters</span></span>
<span data-ttu-id="66dad-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="66dad-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="66dad-121">既定の並べ替え順序は `name asc` です。</span><span class="sxs-lookup"><span data-stu-id="66dad-121">The default sort order is `name asc`.</span></span>

<span data-ttu-id="66dad-p103">既定のクエリが `parentNotebook` を展開し、`id`、`displayName`、`self` プロパティを選択します。セクションの有効な `expand` 値は、`parentNotebook` と `parentSectionGroup` です。</span><span class="sxs-lookup"><span data-stu-id="66dad-p103">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="66dad-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="66dad-124">Request headers</span></span>
| <span data-ttu-id="66dad-125">名前</span><span class="sxs-lookup"><span data-stu-id="66dad-125">Name</span></span>       | <span data-ttu-id="66dad-126">型</span><span class="sxs-lookup"><span data-stu-id="66dad-126">Type</span></span> | <span data-ttu-id="66dad-127">説明</span><span class="sxs-lookup"><span data-stu-id="66dad-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="66dad-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="66dad-128">Authorization</span></span>  | <span data-ttu-id="66dad-129">string</span><span class="sxs-lookup"><span data-stu-id="66dad-129">string</span></span>  | <span data-ttu-id="66dad-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="66dad-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="66dad-132">承諾</span><span class="sxs-lookup"><span data-stu-id="66dad-132">Accept</span></span> | <span data-ttu-id="66dad-133">string</span><span class="sxs-lookup"><span data-stu-id="66dad-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="66dad-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="66dad-134">Request body</span></span>
<span data-ttu-id="66dad-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="66dad-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66dad-136">応答</span><span class="sxs-lookup"><span data-stu-id="66dad-136">Response</span></span>

<span data-ttu-id="66dad-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [section](../resources/section.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="66dad-137">If successful, this method returns a `200 OK` response code and a collection of [section](../resources/section.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="66dad-138">例</span><span class="sxs-lookup"><span data-stu-id="66dad-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="66dad-139">要求</span><span class="sxs-lookup"><span data-stu-id="66dad-139">Request</span></span>
<span data-ttu-id="66dad-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="66dad-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sections"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}/sections
```
##### <a name="response"></a><span data-ttu-id="66dad-141">応答</span><span class="sxs-lookup"><span data-stu-id="66dad-141">Response</span></span>
<span data-ttu-id="66dad-p105">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="66dad-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List sections",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
