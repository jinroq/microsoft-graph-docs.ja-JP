---
title: sectionGroups を一覧表示する
description: sectionGroup オブジェクトの一覧を取得します。
ms.openlocfilehash: c81d216917fef7032c210490ac6ba3a0ef922a30
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074511"
---
# <a name="list-sectiongroups"></a><span data-ttu-id="35569-103">sectionGroups を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="35569-103">List sectionGroups</span></span>

> <span data-ttu-id="35569-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="35569-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35569-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="35569-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="35569-106">[sectionGroup](../resources/sectiongroup.md) オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="35569-106">Retrieve a list of [sectionGroup](../resources/sectiongroup.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="35569-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="35569-107">Permissions</span></span>
<span data-ttu-id="35569-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="35569-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35569-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="35569-110">Permission type</span></span>      | <span data-ttu-id="35569-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="35569-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35569-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="35569-112">Delegated (work or school account)</span></span> | <span data-ttu-id="35569-113">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35569-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="35569-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="35569-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35569-115">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35569-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="35569-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="35569-116">Application</span></span> | <span data-ttu-id="35569-117">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35569-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="35569-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="35569-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups
GET /users/{id | userPrincipalName}/onenote/sectionGroups
GET /groups/{id}/onenote/sectionGroups
GET /sites/{id}/onenote/sectionGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="35569-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="35569-119">Optional query parameters</span></span>
<span data-ttu-id="35569-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="35569-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="35569-121">既定の並べ替え順序は `name asc` です。</span><span class="sxs-lookup"><span data-stu-id="35569-121">The default sort order is `name asc`.</span></span>

<span data-ttu-id="35569-p103">既定のクエリが `parentNotebook` を展開し、`id`、`displayName`、`self` プロパティを選択します。セクション グループで有効な `expand` 値は、`sections`、`sectionGroups`、`parentNotebook`、`parentSectionGroup` です。</span><span class="sxs-lookup"><span data-stu-id="35569-p103">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for section groups are `sections`, `sectionGroups`, `parentNotebook`, and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="35569-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="35569-124">Request headers</span></span>
| <span data-ttu-id="35569-125">名前</span><span class="sxs-lookup"><span data-stu-id="35569-125">Name</span></span>       | <span data-ttu-id="35569-126">型</span><span class="sxs-lookup"><span data-stu-id="35569-126">Type</span></span> | <span data-ttu-id="35569-127">説明</span><span class="sxs-lookup"><span data-stu-id="35569-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="35569-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="35569-128">Authorization</span></span>  | <span data-ttu-id="35569-129">string</span><span class="sxs-lookup"><span data-stu-id="35569-129">string</span></span>  | <span data-ttu-id="35569-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="35569-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="35569-132">承諾</span><span class="sxs-lookup"><span data-stu-id="35569-132">Accept</span></span> | <span data-ttu-id="35569-133">string</span><span class="sxs-lookup"><span data-stu-id="35569-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="35569-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="35569-134">Request body</span></span>
<span data-ttu-id="35569-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="35569-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35569-136">応答</span><span class="sxs-lookup"><span data-stu-id="35569-136">Response</span></span>

<span data-ttu-id="35569-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [sectionGroup](../resources/sectiongroup.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="35569-137">If successful, this method returns a `200 OK` response code and collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="35569-138">例</span><span class="sxs-lookup"><span data-stu-id="35569-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="35569-139">要求</span><span class="sxs-lookup"><span data-stu-id="35569-139">Request</span></span>
<span data-ttu-id="35569-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="35569-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/sectionGroups
```
##### <a name="response"></a><span data-ttu-id="35569-141">応答</span><span class="sxs-lookup"><span data-stu-id="35569-141">Response</span></span>
<span data-ttu-id="35569-p105">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="35569-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectiongroup",
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
      "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
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