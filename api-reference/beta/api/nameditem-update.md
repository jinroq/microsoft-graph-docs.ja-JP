---
title: NamedItem オブジェクトを更新する
description: nameditem オブジェクトのプロパティを更新します。
localization_priority: Normal
ms.openlocfilehash: b7ef5b2086668b525cf527baab5a882f9c11e6ca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883749"
---
# <a name="update-nameditem"></a><span data-ttu-id="ec492-103">NamedItem オブジェクトを更新する</span><span class="sxs-lookup"><span data-stu-id="ec492-103">Update nameditem</span></span>

> <span data-ttu-id="ec492-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ec492-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec492-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ec492-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ec492-106">nameditem オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ec492-106">Update the properties of nameditem object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ec492-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ec492-107">Permissions</span></span>
<span data-ttu-id="ec492-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ec492-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec492-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ec492-110">Permission type</span></span>      | <span data-ttu-id="ec492-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ec492-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec492-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ec492-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ec492-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec492-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ec492-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ec492-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec492-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec492-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ec492-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ec492-116">Application</span></span> | <span data-ttu-id="ec492-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ec492-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec492-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ec492-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="ec492-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ec492-119">Optional request headers</span></span>
| <span data-ttu-id="ec492-120">名前</span><span class="sxs-lookup"><span data-stu-id="ec492-120">Name</span></span>       | <span data-ttu-id="ec492-121">説明</span><span class="sxs-lookup"><span data-stu-id="ec492-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ec492-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec492-122">Authorization</span></span>  | <span data-ttu-id="ec492-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ec492-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ec492-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ec492-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="ec492-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="ec492-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec492-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="ec492-128">Request body</span></span>
<span data-ttu-id="ec492-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="ec492-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ec492-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ec492-132">Property</span></span>     | <span data-ttu-id="ec492-133">種類</span><span class="sxs-lookup"><span data-stu-id="ec492-133">Type</span></span>   |<span data-ttu-id="ec492-134">説明</span><span class="sxs-lookup"><span data-stu-id="ec492-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ec492-135">visible</span><span class="sxs-lookup"><span data-stu-id="ec492-135">visible</span></span>|<span data-ttu-id="ec492-136">ブール値</span><span class="sxs-lookup"><span data-stu-id="ec492-136">boolean</span></span>|<span data-ttu-id="ec492-137">オブジェクトを表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ec492-137">Specifies whether the object is visible or not.</span></span>|
|<span data-ttu-id="ec492-138">comment</span><span class="sxs-lookup"><span data-stu-id="ec492-138">comment</span></span>|   <span data-ttu-id="ec492-139">文字列</span><span class="sxs-lookup"><span data-stu-id="ec492-139">string</span></span>  |<span data-ttu-id="ec492-140">この名前に関連付けられているコメントを表します。</span><span class="sxs-lookup"><span data-stu-id="ec492-140">Represents the comment associated with this name.</span></span>|

## <a name="response"></a><span data-ttu-id="ec492-141">応答</span><span class="sxs-lookup"><span data-stu-id="ec492-141">Response</span></span>

<span data-ttu-id="ec492-142">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [NamedItem](../resources/nameditem.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ec492-142">If successful, this method returns a `200 OK` response code and updated [NamedItem](../resources/nameditem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ec492-143">例</span><span class="sxs-lookup"><span data-stu-id="ec492-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec492-144">要求</span><span class="sxs-lookup"><span data-stu-id="ec492-144">Request</span></span>
<span data-ttu-id="ec492-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ec492-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_nameditem"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)
Content-type: application/json
Content-length: 87

{
  "type": "type-value",
  "scope": "scope-value",
  "comment": "comment-value",
  "value": {
  },
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="ec492-146">応答</span><span class="sxs-lookup"><span data-stu-id="ec492-146">Response</span></span>
<span data-ttu-id="ec492-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ec492-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 87

{
  "name": "name-value",
  "type": "type-value",
  "value": {
  },
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update nameditem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
