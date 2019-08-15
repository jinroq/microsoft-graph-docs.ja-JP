---
title: SectionGroups を一覧表示する
description: 指定されたセクショングループからセクショングループの一覧を取得します。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 9500d82e9f9b1dc4010b53225c49ab946c3a2130
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410487"
---
# <a name="list-sectiongroups"></a><span data-ttu-id="7b077-103">SectionGroups を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7b077-103">List sectionGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b077-104">指定されたセクショングループから[セクショングループ](../resources/sectiongroup.md)の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="7b077-104">Retrieve a list of [section groups](../resources/sectiongroup.md) from the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="7b077-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7b077-105">Permissions</span></span>
<span data-ttu-id="7b077-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7b077-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b077-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7b077-108">Permission type</span></span>      | <span data-ttu-id="7b077-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7b077-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b077-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7b077-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7b077-111">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b077-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="7b077-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7b077-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b077-113">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7b077-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="7b077-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7b077-114">Application</span></span> | <span data-ttu-id="7b077-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b077-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b077-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7b077-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}/sectionGroups
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sectionGroups
GET /groups/{id}/onenote/sectionGroups/{id}/sectionGroups
GET /sites/{id}/onenote/sectionGroups/{id}/sectionGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7b077-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7b077-117">Optional query parameters</span></span>
<span data-ttu-id="7b077-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7b077-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="7b077-119">既定の並べ替え順序は `name asc` です。</span><span class="sxs-lookup"><span data-stu-id="7b077-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="7b077-120">既定のクエリは`parentNotebook` 、、 `id` `displayName`、および`self`プロパティを展開して選択します。</span><span class="sxs-lookup"><span data-stu-id="7b077-120">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="7b077-121">セクション`expand`グループの有効な値`sections`は`sectionGroups`、 `parentNotebook`、、 `parentSectionGroup`、です。</span><span class="sxs-lookup"><span data-stu-id="7b077-121">Valid `expand` values for section groups are `sections`, `sectionGroups`, `parentNotebook`, and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b077-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7b077-122">Request headers</span></span>
| <span data-ttu-id="7b077-123">名前</span><span class="sxs-lookup"><span data-stu-id="7b077-123">Name</span></span>       | <span data-ttu-id="7b077-124">型</span><span class="sxs-lookup"><span data-stu-id="7b077-124">Type</span></span> | <span data-ttu-id="7b077-125">説明</span><span class="sxs-lookup"><span data-stu-id="7b077-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7b077-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b077-126">Authorization</span></span>  | <span data-ttu-id="7b077-127">string</span><span class="sxs-lookup"><span data-stu-id="7b077-127">string</span></span>  | <span data-ttu-id="7b077-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7b077-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7b077-130">承諾</span><span class="sxs-lookup"><span data-stu-id="7b077-130">Accept</span></span> | <span data-ttu-id="7b077-131">string</span><span class="sxs-lookup"><span data-stu-id="7b077-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="7b077-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="7b077-132">Request body</span></span>
<span data-ttu-id="7b077-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7b077-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b077-134">応答</span><span class="sxs-lookup"><span data-stu-id="7b077-134">Response</span></span>

<span data-ttu-id="7b077-135">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[sectionGroup](../resources/sectiongroup.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="7b077-135">If successful, this method returns a `200 OK` response code and a collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7b077-136">例</span><span class="sxs-lookup"><span data-stu-id="7b077-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7b077-137">要求</span><span class="sxs-lookup"><span data-stu-id="7b077-137">Request</span></span>
<span data-ttu-id="7b077-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7b077-138">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7b077-139">プロトコル</span><span class="sxs-lookup"><span data-stu-id="7b077-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_sectiongroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}/sectionGroups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7b077-140">C#</span><span class="sxs-lookup"><span data-stu-id="7b077-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-sectiongroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7b077-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b077-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-sectiongroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7b077-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="7b077-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-sectiongroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7b077-143">応答</span><span class="sxs-lookup"><span data-stu-id="7b077-143">Response</span></span>
<span data-ttu-id="7b077-p104">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7b077-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List sectionGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
