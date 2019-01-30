---
title: charttitle オブジェクトを更新する
description: charttitle オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e67790672f2e31baaacd0eba500684f7b2275e97
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640379"
---
# <a name="update-charttitle"></a><span data-ttu-id="04663-103">charttitle オブジェクトを更新する</span><span class="sxs-lookup"><span data-stu-id="04663-103">Update charttitle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04663-104">charttitle オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="04663-104">Update the properties of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="04663-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="04663-105">Permissions</span></span>
<span data-ttu-id="04663-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04663-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04663-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="04663-108">Permission type</span></span>      | <span data-ttu-id="04663-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="04663-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04663-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="04663-110">Delegated (work or school account)</span></span> | <span data-ttu-id="04663-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04663-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="04663-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="04663-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04663-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04663-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="04663-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="04663-114">Application</span></span> | <span data-ttu-id="04663-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04663-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="04663-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="04663-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="04663-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04663-117">Optional request headers</span></span>
| <span data-ttu-id="04663-118">名前</span><span class="sxs-lookup"><span data-stu-id="04663-118">Name</span></span>       | <span data-ttu-id="04663-119">説明</span><span class="sxs-lookup"><span data-stu-id="04663-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="04663-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="04663-120">Authorization</span></span>  | <span data-ttu-id="04663-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="04663-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="04663-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="04663-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="04663-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="04663-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="04663-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="04663-126">Request body</span></span>
<span data-ttu-id="04663-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="04663-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="04663-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04663-130">Property</span></span>     | <span data-ttu-id="04663-131">型</span><span class="sxs-lookup"><span data-stu-id="04663-131">Type</span></span>   |<span data-ttu-id="04663-132">説明</span><span class="sxs-lookup"><span data-stu-id="04663-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04663-133">overlay</span><span class="sxs-lookup"><span data-stu-id="04663-133">overlay</span></span>|<span data-ttu-id="04663-134">ブール値</span><span class="sxs-lookup"><span data-stu-id="04663-134">boolean</span></span>|<span data-ttu-id="04663-135">グラフのタイトルをグラフに重ねるかどうかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="04663-135">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="04663-136">text</span><span class="sxs-lookup"><span data-stu-id="04663-136">text</span></span>|<span data-ttu-id="04663-137">文字列</span><span class="sxs-lookup"><span data-stu-id="04663-137">string</span></span>|<span data-ttu-id="04663-138">グラフのタイトルのテキストを表します。</span><span class="sxs-lookup"><span data-stu-id="04663-138">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="04663-139">visible</span><span class="sxs-lookup"><span data-stu-id="04663-139">visible</span></span>|<span data-ttu-id="04663-140">ブール値</span><span class="sxs-lookup"><span data-stu-id="04663-140">boolean</span></span>|<span data-ttu-id="04663-141">ChartTitle オブジェクトを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="04663-141">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="response"></a><span data-ttu-id="04663-142">応答</span><span class="sxs-lookup"><span data-stu-id="04663-142">Response</span></span>

<span data-ttu-id="04663-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [ChartTitle](../resources/charttitle.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="04663-143">If successful, this method returns a `200 OK` response code and updated [ChartTitle](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="04663-144">例</span><span class="sxs-lookup"><span data-stu-id="04663-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04663-145">要求</span><span class="sxs-lookup"><span data-stu-id="04663-145">Request</span></span>
<span data-ttu-id="04663-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="04663-146">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="04663-147">応答</span><span class="sxs-lookup"><span data-stu-id="04663-147">Response</span></span>
<span data-ttu-id="04663-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="04663-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update charttitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/charttitle-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
