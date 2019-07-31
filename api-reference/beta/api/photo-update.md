---
title: 写真を更新する
description: 写真オブジェクトのプロパティを更新します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: fccd85b7ef3acf72f2f79f639fc8fccacc5dedb8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992389"
---
# <a name="update-photo"></a><span data-ttu-id="1f0dd-103">写真を更新する</span><span class="sxs-lookup"><span data-stu-id="1f0dd-103">Update photo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f0dd-104">写真オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1f0dd-104">Update the properties of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1f0dd-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1f0dd-105">Permissions</span></span>
<span data-ttu-id="1f0dd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1f0dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f0dd-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1f0dd-108">Permission type</span></span>      | <span data-ttu-id="1f0dd-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1f0dd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f0dd-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1f0dd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1f0dd-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f0dd-111">Not supported.</span></span>    |
|<span data-ttu-id="1f0dd-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1f0dd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f0dd-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f0dd-113">Not supported.</span></span>    |
|<span data-ttu-id="1f0dd-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1f0dd-114">Application</span></span> | <span data-ttu-id="1f0dd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f0dd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f0dd-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1f0dd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/photo
PATCH /groups/{id}/photo
PATCH /drive/root/createdByUser/photo
```

## <a name="request-headers"></a><span data-ttu-id="1f0dd-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1f0dd-117">Request headers</span></span>
| <span data-ttu-id="1f0dd-118">名前</span><span class="sxs-lookup"><span data-stu-id="1f0dd-118">Name</span></span>       | <span data-ttu-id="1f0dd-119">型</span><span class="sxs-lookup"><span data-stu-id="1f0dd-119">Type</span></span> | <span data-ttu-id="1f0dd-120">説明</span><span class="sxs-lookup"><span data-stu-id="1f0dd-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1f0dd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f0dd-121">Authorization</span></span>  | <span data-ttu-id="1f0dd-122">string</span><span class="sxs-lookup"><span data-stu-id="1f0dd-122">string</span></span>  | <span data-ttu-id="1f0dd-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1f0dd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f0dd-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1f0dd-125">Request body</span></span>
<span data-ttu-id="1f0dd-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="1f0dd-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1f0dd-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f0dd-129">Property</span></span>     | <span data-ttu-id="1f0dd-130">型</span><span class="sxs-lookup"><span data-stu-id="1f0dd-130">Type</span></span>   |<span data-ttu-id="1f0dd-131">説明</span><span class="sxs-lookup"><span data-stu-id="1f0dd-131">Description</span></span>|
|:---------------|:--------|:----------|

## <a name="response"></a><span data-ttu-id="1f0dd-132">応答</span><span class="sxs-lookup"><span data-stu-id="1f0dd-132">Response</span></span>

<span data-ttu-id="1f0dd-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された[写真](../resources/photo.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1f0dd-133">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1f0dd-134">例</span><span class="sxs-lookup"><span data-stu-id="1f0dd-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1f0dd-135">要求</span><span class="sxs-lookup"><span data-stu-id="1f0dd-135">Request</span></span>
<span data-ttu-id="1f0dd-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1f0dd-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1f0dd-137">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1f0dd-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_photo"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1f0dd-138">C#</span><span class="sxs-lookup"><span data-stu-id="1f0dd-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-photo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1f0dd-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="1f0dd-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-photo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1f0dd-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="1f0dd-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-photo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1f0dd-141">Java</span><span class="sxs-lookup"><span data-stu-id="1f0dd-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-photo-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1f0dd-142">応答</span><span class="sxs-lookup"><span data-stu-id="1f0dd-142">Response</span></span>
<span data-ttu-id="1f0dd-143">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="1f0dd-143">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
