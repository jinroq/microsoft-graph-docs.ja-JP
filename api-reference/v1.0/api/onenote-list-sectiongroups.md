---
title: SectionGroups を一覧表示する
description: SectionGroup オブジェクトの一覧を取得します。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: e1ff4b9b4a31dccaeff2b95fd0fd2242e807e6e1
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274474"
---
# <a name="list-sectiongroups"></a><span data-ttu-id="e23dc-103">SectionGroups を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e23dc-103">List sectionGroups</span></span>

<span data-ttu-id="e23dc-104">[SectionGroup](../resources/sectiongroup.md)オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="e23dc-104">Retrieve a list of [sectionGroup](../resources/sectiongroup.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="e23dc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e23dc-105">Permissions</span></span>
<span data-ttu-id="e23dc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e23dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e23dc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e23dc-108">Permission type</span></span>      | <span data-ttu-id="e23dc-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e23dc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e23dc-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e23dc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e23dc-111">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e23dc-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="e23dc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e23dc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e23dc-113">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e23dc-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="e23dc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e23dc-114">Application</span></span> | <span data-ttu-id="e23dc-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e23dc-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e23dc-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e23dc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups
GET /users/{id | userPrincipalName}/onenote/sectionGroups
GET /groups/{id}/onenote/sectionGroups
GET /sites/{id}/onenote/sectionGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e23dc-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e23dc-117">Optional query parameters</span></span>
<span data-ttu-id="e23dc-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e23dc-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="e23dc-119">既定の並べ替え順序は `name asc` です。</span><span class="sxs-lookup"><span data-stu-id="e23dc-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="e23dc-120">既定のクエリは`parentNotebook` 、、 `id` `displayName`、および`self`プロパティを展開して選択します。</span><span class="sxs-lookup"><span data-stu-id="e23dc-120">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="e23dc-121">セクション`expand`グループの有効な値`sections`は`sectionGroups`、 `parentNotebook`、、 `parentSectionGroup`、です。</span><span class="sxs-lookup"><span data-stu-id="e23dc-121">Valid `expand` values for section groups are `sections`, `sectionGroups`, `parentNotebook`, and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e23dc-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e23dc-122">Request headers</span></span>
| <span data-ttu-id="e23dc-123">名前</span><span class="sxs-lookup"><span data-stu-id="e23dc-123">Name</span></span>       | <span data-ttu-id="e23dc-124">型</span><span class="sxs-lookup"><span data-stu-id="e23dc-124">Type</span></span> | <span data-ttu-id="e23dc-125">説明</span><span class="sxs-lookup"><span data-stu-id="e23dc-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e23dc-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e23dc-126">Authorization</span></span>  | <span data-ttu-id="e23dc-127">string</span><span class="sxs-lookup"><span data-stu-id="e23dc-127">string</span></span>  | <span data-ttu-id="e23dc-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e23dc-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e23dc-130">承諾</span><span class="sxs-lookup"><span data-stu-id="e23dc-130">Accept</span></span> | <span data-ttu-id="e23dc-131">string</span><span class="sxs-lookup"><span data-stu-id="e23dc-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="e23dc-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="e23dc-132">Request body</span></span>
<span data-ttu-id="e23dc-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e23dc-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e23dc-134">応答</span><span class="sxs-lookup"><span data-stu-id="e23dc-134">Response</span></span>

<span data-ttu-id="e23dc-135">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[sectionGroup](../resources/sectiongroup.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e23dc-135">If successful, this method returns a `200 OK` response code and collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e23dc-136">例</span><span class="sxs-lookup"><span data-stu-id="e23dc-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e23dc-137">要求</span><span class="sxs-lookup"><span data-stu-id="e23dc-137">Request</span></span>
<span data-ttu-id="e23dc-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e23dc-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroups"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sectionGroups
```
##### <a name="response"></a><span data-ttu-id="e23dc-139">応答</span><span class="sxs-lookup"><span data-stu-id="e23dc-139">Response</span></span>
<span data-ttu-id="e23dc-p104">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e23dc-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectionGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 378

{
  "value": [
    {
      "sectionsUrl": "sectionsUrl-value",
      "sectionGroupsUrl": "sectionGroupsUrl-value",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e23dc-143">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="e23dc-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e23dc-144">C#</span><span class="sxs-lookup"><span data-stu-id="e23dc-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_sectiongroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e23dc-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="e23dc-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_sectiongroups-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e23dc-146">目的-C</span><span class="sxs-lookup"><span data-stu-id="e23dc-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_sectiongroups-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List sectionGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/onenote-list-sectiongroups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/onenote-list-sectiongroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/onenote-list-sectiongroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
