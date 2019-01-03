---
title: Outlook カテゴリを更新する
description: '指定した outlookCategory オブジェクトの書き込み可能な **color** プロパティを更新します。 **DisplayName**プロパティを変更することはできません。 '
ms.openlocfilehash: 1b664ef4414a798fe3f8ee2cd517a75f96ff3dc6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024043"
---
# <a name="update-outlook-category"></a><span data-ttu-id="6e39e-104">Outlook カテゴリを更新する</span><span class="sxs-lookup"><span data-stu-id="6e39e-104">Update Outlook category</span></span>


<span data-ttu-id="6e39e-105">指定した [outlookCategory](../resources/outlookcategory.md) オブジェクトの書き込み可能な **color** プロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6e39e-105">Update the writable property, **color**, of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span> <span data-ttu-id="6e39e-106">**displayName** をプロパティは、カテゴリの作成後に変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="6e39e-106">You cannot modify the **displayName** property once you have created the category.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e39e-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6e39e-107">Permissions</span></span>
<span data-ttu-id="6e39e-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6e39e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e39e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6e39e-110">Permission type</span></span>      | <span data-ttu-id="6e39e-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6e39e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e39e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6e39e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6e39e-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e39e-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="6e39e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6e39e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e39e-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e39e-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="6e39e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6e39e-116">Application</span></span> | <span data-ttu-id="6e39e-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e39e-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e39e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6e39e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/masterCategories/{id}
PATCH /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6e39e-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6e39e-119">Optional query parameters</span></span>
<span data-ttu-id="6e39e-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6e39e-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e39e-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6e39e-121">Request headers</span></span>
| <span data-ttu-id="6e39e-122">名前</span><span class="sxs-lookup"><span data-stu-id="6e39e-122">Name</span></span>      |<span data-ttu-id="6e39e-123">説明</span><span class="sxs-lookup"><span data-stu-id="6e39e-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6e39e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e39e-124">Authorization</span></span>  | <span data-ttu-id="6e39e-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6e39e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e39e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="6e39e-127">Request body</span></span>
<span data-ttu-id="6e39e-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="6e39e-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6e39e-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6e39e-131">Property</span></span>     | <span data-ttu-id="6e39e-132">型</span><span class="sxs-lookup"><span data-stu-id="6e39e-132">Type</span></span>   |<span data-ttu-id="6e39e-133">説明</span><span class="sxs-lookup"><span data-stu-id="6e39e-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e39e-134">color</span><span class="sxs-lookup"><span data-stu-id="6e39e-134">color</span></span>|<span data-ttu-id="6e39e-135">String</span><span class="sxs-lookup"><span data-stu-id="6e39e-135">String</span></span>|<span data-ttu-id="6e39e-136">カテゴリを特徴付ける、あらかじめ設定された色の定数。定数は、事前定義された 25 種類の色のいずれか 1 つにマッピングされています。</span><span class="sxs-lookup"><span data-stu-id="6e39e-136">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> |

## <a name="response"></a><span data-ttu-id="6e39e-137">応答</span><span class="sxs-lookup"><span data-stu-id="6e39e-137">Response</span></span>

<span data-ttu-id="6e39e-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文に更新後の [outlookCategory](../resources/outlookcategory.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6e39e-138">If successful, this method returns a `200 OK` response code and updated [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6e39e-139">例</span><span class="sxs-lookup"><span data-stu-id="6e39e-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6e39e-140">要求</span><span class="sxs-lookup"><span data-stu-id="6e39e-140">Request</span></span>
<span data-ttu-id="6e39e-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6e39e-141">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="6e39e-142">応答</span><span class="sxs-lookup"><span data-stu-id="6e39e-142">Response</span></span>
<span data-ttu-id="6e39e-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6e39e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->