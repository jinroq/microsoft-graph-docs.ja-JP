---
title: セクションを作成する
description: 指定したセクショングループに新しい onenoteSection を作成します。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: df2541bc27d4a5b2f1f55d0ffc15938365c62392
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272773"
---
# <a name="create-section"></a><span data-ttu-id="a9c54-103">セクションを作成する</span><span class="sxs-lookup"><span data-stu-id="a9c54-103">Create section</span></span>

<span data-ttu-id="a9c54-104">指定したセクショングループに新しい[onenoteSection](../resources/section.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="a9c54-104">Create a new [onenoteSection](../resources/section.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="a9c54-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a9c54-105">Permissions</span></span>
<span data-ttu-id="a9c54-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a9c54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9c54-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a9c54-108">Permission type</span></span>      | <span data-ttu-id="a9c54-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a9c54-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9c54-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a9c54-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a9c54-111">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9c54-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="a9c54-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a9c54-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9c54-113">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9c54-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="a9c54-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a9c54-114">Application</span></span> | <span data-ttu-id="a9c54-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9c54-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9c54-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a9c54-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sections
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sections
POST /groups/{id}/onenote/sectionGroups/{id}/sections
POST /sites/{id}/onenote/sectionGroups/{id}/sections
```
## <a name="request-headers"></a><span data-ttu-id="a9c54-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a9c54-117">Request headers</span></span>
| <span data-ttu-id="a9c54-118">名前</span><span class="sxs-lookup"><span data-stu-id="a9c54-118">Name</span></span>       | <span data-ttu-id="a9c54-119">型</span><span class="sxs-lookup"><span data-stu-id="a9c54-119">Type</span></span> | <span data-ttu-id="a9c54-120">説明</span><span class="sxs-lookup"><span data-stu-id="a9c54-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a9c54-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9c54-121">Authorization</span></span>  | <span data-ttu-id="a9c54-122">string</span><span class="sxs-lookup"><span data-stu-id="a9c54-122">string</span></span>  | <span data-ttu-id="a9c54-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a9c54-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a9c54-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a9c54-125">Content-Type</span></span> | <span data-ttu-id="a9c54-126">string</span><span class="sxs-lookup"><span data-stu-id="a9c54-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="a9c54-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a9c54-127">Request body</span></span>
<span data-ttu-id="a9c54-128">要求本文でセクション名を入力します。</span><span class="sxs-lookup"><span data-stu-id="a9c54-128">In the request body, supply a name for the section.</span></span>

<span data-ttu-id="a9c54-p103">同じ階層レベルでは、セクションの名前を一意にする必要があります。名前は 50 文字以内で、次の文字は使用できません: ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="a9c54-p103">Within the same hierarchy level, section names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="a9c54-131">応答</span><span class="sxs-lookup"><span data-stu-id="a9c54-131">Response</span></span>

<span data-ttu-id="a9c54-132">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[onenoteSection](../resources/section.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a9c54-132">If successful, this method returns a `201 Created` response code and a [onenoteSection](../resources/section.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9c54-133">例</span><span class="sxs-lookup"><span data-stu-id="a9c54-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a9c54-134">要求</span><span class="sxs-lookup"><span data-stu-id="a9c54-134">Request</span></span>
<span data-ttu-id="a9c54-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a9c54-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_section_from_sectiongroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}/sections
Content-type: application/json
Content-length: 27

{
  "displayName": "Section name"
}
```

##### <a name="response"></a><span data-ttu-id="a9c54-136">応答</span><span class="sxs-lookup"><span data-stu-id="a9c54-136">Response</span></span>
<span data-ttu-id="a9c54-p104">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a9c54-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 200 OK
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a9c54-140">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="a9c54-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a9c54-141">C#</span><span class="sxs-lookup"><span data-stu-id="a9c54-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_section_from_sectiongroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a9c54-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="a9c54-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_section_from_sectiongroup-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a9c54-143">目的-C</span><span class="sxs-lookup"><span data-stu-id="a9c54-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_section_from_sectiongroup-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Section",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/sectiongroup-post-sections.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/sectiongroup-post-sections.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/sectiongroup-post-sections.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
