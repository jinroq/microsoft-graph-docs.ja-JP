---
title: Outlook カテゴリを更新する
description: '指定した outlookCategory オブジェクトの書き込み可能な **color** プロパティを更新します。 **DisplayName**プロパティを変更することはできません。 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: f6440708f7083e0b129e48aa0f455b892fd4d157
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965097"
---
# <a name="update-outlook-category"></a><span data-ttu-id="1d13e-104">Outlook カテゴリを更新する</span><span class="sxs-lookup"><span data-stu-id="1d13e-104">Update Outlook category</span></span>

> <span data-ttu-id="1d13e-105">**重要**: [Microsoft Graph で/beta のバージョンの Api を選択し、プレビューでは、変更されることができます。</span><span class="sxs-lookup"><span data-stu-id="1d13e-105">**Important**: APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d13e-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d13e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1d13e-107">指定した [outlookCategory](../resources/outlookcategory.md) オブジェクトの書き込み可能な **color** プロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1d13e-107">Update the writable property, **color**, of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span> <span data-ttu-id="1d13e-108">**displayName** をプロパティは、カテゴリの作成後に変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="1d13e-108">You cannot modify the **displayName** property once you have created the category.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d13e-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1d13e-109">Permissions</span></span>
<span data-ttu-id="1d13e-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1d13e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d13e-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1d13e-112">Permission type</span></span>      | <span data-ttu-id="1d13e-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1d13e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d13e-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1d13e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="1d13e-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d13e-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="1d13e-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1d13e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d13e-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d13e-117">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="1d13e-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1d13e-118">Application</span></span> | <span data-ttu-id="1d13e-119">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d13e-119">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d13e-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1d13e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/masterCategories/{id}
PATCH /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1d13e-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1d13e-121">Request headers</span></span>
| <span data-ttu-id="1d13e-122">名前</span><span class="sxs-lookup"><span data-stu-id="1d13e-122">Name</span></span>      |<span data-ttu-id="1d13e-123">説明</span><span class="sxs-lookup"><span data-stu-id="1d13e-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1d13e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d13e-124">Authorization</span></span>  | <span data-ttu-id="1d13e-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1d13e-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d13e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1d13e-127">Request body</span></span>
<span data-ttu-id="1d13e-p106">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="1d13e-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1d13e-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d13e-131">Property</span></span>     | <span data-ttu-id="1d13e-132">種類</span><span class="sxs-lookup"><span data-stu-id="1d13e-132">Type</span></span>   |<span data-ttu-id="1d13e-133">説明</span><span class="sxs-lookup"><span data-stu-id="1d13e-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d13e-134">color</span><span class="sxs-lookup"><span data-stu-id="1d13e-134">color</span></span>|<span data-ttu-id="1d13e-135">String</span><span class="sxs-lookup"><span data-stu-id="1d13e-135">String</span></span>|<span data-ttu-id="1d13e-136">カテゴリを特徴付ける、あらかじめ設定された色の定数。定数は、事前定義された 25 種類の色のいずれか 1 つにマッピングされています。</span><span class="sxs-lookup"><span data-stu-id="1d13e-136">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> |

## <a name="response"></a><span data-ttu-id="1d13e-137">応答</span><span class="sxs-lookup"><span data-stu-id="1d13e-137">Response</span></span>

<span data-ttu-id="1d13e-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文に更新後の [outlookCategory](../resources/outlookcategory.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1d13e-138">If successful, this method returns a `200 OK` response code and updated [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1d13e-139">例</span><span class="sxs-lookup"><span data-stu-id="1d13e-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1d13e-140">要求</span><span class="sxs-lookup"><span data-stu-id="1d13e-140">Request</span></span>
<span data-ttu-id="1d13e-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1d13e-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_outlookcategory"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/outlook/masterCategories('bac262b7-485d-4739-b436-e31467d64fac')
Content-type: application/json
Content-length: 30

{
  "color":"preset15"
}
```
##### <a name="response"></a><span data-ttu-id="1d13e-142">応答</span><span class="sxs-lookup"><span data-stu-id="1d13e-142">Response</span></span>
<span data-ttu-id="1d13e-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1d13e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
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
