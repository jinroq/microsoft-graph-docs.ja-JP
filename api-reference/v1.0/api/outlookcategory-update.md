---
title: Outlook カテゴリを更新する
description: '指定した outlookCategory オブジェクトの書き込み可能な **color** プロパティを更新します。 **DisplayName**プロパティを変更することはできません '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a39c0d8aed73f40848e388872a62c4d459181247
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36309443"
---
# <a name="update-outlook-category"></a><span data-ttu-id="bea94-104">Outlook カテゴリを更新する</span><span class="sxs-lookup"><span data-stu-id="bea94-104">Update Outlook category</span></span>


<span data-ttu-id="bea94-105">指定した [outlookCategory](../resources/outlookcategory.md) オブジェクトの書き込み可能な **color** プロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bea94-105">Update the writable property, **color**, of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span> <span data-ttu-id="bea94-106">**displayName** をプロパティは、カテゴリの作成後に変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="bea94-106">You cannot modify the **displayName** property once you have created the category.</span></span>

## <a name="permissions"></a><span data-ttu-id="bea94-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bea94-107">Permissions</span></span>
<span data-ttu-id="bea94-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bea94-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bea94-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bea94-110">Permission type</span></span>      | <span data-ttu-id="bea94-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bea94-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bea94-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bea94-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bea94-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bea94-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="bea94-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bea94-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bea94-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bea94-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="bea94-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bea94-116">Application</span></span> | <span data-ttu-id="bea94-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bea94-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bea94-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bea94-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/masterCategories/{id}
PATCH /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bea94-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bea94-119">Request headers</span></span>
| <span data-ttu-id="bea94-120">名前</span><span class="sxs-lookup"><span data-stu-id="bea94-120">Name</span></span>      |<span data-ttu-id="bea94-121">説明</span><span class="sxs-lookup"><span data-stu-id="bea94-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bea94-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bea94-122">Authorization</span></span>  | <span data-ttu-id="bea94-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bea94-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bea94-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="bea94-125">Request body</span></span>
<span data-ttu-id="bea94-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="bea94-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bea94-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bea94-129">Property</span></span>     | <span data-ttu-id="bea94-130">型</span><span class="sxs-lookup"><span data-stu-id="bea94-130">Type</span></span>   |<span data-ttu-id="bea94-131">説明</span><span class="sxs-lookup"><span data-stu-id="bea94-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bea94-132">color</span><span class="sxs-lookup"><span data-stu-id="bea94-132">color</span></span>|<span data-ttu-id="bea94-133">String</span><span class="sxs-lookup"><span data-stu-id="bea94-133">String</span></span>|<span data-ttu-id="bea94-134">カテゴリを特徴付ける、あらかじめ設定された色の定数。定数は、事前定義された 25 種類の色のいずれか 1 つにマッピングされています。</span><span class="sxs-lookup"><span data-stu-id="bea94-134">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> |

## <a name="response"></a><span data-ttu-id="bea94-135">応答</span><span class="sxs-lookup"><span data-stu-id="bea94-135">Response</span></span>

<span data-ttu-id="bea94-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文に更新後の [outlookCategory](../resources/outlookcategory.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bea94-136">If successful, this method returns a `200 OK` response code and updated [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bea94-137">例</span><span class="sxs-lookup"><span data-stu-id="bea94-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bea94-138">要求</span><span class="sxs-lookup"><span data-stu-id="bea94-138">Request</span></span>
<span data-ttu-id="bea94-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bea94-139">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bea94-140">プロトコル</span><span class="sxs-lookup"><span data-stu-id="bea94-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["bac262b7-485d-4739-b436-e31467d64fac"],
  "name": "update_outlookcategory"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/outlook/masterCategories/bac262b7-485d-4739-b436-e31467d64fac
Content-type: application/json
Content-length: 30

{
  "color":"preset15"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bea94-141">C#</span><span class="sxs-lookup"><span data-stu-id="bea94-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-outlookcategory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bea94-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bea94-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-outlookcategory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bea94-143">目的-C</span><span class="sxs-lookup"><span data-stu-id="bea94-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-outlookcategory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bea94-144">Java</span><span class="sxs-lookup"><span data-stu-id="bea94-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-outlookcategory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bea94-145">応答</span><span class="sxs-lookup"><span data-stu-id="bea94-145">Response</span></span>
<span data-ttu-id="bea94-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bea94-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"bac262b7-485d-4739-b436-e31467d64fac",
  "displayName":"Project expenses",
  "color":"preset15"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
