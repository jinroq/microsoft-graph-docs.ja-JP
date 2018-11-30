---
title: sectionGroups を一覧表示する
description: 指定されたノートブックからセクション グループの一覧を取得します。
ms.openlocfilehash: 3b1629429d18d4bb2c8e05567c8613784f8579e0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020650"
---
# <a name="list-sectiongroups"></a><span data-ttu-id="d2e7c-103">sectionGroups を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d2e7c-103">List sectionGroups</span></span>

<span data-ttu-id="d2e7c-104">指定されたノートブックから[セクション グループ](../resources/sectiongroup.md)の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="d2e7c-104">Retrieve a list of [section groups](../resources/sectiongroup.md) from the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="d2e7c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d2e7c-105">Permissions</span></span>
<span data-ttu-id="d2e7c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d2e7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2e7c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d2e7c-108">Permission type</span></span>      | <span data-ttu-id="d2e7c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d2e7c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2e7c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d2e7c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d2e7c-111">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2e7c-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="d2e7c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d2e7c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2e7c-113">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2e7c-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="d2e7c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d2e7c-114">Application</span></span> | <span data-ttu-id="d2e7c-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2e7c-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2e7c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d2e7c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}/sectionGroups
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}/sectionGroups
GET /groups/{id}/onenote/notebooks/{id}/sectionGroups
GET /sites/{id}/onenote/notebooks/{id}/sectionGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d2e7c-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d2e7c-117">Optional query parameters</span></span>
<span data-ttu-id="d2e7c-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d2e7c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="d2e7c-119">既定の並べ替え順序は `name asc` です。</span><span class="sxs-lookup"><span data-stu-id="d2e7c-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="d2e7c-p102">既定のクエリが `parentNotebook` を展開し、`id`、`displayName`、`self` プロパティを選択します。セクション グループで有効な `expand` 値は、`sections`、`sectionGroups`、`parentNotebook`、`parentSectionGroup` です。</span><span class="sxs-lookup"><span data-stu-id="d2e7c-p102">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for section groups are `sections`, `sectionGroups`, `parentNotebook`, and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2e7c-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2e7c-122">Request headers</span></span>
| <span data-ttu-id="d2e7c-123">名前</span><span class="sxs-lookup"><span data-stu-id="d2e7c-123">Name</span></span>       | <span data-ttu-id="d2e7c-124">型</span><span class="sxs-lookup"><span data-stu-id="d2e7c-124">Type</span></span> | <span data-ttu-id="d2e7c-125">説明</span><span class="sxs-lookup"><span data-stu-id="d2e7c-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d2e7c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2e7c-126">Authorization</span></span>  | <span data-ttu-id="d2e7c-127">string</span><span class="sxs-lookup"><span data-stu-id="d2e7c-127">string</span></span>  | <span data-ttu-id="d2e7c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d2e7c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d2e7c-130">承諾</span><span class="sxs-lookup"><span data-stu-id="d2e7c-130">Accept</span></span> | <span data-ttu-id="d2e7c-131">string</span><span class="sxs-lookup"><span data-stu-id="d2e7c-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="d2e7c-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="d2e7c-132">Request body</span></span>
<span data-ttu-id="d2e7c-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d2e7c-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2e7c-134">応答</span><span class="sxs-lookup"><span data-stu-id="d2e7c-134">Response</span></span>

<span data-ttu-id="d2e7c-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [sectionGroup](../resources/sectiongroup.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d2e7c-135">If successful, this method returns a `200 OK` response code and collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d2e7c-136">例</span><span class="sxs-lookup"><span data-stu-id="d2e7c-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2e7c-137">要求</span><span class="sxs-lookup"><span data-stu-id="d2e7c-137">Request</span></span>
<span data-ttu-id="d2e7c-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d2e7c-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroups"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sectionGroups
```
##### <a name="response"></a><span data-ttu-id="d2e7c-139">応答</span><span class="sxs-lookup"><span data-stu-id="d2e7c-139">Response</span></span>
<span data-ttu-id="d2e7c-p104">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d2e7c-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
