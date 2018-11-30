---
title: ChartAxis を更新する
description: chartaxis オブジェクトのプロパティを更新します。
ms.openlocfilehash: aebb499bd6aaa601fc63eb15c7cd7ab9fc3fe7ed
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069606"
---
# <a name="update-chartaxis"></a><span data-ttu-id="501e0-103">ChartAxis を更新する</span><span class="sxs-lookup"><span data-stu-id="501e0-103">Update chartaxis</span></span>

> <span data-ttu-id="501e0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="501e0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="501e0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="501e0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="501e0-106">chartaxis オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="501e0-106">Update the properties of chartaxis object.</span></span>
## <a name="permissions"></a><span data-ttu-id="501e0-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="501e0-107">Permissions</span></span>
<span data-ttu-id="501e0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="501e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="501e0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="501e0-110">Permission type</span></span>      | <span data-ttu-id="501e0-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="501e0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="501e0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="501e0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="501e0-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="501e0-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="501e0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="501e0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="501e0-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="501e0-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="501e0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="501e0-116">Application</span></span> | <span data-ttu-id="501e0-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="501e0-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="501e0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="501e0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis
```
## <a name="optional-request-headers"></a><span data-ttu-id="501e0-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="501e0-119">Optional request headers</span></span>
| <span data-ttu-id="501e0-120">名前</span><span class="sxs-lookup"><span data-stu-id="501e0-120">Name</span></span>       | <span data-ttu-id="501e0-121">説明</span><span class="sxs-lookup"><span data-stu-id="501e0-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="501e0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="501e0-122">Authorization</span></span>  | <span data-ttu-id="501e0-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="501e0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="501e0-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="501e0-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="501e0-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="501e0-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="501e0-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="501e0-128">Request body</span></span>
<span data-ttu-id="501e0-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="501e0-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="501e0-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="501e0-132">Property</span></span>     | <span data-ttu-id="501e0-133">型</span><span class="sxs-lookup"><span data-stu-id="501e0-133">Type</span></span>   |<span data-ttu-id="501e0-134">説明</span><span class="sxs-lookup"><span data-stu-id="501e0-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="501e0-135">majorUnit</span><span class="sxs-lookup"><span data-stu-id="501e0-135">majorUnit</span></span>|<span data-ttu-id="501e0-136">オブジェクト</span><span class="sxs-lookup"><span data-stu-id="501e0-136">object</span></span>|<span data-ttu-id="501e0-p106">2 つの大きい目盛の間隔を表します。数値の値または空の文字列を設定できます。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="501e0-p106">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="501e0-140">maximum</span><span class="sxs-lookup"><span data-stu-id="501e0-140">maximum</span></span>|<span data-ttu-id="501e0-141">object</span><span class="sxs-lookup"><span data-stu-id="501e0-141">object</span></span>|<span data-ttu-id="501e0-p107">数値軸の最大値を表します。数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="501e0-p107">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="501e0-145">minimum</span><span class="sxs-lookup"><span data-stu-id="501e0-145">minimum</span></span>|<span data-ttu-id="501e0-146">object</span><span class="sxs-lookup"><span data-stu-id="501e0-146">object</span></span>|<span data-ttu-id="501e0-p108">数値軸の最小値を表します。数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="501e0-p108">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="501e0-150">minorUnit</span><span class="sxs-lookup"><span data-stu-id="501e0-150">minorUnit</span></span>|<span data-ttu-id="501e0-151">オブジェクト</span><span class="sxs-lookup"><span data-stu-id="501e0-151">object</span></span>|<span data-ttu-id="501e0-p109">2 つの小さい目盛の間隔を表します。"数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="501e0-p109">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="response"></a><span data-ttu-id="501e0-155">応答</span><span class="sxs-lookup"><span data-stu-id="501e0-155">Response</span></span>

<span data-ttu-id="501e0-156">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [ChartAxis](../resources/chartaxis.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="501e0-156">If successful, this method returns a `200 OK` response code and updated [ChartAxis](../resources/chartaxis.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="501e0-157">例</span><span class="sxs-lookup"><span data-stu-id="501e0-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="501e0-158">要求</span><span class="sxs-lookup"><span data-stu-id="501e0-158">Request</span></span>
<span data-ttu-id="501e0-159">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="501e0-159">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartaxis"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```
##### <a name="response"></a><span data-ttu-id="501e0-160">応答</span><span class="sxs-lookup"><span data-stu-id="501e0-160">Response</span></span>
<span data-ttu-id="501e0-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="501e0-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartaxis"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartaxis",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->