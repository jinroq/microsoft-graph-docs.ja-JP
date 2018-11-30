---
title: 写真を更新する
description: 写真オブジェクトのプロパティを更新します。
ms.openlocfilehash: 8071c9e331f9af72c9a288239206f396d9ad3fcb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066754"
---
# <a name="update-photo"></a><span data-ttu-id="467c1-103">写真を更新する</span><span class="sxs-lookup"><span data-stu-id="467c1-103">Update photo</span></span>

> <span data-ttu-id="467c1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="467c1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="467c1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="467c1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="467c1-106">写真オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="467c1-106">Update the properties of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="467c1-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="467c1-107">Permissions</span></span>
<span data-ttu-id="467c1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="467c1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="467c1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="467c1-110">Permission type</span></span>      | <span data-ttu-id="467c1-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="467c1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="467c1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="467c1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="467c1-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="467c1-113">Not supported.</span></span>    |
|<span data-ttu-id="467c1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="467c1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="467c1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="467c1-115">Not supported.</span></span>    |
|<span data-ttu-id="467c1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="467c1-116">Application</span></span> | <span data-ttu-id="467c1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="467c1-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="467c1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="467c1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/photo
PATCH /groups/{id}/photo
PATCH /drive/root/createdByUser/photo
```

## <a name="request-headers"></a><span data-ttu-id="467c1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="467c1-119">Request headers</span></span>
| <span data-ttu-id="467c1-120">名前</span><span class="sxs-lookup"><span data-stu-id="467c1-120">Name</span></span>       | <span data-ttu-id="467c1-121">型</span><span class="sxs-lookup"><span data-stu-id="467c1-121">Type</span></span> | <span data-ttu-id="467c1-122">説明</span><span class="sxs-lookup"><span data-stu-id="467c1-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="467c1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="467c1-123">Authorization</span></span>  | <span data-ttu-id="467c1-124">string</span><span class="sxs-lookup"><span data-stu-id="467c1-124">string</span></span>  | <span data-ttu-id="467c1-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="467c1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="467c1-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="467c1-127">Request body</span></span>
<span data-ttu-id="467c1-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="467c1-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="467c1-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="467c1-131">Property</span></span>     | <span data-ttu-id="467c1-132">型</span><span class="sxs-lookup"><span data-stu-id="467c1-132">Type</span></span>   |<span data-ttu-id="467c1-133">説明</span><span class="sxs-lookup"><span data-stu-id="467c1-133">Description</span></span>|
|:---------------|:--------|:----------|

## <a name="response"></a><span data-ttu-id="467c1-134">応答</span><span class="sxs-lookup"><span data-stu-id="467c1-134">Response</span></span>

<span data-ttu-id="467c1-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された[写真](../resources/photo.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="467c1-135">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="467c1-136">例</span><span class="sxs-lookup"><span data-stu-id="467c1-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="467c1-137">要求</span><span class="sxs-lookup"><span data-stu-id="467c1-137">Request</span></span>
<span data-ttu-id="467c1-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="467c1-138">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="467c1-139">応答</span><span class="sxs-lookup"><span data-stu-id="467c1-139">Response</span></span>
<span data-ttu-id="467c1-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="467c1-140">Here is an example of the response.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
