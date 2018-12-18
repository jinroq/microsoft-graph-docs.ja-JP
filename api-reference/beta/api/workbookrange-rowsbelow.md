---
title: 'workbookRange: rowsBelow'
description: 指定した範囲の下にある特定の行数を取得します。
author: lumine2008
ms.openlocfilehash: c6b7641dbc784c3c3fe7522308729877b7eb2ff9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337535"
---
# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="e193e-103">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="e193e-103">workbookRange: rowsBelow</span></span>

> <span data-ttu-id="e193e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e193e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e193e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e193e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e193e-106">指定した範囲の下にある特定の行数を取得します。</span><span class="sxs-lookup"><span data-stu-id="e193e-106">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="e193e-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e193e-107">Permissions</span></span>
<span data-ttu-id="e193e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e193e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e193e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e193e-110">Permission type</span></span>      | <span data-ttu-id="e193e-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e193e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e193e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e193e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e193e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e193e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e193e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e193e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e193e-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e193e-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e193e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e193e-116">Application</span></span> | <span data-ttu-id="e193e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e193e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e193e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e193e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="e193e-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="e193e-119">Function parameters</span></span>

| <span data-ttu-id="e193e-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e193e-120">Parameter</span></span>    | <span data-ttu-id="e193e-121">種類</span><span class="sxs-lookup"><span data-stu-id="e193e-121">Type</span></span>   |<span data-ttu-id="e193e-122">説明</span><span class="sxs-lookup"><span data-stu-id="e193e-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e193e-123">count</span><span class="sxs-lookup"><span data-stu-id="e193e-123">count</span></span>|<span data-ttu-id="e193e-124">Int32</span><span class="sxs-lookup"><span data-stu-id="e193e-124">Int32</span></span>|<span data-ttu-id="e193e-p103">省略可能。結果の範囲に含める行の数です。通常、正の数値を使用して現在の範囲外に範囲を作成します。負の数値を使用して、現在の範囲内に範囲を作成することもできます。既定値は 1 です。</span><span class="sxs-lookup"><span data-stu-id="e193e-p103">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="e193e-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e193e-130">Request headers</span></span>
| <span data-ttu-id="e193e-131">名前</span><span class="sxs-lookup"><span data-stu-id="e193e-131">Name</span></span>       | <span data-ttu-id="e193e-132">説明</span><span class="sxs-lookup"><span data-stu-id="e193e-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e193e-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="e193e-133">Authorization</span></span>  | <span data-ttu-id="e193e-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e193e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e193e-136">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e193e-136">Workbook-Session-Id</span></span>  | <span data-ttu-id="e193e-p105">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="e193e-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e193e-139">要求本文</span><span class="sxs-lookup"><span data-stu-id="e193e-139">Request body</span></span>
<span data-ttu-id="e193e-140">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e193e-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e193e-141">応答</span><span class="sxs-lookup"><span data-stu-id="e193e-141">Response</span></span>

<span data-ttu-id="e193e-142">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRange](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e193e-142">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e193e-143">例</span><span class="sxs-lookup"><span data-stu-id="e193e-143">Example</span></span>
<span data-ttu-id="e193e-144">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="e193e-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e193e-145">要求</span><span class="sxs-lookup"><span data-stu-id="e193e-145">Request</span></span>
<span data-ttu-id="e193e-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e193e-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_rowsBelow"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```

##### <a name="response"></a><span data-ttu-id="e193e-147">応答</span><span class="sxs-lookup"><span data-stu-id="e193e-147">Response</span></span>
<span data-ttu-id="e193e-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e193e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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