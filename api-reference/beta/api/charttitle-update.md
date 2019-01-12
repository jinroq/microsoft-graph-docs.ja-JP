---
title: charttitle オブジェクトを更新する
description: charttitle オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4d0beb65acb208d6f04d495a98b3c48a046b29ba
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980805"
---
# <a name="update-charttitle"></a><span data-ttu-id="30809-103">charttitle オブジェクトを更新する</span><span class="sxs-lookup"><span data-stu-id="30809-103">Update charttitle</span></span>

> <span data-ttu-id="30809-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="30809-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="30809-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="30809-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="30809-106">charttitle オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="30809-106">Update the properties of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="30809-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="30809-107">Permissions</span></span>
<span data-ttu-id="30809-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="30809-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30809-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="30809-110">Permission type</span></span>      | <span data-ttu-id="30809-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="30809-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30809-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="30809-112">Delegated (work or school account)</span></span> | <span data-ttu-id="30809-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30809-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="30809-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="30809-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30809-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30809-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="30809-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="30809-116">Application</span></span> | <span data-ttu-id="30809-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="30809-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="30809-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="30809-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="30809-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="30809-119">Optional request headers</span></span>
| <span data-ttu-id="30809-120">名前</span><span class="sxs-lookup"><span data-stu-id="30809-120">Name</span></span>       | <span data-ttu-id="30809-121">説明</span><span class="sxs-lookup"><span data-stu-id="30809-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="30809-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="30809-122">Authorization</span></span>  | <span data-ttu-id="30809-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="30809-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="30809-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="30809-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="30809-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="30809-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="30809-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="30809-128">Request body</span></span>
<span data-ttu-id="30809-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="30809-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="30809-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="30809-132">Property</span></span>     | <span data-ttu-id="30809-133">型</span><span class="sxs-lookup"><span data-stu-id="30809-133">Type</span></span>   |<span data-ttu-id="30809-134">説明</span><span class="sxs-lookup"><span data-stu-id="30809-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30809-135">overlay</span><span class="sxs-lookup"><span data-stu-id="30809-135">overlay</span></span>|<span data-ttu-id="30809-136">ブール値</span><span class="sxs-lookup"><span data-stu-id="30809-136">boolean</span></span>|<span data-ttu-id="30809-137">グラフのタイトルをグラフに重ねるかどうかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="30809-137">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="30809-138">text</span><span class="sxs-lookup"><span data-stu-id="30809-138">text</span></span>|<span data-ttu-id="30809-139">文字列</span><span class="sxs-lookup"><span data-stu-id="30809-139">string</span></span>|<span data-ttu-id="30809-140">グラフのタイトルのテキストを表します。</span><span class="sxs-lookup"><span data-stu-id="30809-140">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="30809-141">visible</span><span class="sxs-lookup"><span data-stu-id="30809-141">visible</span></span>|<span data-ttu-id="30809-142">ブール値</span><span class="sxs-lookup"><span data-stu-id="30809-142">boolean</span></span>|<span data-ttu-id="30809-143">ChartTitle オブジェクトを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="30809-143">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="response"></a><span data-ttu-id="30809-144">応答</span><span class="sxs-lookup"><span data-stu-id="30809-144">Response</span></span>

<span data-ttu-id="30809-145">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [ChartTitle](../resources/charttitle.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="30809-145">If successful, this method returns a `200 OK` response code and updated [ChartTitle](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="30809-146">例</span><span class="sxs-lookup"><span data-stu-id="30809-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="30809-147">要求</span><span class="sxs-lookup"><span data-stu-id="30809-147">Request</span></span>
<span data-ttu-id="30809-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="30809-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_charttitle"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/title
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="30809-149">応答</span><span class="sxs-lookup"><span data-stu-id="30809-149">Response</span></span>
<span data-ttu-id="30809-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="30809-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update charttitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
