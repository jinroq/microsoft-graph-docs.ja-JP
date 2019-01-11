---
title: 'workbookRange: columnsBefore'
description: 指定した範囲の左にある特定の列数を取得します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 8eff3ffd7291f9e3ae3537fc660760550b3b536e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830115"
---
# <a name="workbookrange-columnsbefore"></a><span data-ttu-id="dc43c-103">workbookRange: columnsBefore</span><span class="sxs-lookup"><span data-stu-id="dc43c-103">workbookRange: columnsBefore</span></span>

> <span data-ttu-id="dc43c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dc43c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc43c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc43c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dc43c-106">指定した範囲の左にある特定の列数を取得します。</span><span class="sxs-lookup"><span data-stu-id="dc43c-106">Gets a certain number of columns to the left of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc43c-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dc43c-107">Permissions</span></span>
<span data-ttu-id="dc43c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dc43c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc43c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dc43c-110">Permission type</span></span>      | <span data-ttu-id="dc43c-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dc43c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc43c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dc43c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dc43c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc43c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dc43c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dc43c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc43c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc43c-115">Not supported.</span></span>    |
|<span data-ttu-id="dc43c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dc43c-116">Application</span></span> | <span data-ttu-id="dc43c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc43c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc43c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dc43c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="dc43c-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="dc43c-119">Function parameters</span></span>

| <span data-ttu-id="dc43c-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="dc43c-120">Parameter</span></span>    | <span data-ttu-id="dc43c-121">Type</span><span class="sxs-lookup"><span data-stu-id="dc43c-121">Type</span></span>   |<span data-ttu-id="dc43c-122">説明</span><span class="sxs-lookup"><span data-stu-id="dc43c-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc43c-123">count</span><span class="sxs-lookup"><span data-stu-id="dc43c-123">count</span></span>|<span data-ttu-id="dc43c-124">Int32</span><span class="sxs-lookup"><span data-stu-id="dc43c-124">Int32</span></span>|<span data-ttu-id="dc43c-p103">結果の範囲に含める列の数です。通常、正の数値を使用して現在の範囲外に範囲を作成します。負の数値を使用して、現在の範囲内に範囲を作成することもできます。既定値は 1 です。</span><span class="sxs-lookup"><span data-stu-id="dc43c-p103">The number of columns to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="dc43c-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dc43c-129">Request headers</span></span>
| <span data-ttu-id="dc43c-130">名前</span><span class="sxs-lookup"><span data-stu-id="dc43c-130">Name</span></span>       | <span data-ttu-id="dc43c-131">説明</span><span class="sxs-lookup"><span data-stu-id="dc43c-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dc43c-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc43c-132">Authorization</span></span>  | <span data-ttu-id="dc43c-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="dc43c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dc43c-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dc43c-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="dc43c-p105">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="dc43c-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc43c-138">要求本文</span><span class="sxs-lookup"><span data-stu-id="dc43c-138">Request body</span></span>
<span data-ttu-id="dc43c-139">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="dc43c-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc43c-140">応答</span><span class="sxs-lookup"><span data-stu-id="dc43c-140">Response</span></span>
<span data-ttu-id="dc43c-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRange](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dc43c-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc43c-142">例</span><span class="sxs-lookup"><span data-stu-id="dc43c-142">Example</span></span>
<span data-ttu-id="dc43c-143">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="dc43c-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dc43c-144">要求</span><span class="sxs-lookup"><span data-stu-id="dc43c-144">Request</span></span>
<span data-ttu-id="dc43c-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dc43c-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_columnsbefore"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=2)
```

##### <a name="response"></a><span data-ttu-id="dc43c-146">応答</span><span class="sxs-lookup"><span data-stu-id="dc43c-146">Response</span></span>
<span data-ttu-id="dc43c-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dc43c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
