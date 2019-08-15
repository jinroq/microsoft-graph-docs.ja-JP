---
title: SectionGroup の取得
description: SectionGroup オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 5b716ea35847884a20493ef16ddee0817ae05fa7
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410536"
---
# <a name="get-sectiongroup"></a><span data-ttu-id="58e77-103">SectionGroup の取得</span><span class="sxs-lookup"><span data-stu-id="58e77-103">Get sectionGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58e77-104">[SectionGroup](../resources/sectiongroup.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="58e77-104">Retrieve the properties and relationships of a [sectionGroup](../resources/sectiongroup.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="58e77-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="58e77-105">Permissions</span></span>
<span data-ttu-id="58e77-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="58e77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58e77-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="58e77-108">Permission type</span></span>      | <span data-ttu-id="58e77-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="58e77-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58e77-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="58e77-110">Delegated (work or school account)</span></span> | <span data-ttu-id="58e77-111">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58e77-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="58e77-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="58e77-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58e77-113">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58e77-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="58e77-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="58e77-114">Application</span></span> | <span data-ttu-id="58e77-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58e77-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="58e77-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="58e77-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}
GET /groups/{id}/onenote/sectionGroups/{id}
GET /sites/{id}/onenote/sectionGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="58e77-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="58e77-117">Optional query parameters</span></span>
<span data-ttu-id="58e77-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="58e77-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="58e77-119">既定のクエリは`parentNotebook` 、、 `id` `name`、および`self`プロパティを展開して選択します。</span><span class="sxs-lookup"><span data-stu-id="58e77-119">The default query expands `parentNotebook` and selects its `id`, `name`, and `self` properties.</span></span> <span data-ttu-id="58e77-120">セクション`expand`グループの有効な値`parentNotebook`は`parentSectionGroup`、とです。</span><span class="sxs-lookup"><span data-stu-id="58e77-120">Valid `expand` values for section groups are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="58e77-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="58e77-121">Request headers</span></span>
| <span data-ttu-id="58e77-122">名前</span><span class="sxs-lookup"><span data-stu-id="58e77-122">Name</span></span>       | <span data-ttu-id="58e77-123">型</span><span class="sxs-lookup"><span data-stu-id="58e77-123">Type</span></span> | <span data-ttu-id="58e77-124">説明</span><span class="sxs-lookup"><span data-stu-id="58e77-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="58e77-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="58e77-125">Authorization</span></span>  | <span data-ttu-id="58e77-126">string</span><span class="sxs-lookup"><span data-stu-id="58e77-126">string</span></span>  | <span data-ttu-id="58e77-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="58e77-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="58e77-129">承諾</span><span class="sxs-lookup"><span data-stu-id="58e77-129">Accept</span></span> | <span data-ttu-id="58e77-130">string</span><span class="sxs-lookup"><span data-stu-id="58e77-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="58e77-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="58e77-131">Request body</span></span>
<span data-ttu-id="58e77-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="58e77-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58e77-133">応答</span><span class="sxs-lookup"><span data-stu-id="58e77-133">Response</span></span>

<span data-ttu-id="58e77-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [sectionGroup](../resources/sectiongroup.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="58e77-134">If successful, this method returns a `200 OK` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="58e77-135">例</span><span class="sxs-lookup"><span data-stu-id="58e77-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="58e77-136">要求</span><span class="sxs-lookup"><span data-stu-id="58e77-136">Request</span></span>
<span data-ttu-id="58e77-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="58e77-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="58e77-138">プロトコル</span><span class="sxs-lookup"><span data-stu-id="58e77-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_sectiongroup"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="58e77-139">C#</span><span class="sxs-lookup"><span data-stu-id="58e77-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-sectiongroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="58e77-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58e77-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-sectiongroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="58e77-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="58e77-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-sectiongroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="58e77-142">応答</span><span class="sxs-lookup"><span data-stu-id="58e77-142">Response</span></span>
<span data-ttu-id="58e77-p104">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="58e77-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
