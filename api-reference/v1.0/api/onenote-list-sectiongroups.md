---
title: sectionGroups を一覧表示する
description: sectionGroup オブジェクトの一覧を取得します。
author: Jewan-microsoft
ms.openlocfilehash: 3f33f8b7b35cb5b1d4408b0a8f2ec6e4c968bfc9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341500"
---
# <a name="list-sectiongroups"></a><span data-ttu-id="a090d-103">sectionGroups を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a090d-103">List sectionGroups</span></span>

<span data-ttu-id="a090d-104">[sectionGroup](../resources/sectiongroup.md) オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="a090d-104">Retrieve a list of [sectionGroup](../resources/sectiongroup.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="a090d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a090d-105">Permissions</span></span>
<span data-ttu-id="a090d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a090d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a090d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a090d-108">Permission type</span></span>      | <span data-ttu-id="a090d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a090d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a090d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a090d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a090d-111">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a090d-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="a090d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a090d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a090d-113">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a090d-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="a090d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a090d-114">Application</span></span> | <span data-ttu-id="a090d-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a090d-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a090d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a090d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups
GET /users/{id | userPrincipalName}/onenote/sectionGroups
GET /groups/{id}/onenote/sectionGroups
GET /sites/{id}/onenote/sectionGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a090d-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a090d-117">Optional query parameters</span></span>
<span data-ttu-id="a090d-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a090d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="a090d-119">既定の並べ替え順序は `name asc` です。</span><span class="sxs-lookup"><span data-stu-id="a090d-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="a090d-p102">既定のクエリが `parentNotebook` を展開し、`id`、`displayName`、`self` プロパティを選択します。セクション グループで有効な `expand` 値は、`sections`、`sectionGroups`、`parentNotebook`、`parentSectionGroup` です。</span><span class="sxs-lookup"><span data-stu-id="a090d-p102">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for section groups are `sections`, `sectionGroups`, `parentNotebook`, and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a090d-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a090d-122">Request headers</span></span>
| <span data-ttu-id="a090d-123">名前</span><span class="sxs-lookup"><span data-stu-id="a090d-123">Name</span></span>       | <span data-ttu-id="a090d-124">種類</span><span class="sxs-lookup"><span data-stu-id="a090d-124">Type</span></span> | <span data-ttu-id="a090d-125">説明</span><span class="sxs-lookup"><span data-stu-id="a090d-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a090d-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a090d-126">Authorization</span></span>  | <span data-ttu-id="a090d-127">string</span><span class="sxs-lookup"><span data-stu-id="a090d-127">string</span></span>  | <span data-ttu-id="a090d-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a090d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a090d-130">承諾</span><span class="sxs-lookup"><span data-stu-id="a090d-130">Accept</span></span> | <span data-ttu-id="a090d-131">string</span><span class="sxs-lookup"><span data-stu-id="a090d-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="a090d-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="a090d-132">Request body</span></span>
<span data-ttu-id="a090d-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a090d-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a090d-134">応答</span><span class="sxs-lookup"><span data-stu-id="a090d-134">Response</span></span>

<span data-ttu-id="a090d-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [sectionGroup](../resources/sectiongroup.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a090d-135">If successful, this method returns a `200 OK` response code and collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a090d-136">例</span><span class="sxs-lookup"><span data-stu-id="a090d-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a090d-137">要求</span><span class="sxs-lookup"><span data-stu-id="a090d-137">Request</span></span>
<span data-ttu-id="a090d-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a090d-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroups"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sectionGroups
```
##### <a name="response"></a><span data-ttu-id="a090d-139">応答</span><span class="sxs-lookup"><span data-stu-id="a090d-139">Response</span></span>
<span data-ttu-id="a090d-p104">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a090d-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List sectionGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->