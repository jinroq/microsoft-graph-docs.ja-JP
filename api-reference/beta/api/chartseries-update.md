---
title: Update chartseries
description: chartseries オブジェクトのプロパティを更新します。
author: lumine2008
ms.openlocfilehash: 69e6de2e6d332a63f4ea7b1cc23ca48032cbbaba
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358955"
---
# <a name="update-chartseries"></a><span data-ttu-id="503c3-103">Update chartseries</span><span class="sxs-lookup"><span data-stu-id="503c3-103">Update chartseries</span></span>

> <span data-ttu-id="503c3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="503c3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="503c3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="503c3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="503c3-106">chartseries オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="503c3-106">Update the properties of chartseries object.</span></span>
## <a name="permissions"></a><span data-ttu-id="503c3-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="503c3-107">Permissions</span></span>
<span data-ttu-id="503c3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="503c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="503c3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="503c3-110">Permission type</span></span>      | <span data-ttu-id="503c3-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="503c3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="503c3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="503c3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="503c3-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="503c3-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="503c3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="503c3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="503c3-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="503c3-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="503c3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="503c3-116">Application</span></span> | <span data-ttu-id="503c3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="503c3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="503c3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="503c3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="503c3-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="503c3-119">Optional request headers</span></span>
| <span data-ttu-id="503c3-120">名前</span><span class="sxs-lookup"><span data-stu-id="503c3-120">Name</span></span>       | <span data-ttu-id="503c3-121">説明</span><span class="sxs-lookup"><span data-stu-id="503c3-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="503c3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="503c3-122">Authorization</span></span>  | <span data-ttu-id="503c3-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="503c3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="503c3-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="503c3-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="503c3-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="503c3-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="503c3-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="503c3-128">Request body</span></span>
<span data-ttu-id="503c3-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="503c3-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="503c3-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="503c3-132">Property</span></span>     | <span data-ttu-id="503c3-133">種類</span><span class="sxs-lookup"><span data-stu-id="503c3-133">Type</span></span>   |<span data-ttu-id="503c3-134">説明</span><span class="sxs-lookup"><span data-stu-id="503c3-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="503c3-135">name</span><span class="sxs-lookup"><span data-stu-id="503c3-135">name</span></span>|<span data-ttu-id="503c3-136">文字列</span><span class="sxs-lookup"><span data-stu-id="503c3-136">string</span></span>|<span data-ttu-id="503c3-137">グラフのデータ系列の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="503c3-137">Represents the name of a series in a chart.</span></span>|

## <a name="response"></a><span data-ttu-id="503c3-138">応答</span><span class="sxs-lookup"><span data-stu-id="503c3-138">Response</span></span>

<span data-ttu-id="503c3-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [ChartSeries](../resources/chartseries.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="503c3-139">If successful, this method returns a `200 OK` response code and updated [ChartSeries](../resources/chartseries.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="503c3-140">例</span><span class="sxs-lookup"><span data-stu-id="503c3-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="503c3-141">要求</span><span class="sxs-lookup"><span data-stu-id="503c3-141">Request</span></span>
<span data-ttu-id="503c3-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="503c3-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartseries"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
##### <a name="response"></a><span data-ttu-id="503c3-143">応答</span><span class="sxs-lookup"><span data-stu-id="503c3-143">Response</span></span>
<span data-ttu-id="503c3-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="503c3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartSeries"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartseries",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->