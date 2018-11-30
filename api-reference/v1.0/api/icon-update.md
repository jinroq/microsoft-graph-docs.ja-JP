---
title: アイコンを更新する
description: アイコン オブジェクトのプロパティを更新します。
ms.openlocfilehash: 0cb3b1af0369c86290c842232acc57792d1552ce
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023750"
---
# <a name="update-icon"></a><span data-ttu-id="e947d-103">アイコンを更新する</span><span class="sxs-lookup"><span data-stu-id="e947d-103">Update icon</span></span>

<span data-ttu-id="e947d-104">アイコン オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e947d-104">Update the properties of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e947d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e947d-105">Permissions</span></span>
<span data-ttu-id="e947d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e947d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e947d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e947d-108">Permission type</span></span>      | <span data-ttu-id="e947d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e947d-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="e947d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e947d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e947d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e947d-111">Files.ReadWrite</span></span>    | 
|<span data-ttu-id="e947d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e947d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e947d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e947d-113">Not supported.</span></span>    | 
|<span data-ttu-id="e947d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e947d-114">Application</span></span> | <span data-ttu-id="e947d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e947d-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e947d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e947d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/sort/fields/icon
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-request-headers"></a><span data-ttu-id="e947d-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e947d-117">Optional request headers</span></span>
| <span data-ttu-id="e947d-118">名前</span><span class="sxs-lookup"><span data-stu-id="e947d-118">Name</span></span>       | <span data-ttu-id="e947d-119">説明</span><span class="sxs-lookup"><span data-stu-id="e947d-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e947d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e947d-120">Authorization</span></span>  | <span data-ttu-id="e947d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e947d-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="e947d-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="e947d-123">Request body</span></span>
<span data-ttu-id="e947d-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="e947d-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e947d-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e947d-127">Property</span></span>     | <span data-ttu-id="e947d-128">型</span><span class="sxs-lookup"><span data-stu-id="e947d-128">Type</span></span>   |<span data-ttu-id="e947d-129">説明</span><span class="sxs-lookup"><span data-stu-id="e947d-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e947d-130">index</span><span class="sxs-lookup"><span data-stu-id="e947d-130">index</span></span>|<span data-ttu-id="e947d-131">int</span><span class="sxs-lookup"><span data-stu-id="e947d-131">int</span></span>|<span data-ttu-id="e947d-132">指定したセット内のアイコンのインデックスを表します。</span><span class="sxs-lookup"><span data-stu-id="e947d-132">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="e947d-133">set</span><span class="sxs-lookup"><span data-stu-id="e947d-133">set</span></span>|<span data-ttu-id="e947d-134">文字列</span><span class="sxs-lookup"><span data-stu-id="e947d-134">string</span></span>|<span data-ttu-id="e947d-135">一部であるアイコンのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="e947d-135">Represents the set that the icon is part of.</span></span> <span data-ttu-id="e947d-136">可能な値: `Invalid`、 `ThreeArrows`、 `ThreeArrowsGray`、 `ThreeFlags`、 `ThreeTrafficLights1`、 `ThreeTrafficLights2`、 `ThreeSigns`、 `ThreeSymbols`、 `ThreeSymbols2`、 `FourArrows`、 `FourArrowsGray`、 `FourRedToBlack`、 `FourRating`、 `FourTrafficLights`、 `FiveArrows`、 `FiveArrowsGray`、 `FiveRating`、 `FiveQuarters`、 `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span><span class="sxs-lookup"><span data-stu-id="e947d-136">The possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="response"></a><span data-ttu-id="e947d-137">応答</span><span class="sxs-lookup"><span data-stu-id="e947d-137">Response</span></span>

<span data-ttu-id="e947d-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された[アイコン](../resources/icon.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e947d-138">If successful, this method returns a `200 OK` response code and updated [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e947d-139">例</span><span class="sxs-lookup"><span data-stu-id="e947d-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e947d-140">要求</span><span class="sxs-lookup"><span data-stu-id="e947d-140">Request</span></span>
<span data-ttu-id="e947d-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e947d-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_icon"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```
##### <a name="response"></a><span data-ttu-id="e947d-142">応答</span><span class="sxs-lookup"><span data-stu-id="e947d-142">Response</span></span>
<span data-ttu-id="e947d-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e947d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookIcon"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update icon",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->