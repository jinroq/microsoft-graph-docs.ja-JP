---
title: ノートブックを作成する
description: 新しい OneNote ノートブックを作成します。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 1fe0e9ac5c4ed1da62bf7419a0bd9e5fefa3a235
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878834"
---
# <a name="create-notebook"></a><span data-ttu-id="88e6f-103">ノートブックを作成する</span><span class="sxs-lookup"><span data-stu-id="88e6f-103">Create notebook</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88e6f-104">新しい OneNote[ノートブック](../resources/notebook.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="88e6f-104">Create a new OneNote [notebook](../resources/notebook.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="88e6f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="88e6f-105">Permissions</span></span>
<span data-ttu-id="88e6f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="88e6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88e6f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="88e6f-108">Permission type</span></span>      | <span data-ttu-id="88e6f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="88e6f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88e6f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="88e6f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="88e6f-111">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88e6f-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="88e6f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="88e6f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88e6f-113">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="88e6f-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="88e6f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="88e6f-114">Application</span></span> | <span data-ttu-id="88e6f-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88e6f-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="88e6f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="88e6f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks
POST /users/{id | userPrincipalName}/onenote/notebooks
POST /groups/{id}/onenote/notebooks
POST /sites/{id}/onenote/notebooks
```
## <a name="request-headers"></a><span data-ttu-id="88e6f-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="88e6f-117">Request headers</span></span>
| <span data-ttu-id="88e6f-118">名前</span><span class="sxs-lookup"><span data-stu-id="88e6f-118">Name</span></span>       | <span data-ttu-id="88e6f-119">型</span><span class="sxs-lookup"><span data-stu-id="88e6f-119">Type</span></span> | <span data-ttu-id="88e6f-120">説明</span><span class="sxs-lookup"><span data-stu-id="88e6f-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="88e6f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="88e6f-121">Authorization</span></span>  | <span data-ttu-id="88e6f-122">string</span><span class="sxs-lookup"><span data-stu-id="88e6f-122">string</span></span>  | <span data-ttu-id="88e6f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="88e6f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="88e6f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="88e6f-125">Content-Type</span></span> | <span data-ttu-id="88e6f-126">string</span><span class="sxs-lookup"><span data-stu-id="88e6f-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="88e6f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="88e6f-127">Request body</span></span>
<span data-ttu-id="88e6f-128">要求本文で、ノートブックの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="88e6f-128">In the request body, supply a name for the notebook.</span></span> 

<span data-ttu-id="88e6f-129">ノートブック名は一意である必要があります。</span><span class="sxs-lookup"><span data-stu-id="88e6f-129">Notebook names must be unique.</span></span> <span data-ttu-id="88e6f-130">名前に128文字を超える文字を含めることはできません。また\/、次の文字を含めることはできません:? \*: <>| ' "</span><span class="sxs-lookup"><span data-stu-id="88e6f-130">The name cannot contain more than 128 characters or contain the following characters:  ?\*\/:<>|'"</span></span>

## <a name="response"></a><span data-ttu-id="88e6f-131">応答</span><span class="sxs-lookup"><span data-stu-id="88e6f-131">Response</span></span>

<span data-ttu-id="88e6f-132">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で新しい[notebook](../resources/notebook.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="88e6f-132">If successful, this method returns a `201 Created` response code and the new [notebook](../resources/notebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88e6f-133">例</span><span class="sxs-lookup"><span data-stu-id="88e6f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="88e6f-134">要求</span><span class="sxs-lookup"><span data-stu-id="88e6f-134">Request</span></span>
<span data-ttu-id="88e6f-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="88e6f-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="88e6f-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="88e6f-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_notebook_from_onenote"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks
Content-type: application/json
Content-length: 30

{
  "displayName": "Notebook name"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="88e6f-137">C#</span><span class="sxs-lookup"><span data-stu-id="88e6f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-notebook-from-onenote-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="88e6f-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="88e6f-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-notebook-from-onenote-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="88e6f-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="88e6f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-notebook-from-onenote-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="88e6f-140">Java</span><span class="sxs-lookup"><span data-stu-id="88e6f-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-notebook-from-onenote-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="88e6f-141">応答</span><span class="sxs-lookup"><span data-stu-id="88e6f-141">Response</span></span>
<span data-ttu-id="88e6f-p104">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="88e6f-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 284

{
  "isDefault": true,
  "userRole": {
  },
  "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
  "isShared": true,
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
