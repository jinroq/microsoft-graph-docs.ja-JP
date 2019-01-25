---
title: Update chartseries
description: chartseries オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 312c2a0a219cd1f88ede106f253c0c9019109253
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514580"
---
# <a name="update-chartseries"></a><span data-ttu-id="063d6-103">Update chartseries</span><span class="sxs-lookup"><span data-stu-id="063d6-103">Update chartseries</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="063d6-104">chartseries オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="063d6-104">Update the properties of chartseries object.</span></span>
## <a name="permissions"></a><span data-ttu-id="063d6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="063d6-105">Permissions</span></span>
<span data-ttu-id="063d6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="063d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="063d6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="063d6-108">Permission type</span></span>      | <span data-ttu-id="063d6-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="063d6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="063d6-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="063d6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="063d6-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="063d6-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="063d6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="063d6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="063d6-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="063d6-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="063d6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="063d6-114">Application</span></span> | <span data-ttu-id="063d6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="063d6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="063d6-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="063d6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="063d6-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="063d6-117">Optional request headers</span></span>
| <span data-ttu-id="063d6-118">名前</span><span class="sxs-lookup"><span data-stu-id="063d6-118">Name</span></span>       | <span data-ttu-id="063d6-119">説明</span><span class="sxs-lookup"><span data-stu-id="063d6-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="063d6-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="063d6-120">Authorization</span></span>  | <span data-ttu-id="063d6-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="063d6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="063d6-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="063d6-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="063d6-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="063d6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="063d6-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="063d6-126">Request body</span></span>
<span data-ttu-id="063d6-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="063d6-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="063d6-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="063d6-130">Property</span></span>     | <span data-ttu-id="063d6-131">型</span><span class="sxs-lookup"><span data-stu-id="063d6-131">Type</span></span>   |<span data-ttu-id="063d6-132">説明</span><span class="sxs-lookup"><span data-stu-id="063d6-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="063d6-133">name</span><span class="sxs-lookup"><span data-stu-id="063d6-133">name</span></span>|<span data-ttu-id="063d6-134">文字列</span><span class="sxs-lookup"><span data-stu-id="063d6-134">string</span></span>|<span data-ttu-id="063d6-135">グラフのデータ系列の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="063d6-135">Represents the name of a series in a chart.</span></span>|

## <a name="response"></a><span data-ttu-id="063d6-136">応答</span><span class="sxs-lookup"><span data-stu-id="063d6-136">Response</span></span>

<span data-ttu-id="063d6-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [ChartSeries](../resources/chartseries.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="063d6-137">If successful, this method returns a `200 OK` response code and updated [ChartSeries](../resources/chartseries.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="063d6-138">例</span><span class="sxs-lookup"><span data-stu-id="063d6-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="063d6-139">要求</span><span class="sxs-lookup"><span data-stu-id="063d6-139">Request</span></span>
<span data-ttu-id="063d6-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="063d6-140">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="063d6-141">応答</span><span class="sxs-lookup"><span data-stu-id="063d6-141">Response</span></span>
<span data-ttu-id="063d6-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="063d6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update chartseries",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartseries-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
