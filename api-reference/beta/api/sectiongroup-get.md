---
title: SectionGroup の取得
description: SectionGroup オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: e9fa7c67f98d8c745fe4853b28f63815a9ae4cc4
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638852"
---
# <a name="get-sectiongroup"></a><span data-ttu-id="bc7d6-103">SectionGroup の取得</span><span class="sxs-lookup"><span data-stu-id="bc7d6-103">Get sectionGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc7d6-104">[SectionGroup](../resources/sectiongroup.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="bc7d6-104">Retrieve the properties and relationships of a [sectionGroup](../resources/sectiongroup.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bc7d6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bc7d6-105">Permissions</span></span>
<span data-ttu-id="bc7d6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bc7d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc7d6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bc7d6-108">Permission type</span></span>      | <span data-ttu-id="bc7d6-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bc7d6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc7d6-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bc7d6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bc7d6-111">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc7d6-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="bc7d6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bc7d6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc7d6-113">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc7d6-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="bc7d6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bc7d6-114">Application</span></span> | <span data-ttu-id="bc7d6-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc7d6-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc7d6-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bc7d6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}
GET /groups/{id}/onenote/sectionGroups/{id}
GET /sites/{id}/onenote/sectionGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bc7d6-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="bc7d6-117">Optional query parameters</span></span>
<span data-ttu-id="bc7d6-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="bc7d6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="bc7d6-119">既定のクエリは`parentNotebook` 、、 `id` `name`、および`self`プロパティを展開して選択します。</span><span class="sxs-lookup"><span data-stu-id="bc7d6-119">The default query expands `parentNotebook` and selects its `id`, `name`, and `self` properties.</span></span> <span data-ttu-id="bc7d6-120">セクション`expand`グループの有効な値`parentNotebook`は`parentSectionGroup`、とです。</span><span class="sxs-lookup"><span data-stu-id="bc7d6-120">Valid `expand` values for section groups are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bc7d6-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bc7d6-121">Request headers</span></span>
| <span data-ttu-id="bc7d6-122">名前</span><span class="sxs-lookup"><span data-stu-id="bc7d6-122">Name</span></span>       | <span data-ttu-id="bc7d6-123">型</span><span class="sxs-lookup"><span data-stu-id="bc7d6-123">Type</span></span> | <span data-ttu-id="bc7d6-124">説明</span><span class="sxs-lookup"><span data-stu-id="bc7d6-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bc7d6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc7d6-125">Authorization</span></span>  | <span data-ttu-id="bc7d6-126">string</span><span class="sxs-lookup"><span data-stu-id="bc7d6-126">string</span></span>  | <span data-ttu-id="bc7d6-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bc7d6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bc7d6-129">承諾</span><span class="sxs-lookup"><span data-stu-id="bc7d6-129">Accept</span></span> | <span data-ttu-id="bc7d6-130">string</span><span class="sxs-lookup"><span data-stu-id="bc7d6-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="bc7d6-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="bc7d6-131">Request body</span></span>
<span data-ttu-id="bc7d6-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bc7d6-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc7d6-133">応答</span><span class="sxs-lookup"><span data-stu-id="bc7d6-133">Response</span></span>

<span data-ttu-id="bc7d6-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [sectionGroup](../resources/sectiongroup.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bc7d6-134">If successful, this method returns a `200 OK` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bc7d6-135">例</span><span class="sxs-lookup"><span data-stu-id="bc7d6-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc7d6-136">要求</span><span class="sxs-lookup"><span data-stu-id="bc7d6-136">Request</span></span>
<span data-ttu-id="bc7d6-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bc7d6-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroup"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="bc7d6-138">応答</span><span class="sxs-lookup"><span data-stu-id="bc7d6-138">Response</span></span>
<span data-ttu-id="bc7d6-p104">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="bc7d6-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectionGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

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
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bc7d6-142">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="bc7d6-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bc7d6-143">Visual</span><span class="sxs-lookup"><span data-stu-id="bc7d6-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_sectiongroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bc7d6-144">Java</span><span class="sxs-lookup"><span data-stu-id="bc7d6-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_sectiongroup-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get sectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/sectiongroup-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/sectiongroup-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
