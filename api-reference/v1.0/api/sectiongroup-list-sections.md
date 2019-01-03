---
title: セクションを一覧表示する
description: 指定されたセクション グループには、onenoteSection オブジェクトの一覧を取得します。
ms.openlocfilehash: 0298293f1f82cd61d376e195360b79d4a96d5344
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022018"
---
# <a name="list-sections"></a><span data-ttu-id="45219-103">セクションを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="45219-103">List sections</span></span>

<span data-ttu-id="45219-104">指定されたセクション グループには、 [onenoteSection](../resources/section.md)オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="45219-104">Retrieve a list of [onenoteSection](../resources/section.md) objects from the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="45219-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="45219-105">Permissions</span></span>
<span data-ttu-id="45219-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="45219-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45219-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="45219-108">Permission type</span></span>      | <span data-ttu-id="45219-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="45219-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45219-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="45219-110">Delegated (work or school account)</span></span> | <span data-ttu-id="45219-111">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45219-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="45219-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="45219-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45219-113">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="45219-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="45219-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="45219-114">Application</span></span> | <span data-ttu-id="45219-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45219-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="45219-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="45219-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}/sections
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sections
GET /groups/{id}/onenote/sectionGroups/{id}/sections
GET /sites/{id}/onenote/sectionGroups/{id}/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="45219-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="45219-117">Optional query parameters</span></span>
<span data-ttu-id="45219-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="45219-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="45219-119">既定の並べ替え順序は `name asc` です。</span><span class="sxs-lookup"><span data-stu-id="45219-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="45219-p102">既定のクエリが `parentNotebook` を展開し、`id`、`displayName`、`self` プロパティを選択します。セクションの有効な `expand` 値は、`parentNotebook` と `parentSectionGroup` です。</span><span class="sxs-lookup"><span data-stu-id="45219-p102">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="45219-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="45219-122">Request headers</span></span>
| <span data-ttu-id="45219-123">名前</span><span class="sxs-lookup"><span data-stu-id="45219-123">Name</span></span>       | <span data-ttu-id="45219-124">型</span><span class="sxs-lookup"><span data-stu-id="45219-124">Type</span></span> | <span data-ttu-id="45219-125">説明</span><span class="sxs-lookup"><span data-stu-id="45219-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="45219-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="45219-126">Authorization</span></span>  | <span data-ttu-id="45219-127">string</span><span class="sxs-lookup"><span data-stu-id="45219-127">string</span></span>  | <span data-ttu-id="45219-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="45219-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="45219-130">承諾</span><span class="sxs-lookup"><span data-stu-id="45219-130">Accept</span></span> | <span data-ttu-id="45219-131">string</span><span class="sxs-lookup"><span data-stu-id="45219-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="45219-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="45219-132">Request body</span></span>
<span data-ttu-id="45219-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="45219-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45219-134">応答</span><span class="sxs-lookup"><span data-stu-id="45219-134">Response</span></span>

<span data-ttu-id="45219-135">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[onenoteSection](../resources/section.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="45219-135">If successful, this method returns a `200 OK` response code and a collection of [onenoteSection](../resources/section.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="45219-136">例</span><span class="sxs-lookup"><span data-stu-id="45219-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="45219-137">要求</span><span class="sxs-lookup"><span data-stu-id="45219-137">Request</span></span>
<span data-ttu-id="45219-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="45219-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sections"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}/sections
```
##### <a name="response"></a><span data-ttu-id="45219-139">応答</span><span class="sxs-lookup"><span data-stu-id="45219-139">Response</span></span>
<span data-ttu-id="45219-p104">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="45219-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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