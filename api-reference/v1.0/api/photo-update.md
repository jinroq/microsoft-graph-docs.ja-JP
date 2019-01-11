---
title: 写真を更新する
description: 写真オブジェクトのプロパティを更新します。
localization_priority: Normal
ms.openlocfilehash: 80c866eab74307d3001887110e050aa438cdde9f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883784"
---
# <a name="update-photo"></a><span data-ttu-id="c7c72-103">写真を更新する</span><span class="sxs-lookup"><span data-stu-id="c7c72-103">Update photo</span></span>

<span data-ttu-id="c7c72-104">写真オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c7c72-104">Update the properties of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c7c72-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c7c72-105">Permissions</span></span>
<span data-ttu-id="c7c72-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c7c72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7c72-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c7c72-108">Permission type</span></span>      | <span data-ttu-id="c7c72-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c7c72-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7c72-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c7c72-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c7c72-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7c72-111">Not supported.</span></span>    |
|<span data-ttu-id="c7c72-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c7c72-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7c72-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7c72-113">Not supported.</span></span>    |
|<span data-ttu-id="c7c72-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c7c72-114">Application</span></span> | <span data-ttu-id="c7c72-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7c72-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7c72-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c7c72-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/photo
PATCH /groups/{id}/photo
PATCH /drive/root/createdByUser/photo
```

## <a name="request-headers"></a><span data-ttu-id="c7c72-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c7c72-117">Request headers</span></span>
| <span data-ttu-id="c7c72-118">名前</span><span class="sxs-lookup"><span data-stu-id="c7c72-118">Name</span></span>       | <span data-ttu-id="c7c72-119">種類</span><span class="sxs-lookup"><span data-stu-id="c7c72-119">Type</span></span> | <span data-ttu-id="c7c72-120">説明</span><span class="sxs-lookup"><span data-stu-id="c7c72-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c7c72-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7c72-121">Authorization</span></span>  | <span data-ttu-id="c7c72-122">string</span><span class="sxs-lookup"><span data-stu-id="c7c72-122">string</span></span>  | <span data-ttu-id="c7c72-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c7c72-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7c72-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c7c72-125">Request body</span></span>
<span data-ttu-id="c7c72-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="c7c72-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c7c72-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7c72-129">Property</span></span>     | <span data-ttu-id="c7c72-130">種類</span><span class="sxs-lookup"><span data-stu-id="c7c72-130">Type</span></span>   |<span data-ttu-id="c7c72-131">説明</span><span class="sxs-lookup"><span data-stu-id="c7c72-131">Description</span></span>|
|:---------------|:--------|:----------|

## <a name="response"></a><span data-ttu-id="c7c72-132">応答</span><span class="sxs-lookup"><span data-stu-id="c7c72-132">Response</span></span>

<span data-ttu-id="c7c72-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された[写真](../resources/photo.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c7c72-133">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c7c72-134">例</span><span class="sxs-lookup"><span data-stu-id="c7c72-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c7c72-135">要求</span><span class="sxs-lookup"><span data-stu-id="c7c72-135">Request</span></span>
<span data-ttu-id="c7c72-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c7c72-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_photo"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```
##### <a name="response"></a><span data-ttu-id="c7c72-137">応答</span><span class="sxs-lookup"><span data-stu-id="c7c72-137">Response</span></span>
<span data-ttu-id="c7c72-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c7c72-138">Here is an example of the response.</span></span>
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
