---
title: セクションを作成する
description: 指定したノートブックに新しい onenoteSection を作成します。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 9985c4fc58ed639d2985c76591dc2bedf6eddabf
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892681"
---
# <a name="create-section"></a><span data-ttu-id="69592-103">セクションを作成する</span><span class="sxs-lookup"><span data-stu-id="69592-103">Create section</span></span>

<span data-ttu-id="69592-104">指定したノートブックに新しい[onenoteSection](../resources/section.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="69592-104">Create a new [onenoteSection](../resources/section.md) in the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="69592-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="69592-105">Permissions</span></span>
<span data-ttu-id="69592-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="69592-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69592-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="69592-108">Permission type</span></span>      | <span data-ttu-id="69592-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="69592-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69592-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="69592-110">Delegated (work or school account)</span></span> | <span data-ttu-id="69592-111">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69592-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="69592-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="69592-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69592-113">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69592-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="69592-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="69592-114">Application</span></span> | <span data-ttu-id="69592-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69592-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="69592-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="69592-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/sections
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/sections
POST /groups/{id}/onenote/notebooks/{id}/sections
POST /sites/{id}/onenote/notebooks/{id}/sections
```
## <a name="request-headers"></a><span data-ttu-id="69592-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="69592-117">Request headers</span></span>
| <span data-ttu-id="69592-118">名前</span><span class="sxs-lookup"><span data-stu-id="69592-118">Name</span></span>       | <span data-ttu-id="69592-119">型</span><span class="sxs-lookup"><span data-stu-id="69592-119">Type</span></span> | <span data-ttu-id="69592-120">説明</span><span class="sxs-lookup"><span data-stu-id="69592-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="69592-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="69592-121">Authorization</span></span>  | <span data-ttu-id="69592-122">string</span><span class="sxs-lookup"><span data-stu-id="69592-122">string</span></span>  | <span data-ttu-id="69592-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="69592-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="69592-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="69592-125">Content-Type</span></span> | <span data-ttu-id="69592-126">string</span><span class="sxs-lookup"><span data-stu-id="69592-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="69592-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="69592-127">Request body</span></span>
<span data-ttu-id="69592-128">要求本文でセクション名を入力します。</span><span class="sxs-lookup"><span data-stu-id="69592-128">In the request body, supply a name for the section.</span></span>

<span data-ttu-id="69592-p103">同じ階層レベルでは、セクションの名前を一意にする必要があります。名前は 50 文字以内で、次の文字は使用できません: ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="69592-p103">Within the same hierarchy level, section names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="69592-131">応答</span><span class="sxs-lookup"><span data-stu-id="69592-131">Response</span></span>

<span data-ttu-id="69592-132">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[onenoteSection](../resources/section.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="69592-132">If successful, this method returns a `201 Created` response code and a [onenoteSection](../resources/section.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69592-133">例</span><span class="sxs-lookup"><span data-stu-id="69592-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="69592-134">要求</span><span class="sxs-lookup"><span data-stu-id="69592-134">Request</span></span>
<span data-ttu-id="69592-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="69592-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="69592-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="69592-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_section_from_notebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sections
Content-type: application/json
Content-length: 27

{
  "displayName": "Section name"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="69592-137">C#</span><span class="sxs-lookup"><span data-stu-id="69592-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-section-from-notebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="69592-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="69592-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-section-from-notebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="69592-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="69592-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-section-from-notebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="69592-140">Java</span><span class="sxs-lookup"><span data-stu-id="69592-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-section-from-notebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="69592-141">応答</span><span class="sxs-lookup"><span data-stu-id="69592-141">Response</span></span>
<span data-ttu-id="69592-p104">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="69592-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 272

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Section",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
