---
title: 契約を更新する
description: アグリーメントオブジェクトのプロパティを更新します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: cb4c72f9646723bbef1d7544396864fb6a49f4f1
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408456"
---
# <a name="update-agreement"></a><span data-ttu-id="ce7db-103">契約を更新する</span><span class="sxs-lookup"><span data-stu-id="ce7db-103">Update agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce7db-104">[アグリーメント](../resources/agreement.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ce7db-104">Update the properties of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ce7db-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ce7db-105">Permissions</span></span>
<span data-ttu-id="ce7db-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce7db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce7db-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ce7db-108">Permission type</span></span>                        | <span data-ttu-id="ce7db-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ce7db-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce7db-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ce7db-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ce7db-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce7db-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="ce7db-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ce7db-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce7db-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce7db-113">Not supported.</span></span> |
|<span data-ttu-id="ce7db-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ce7db-114">Application</span></span>                            | <span data-ttu-id="ce7db-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce7db-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce7db-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ce7db-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /agreements/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ce7db-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce7db-117">Request headers</span></span>
| <span data-ttu-id="ce7db-118">名前</span><span class="sxs-lookup"><span data-stu-id="ce7db-118">Name</span></span>         | <span data-ttu-id="ce7db-119">型</span><span class="sxs-lookup"><span data-stu-id="ce7db-119">Type</span></span>        | <span data-ttu-id="ce7db-120">説明</span><span class="sxs-lookup"><span data-stu-id="ce7db-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ce7db-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce7db-121">Authorization</span></span> | <span data-ttu-id="ce7db-122">string</span><span class="sxs-lookup"><span data-stu-id="ce7db-122">string</span></span> | <span data-ttu-id="ce7db-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="ce7db-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce7db-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ce7db-125">Request body</span></span>
<span data-ttu-id="ce7db-126">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="ce7db-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ce7db-127">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="ce7db-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ce7db-128">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="ce7db-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ce7db-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce7db-129">Property</span></span>     | <span data-ttu-id="ce7db-130">型</span><span class="sxs-lookup"><span data-stu-id="ce7db-130">Type</span></span>        | <span data-ttu-id="ce7db-131">説明</span><span class="sxs-lookup"><span data-stu-id="ce7db-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ce7db-132">displayName</span><span class="sxs-lookup"><span data-stu-id="ce7db-132">displayName</span></span>|<span data-ttu-id="ce7db-133">String</span><span class="sxs-lookup"><span data-stu-id="ce7db-133">String</span></span>|<span data-ttu-id="ce7db-134">アグリーメントの表示名。</span><span class="sxs-lookup"><span data-stu-id="ce7db-134">Display name of the agreement.</span></span>|
|<span data-ttu-id="ce7db-135">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="ce7db-135">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="ce7db-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce7db-136">Boolean</span></span>|<span data-ttu-id="ce7db-137">ユーザーが同意する前に、契約を展開して表示する必要があるかどうか。</span><span class="sxs-lookup"><span data-stu-id="ce7db-137">Whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="response"></a><span data-ttu-id="ce7db-138">応答</span><span class="sxs-lookup"><span data-stu-id="ce7db-138">Response</span></span>
<span data-ttu-id="ce7db-139">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[アグリーメント](../resources/agreement.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ce7db-139">If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ce7db-140">例</span><span class="sxs-lookup"><span data-stu-id="ce7db-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ce7db-141">要求</span><span class="sxs-lookup"><span data-stu-id="ce7db-141">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ce7db-142">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ce7db-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_agreement"
}-->
```http
PATCH https://graph.microsoft.com/beta/agreements/{id}
Content-type: application/json
Content-length: 85

{
  "displayName": "displayName-value",
  "isViewingBeforeAcceptanceRequired": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ce7db-143">C#</span><span class="sxs-lookup"><span data-stu-id="ce7db-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ce7db-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce7db-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ce7db-145">目的-C</span><span class="sxs-lookup"><span data-stu-id="ce7db-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ce7db-146">応答</span><span class="sxs-lookup"><span data-stu-id="ce7db-146">Response</span></span>
><span data-ttu-id="ce7db-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ce7db-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 105

{
  "displayName": "displayName-value",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
