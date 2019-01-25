---
title: ノートブックを一覧表示する
description: ノートブック オブジェクトの一覧を取得します。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 49274d1ed7ab74ee5a4322bf9e13d849052f1c35
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511129"
---
# <a name="list-notebooks"></a><span data-ttu-id="0797d-103">ノートブックを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="0797d-103">List notebooks</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0797d-104">[ノートブック](../resources/notebook.md) オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="0797d-104">Retrieve a list of [notebook](../resources/notebook.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="0797d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0797d-105">Permissions</span></span>
<span data-ttu-id="0797d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0797d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0797d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0797d-108">Permission type</span></span>      | <span data-ttu-id="0797d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0797d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0797d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0797d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0797d-111">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0797d-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="0797d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0797d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0797d-113">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0797d-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="0797d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0797d-114">Application</span></span> | <span data-ttu-id="0797d-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0797d-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0797d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0797d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks
GET /users/{id | userPrincipalName}/onenote/notebooks
GET /groups/{id}/onenote/notebooks
GET /sites/{id}/onenote/notebooks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0797d-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0797d-117">Optional query parameters</span></span>
<span data-ttu-id="0797d-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0797d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="0797d-119">既定の並べ替え順序は `name asc` です。</span><span class="sxs-lookup"><span data-stu-id="0797d-119">The default sort order is `name asc`.</span></span> 

<span data-ttu-id="0797d-120">ノートブックの有効な `expand` 値は `sections` および `sectionGroups` です。</span><span class="sxs-lookup"><span data-stu-id="0797d-120">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0797d-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0797d-121">Request headers</span></span>
| <span data-ttu-id="0797d-122">名前</span><span class="sxs-lookup"><span data-stu-id="0797d-122">Name</span></span>       | <span data-ttu-id="0797d-123">型</span><span class="sxs-lookup"><span data-stu-id="0797d-123">Type</span></span> | <span data-ttu-id="0797d-124">説明</span><span class="sxs-lookup"><span data-stu-id="0797d-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0797d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0797d-125">Authorization</span></span>  | <span data-ttu-id="0797d-126">string</span><span class="sxs-lookup"><span data-stu-id="0797d-126">string</span></span>  | <span data-ttu-id="0797d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0797d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0797d-129">承諾</span><span class="sxs-lookup"><span data-stu-id="0797d-129">Accept</span></span> | <span data-ttu-id="0797d-130">string</span><span class="sxs-lookup"><span data-stu-id="0797d-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="0797d-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="0797d-131">Request body</span></span>
<span data-ttu-id="0797d-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0797d-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0797d-133">応答</span><span class="sxs-lookup"><span data-stu-id="0797d-133">Response</span></span>

<span data-ttu-id="0797d-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [notebook](../resources/notebook.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="0797d-134">If successful, this method returns a `200 OK` response code and collection of [notebook](../resources/notebook.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0797d-135">例</span><span class="sxs-lookup"><span data-stu-id="0797d-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0797d-136">要求</span><span class="sxs-lookup"><span data-stu-id="0797d-136">Request</span></span>
<span data-ttu-id="0797d-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0797d-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebooks"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/notebooks
```
##### <a name="response"></a><span data-ttu-id="0797d-138">応答</span><span class="sxs-lookup"><span data-stu-id="0797d-138">Response</span></span>
<span data-ttu-id="0797d-p103">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0797d-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 369

{
  "value": [
    {
      "isDefault": true,
      "userRole": {
      },
      "isShared": true,
      "sectionsUrl": "sectionsUrl-value",
      "sectionGroupsUrl": "sectionGroupsUrl-value",
      "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
      "links": {
        "oneNoteClientUrl": {
          "href": "href-value"
        },
        "oneNoteWebUrl": {
          "href": "href-value"
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
  "description": "List notebooks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/onenote-list-notebooks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
