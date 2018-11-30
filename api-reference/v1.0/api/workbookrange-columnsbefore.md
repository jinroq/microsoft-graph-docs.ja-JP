---
title: 'workbookRange: columnsBefore'
description: 指定した範囲の左にある特定の列数を取得します。
ms.openlocfilehash: c6214baadd520637554038b0f344efaa066533ca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023857"
---
# <a name="workbookrange-columnsbefore"></a><span data-ttu-id="785a7-103">workbookRange: columnsBefore</span><span class="sxs-lookup"><span data-stu-id="785a7-103">workbookRange: columnsBefore</span></span>

<span data-ttu-id="785a7-104">指定した範囲の左にある特定の列数を取得します。</span><span class="sxs-lookup"><span data-stu-id="785a7-104">Gets a certain number of columns to the left of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="785a7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="785a7-105">Permissions</span></span>
<span data-ttu-id="785a7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="785a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="785a7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="785a7-108">Permission type</span></span>      | <span data-ttu-id="785a7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="785a7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="785a7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="785a7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="785a7-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="785a7-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="785a7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="785a7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="785a7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="785a7-113">Not supported.</span></span>    |
|<span data-ttu-id="785a7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="785a7-114">Application</span></span> | <span data-ttu-id="785a7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="785a7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="785a7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="785a7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="785a7-117">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="785a7-117">Function parameters</span></span>

| <span data-ttu-id="785a7-118">パラメーター</span><span class="sxs-lookup"><span data-stu-id="785a7-118">Parameter</span></span>    | <span data-ttu-id="785a7-119">型</span><span class="sxs-lookup"><span data-stu-id="785a7-119">Type</span></span>   |<span data-ttu-id="785a7-120">説明</span><span class="sxs-lookup"><span data-stu-id="785a7-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="785a7-121">count</span><span class="sxs-lookup"><span data-stu-id="785a7-121">count</span></span>|<span data-ttu-id="785a7-122">Int32</span><span class="sxs-lookup"><span data-stu-id="785a7-122">Int32</span></span>|<span data-ttu-id="785a7-p102">省略可能。結果の範囲に含める列の数です。通常、正の数値を使用して現在の範囲外に範囲を作成します。負の数値を使用して、現在の範囲内に範囲を作成することもできます。既定値は 1 です。</span><span class="sxs-lookup"><span data-stu-id="785a7-p102">Optional. The number of columns to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="785a7-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="785a7-128">Request headers</span></span>
| <span data-ttu-id="785a7-129">名前</span><span class="sxs-lookup"><span data-stu-id="785a7-129">Name</span></span>       | <span data-ttu-id="785a7-130">説明</span><span class="sxs-lookup"><span data-stu-id="785a7-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="785a7-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="785a7-131">Authorization</span></span>  | <span data-ttu-id="785a7-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="785a7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="785a7-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="785a7-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="785a7-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="785a7-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="785a7-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="785a7-137">Request body</span></span>
<span data-ttu-id="785a7-138">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="785a7-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="785a7-139">応答</span><span class="sxs-lookup"><span data-stu-id="785a7-139">Response</span></span>
<span data-ttu-id="785a7-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRange](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="785a7-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="785a7-141">例</span><span class="sxs-lookup"><span data-stu-id="785a7-141">Example</span></span>
<span data-ttu-id="785a7-142">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="785a7-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="785a7-143">要求</span><span class="sxs-lookup"><span data-stu-id="785a7-143">Request</span></span>
<span data-ttu-id="785a7-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="785a7-144">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_columnsbefore",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=2)
```

##### <a name="response"></a><span data-ttu-id="785a7-145">応答</span><span class="sxs-lookup"><span data-stu-id="785a7-145">Response</span></span>
<span data-ttu-id="785a7-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="785a7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
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
