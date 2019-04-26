---
title: 範囲:UsedRange
description: 指定した範囲オブジェクトのうち使用されている範囲を返します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5c6341e201c878744ade6732ba72b61406a0bdba
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331927"
---
# <a name="range-usedrange"></a><span data-ttu-id="34ce7-103">範囲:UsedRange</span><span class="sxs-lookup"><span data-stu-id="34ce7-103">Range: UsedRange</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34ce7-104">指定した範囲オブジェクトのうち使用されている範囲を返します。</span><span class="sxs-lookup"><span data-stu-id="34ce7-104">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="34ce7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="34ce7-105">Permissions</span></span>
<span data-ttu-id="34ce7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="34ce7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34ce7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="34ce7-108">Permission type</span></span>      | <span data-ttu-id="34ce7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="34ce7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34ce7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="34ce7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="34ce7-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34ce7-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="34ce7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="34ce7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34ce7-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34ce7-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="34ce7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="34ce7-114">Application</span></span> | <span data-ttu-id="34ce7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34ce7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="34ce7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="34ce7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/UsedRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/UsedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/UsedRange

```
## <a name="request-headers"></a><span data-ttu-id="34ce7-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="34ce7-117">Request headers</span></span>
| <span data-ttu-id="34ce7-118">名前</span><span class="sxs-lookup"><span data-stu-id="34ce7-118">Name</span></span>       | <span data-ttu-id="34ce7-119">説明</span><span class="sxs-lookup"><span data-stu-id="34ce7-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="34ce7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="34ce7-120">Authorization</span></span>  | <span data-ttu-id="34ce7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="34ce7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="34ce7-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="34ce7-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="34ce7-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="34ce7-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="34ce7-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="34ce7-126">Request body</span></span>
<span data-ttu-id="34ce7-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="34ce7-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="34ce7-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="34ce7-128">Parameter</span></span>    | <span data-ttu-id="34ce7-129">型</span><span class="sxs-lookup"><span data-stu-id="34ce7-129">Type</span></span>   |<span data-ttu-id="34ce7-130">説明</span><span class="sxs-lookup"><span data-stu-id="34ce7-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34ce7-131">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="34ce7-131">valuesOnly</span></span>|<span data-ttu-id="34ce7-132">ブール値</span><span class="sxs-lookup"><span data-stu-id="34ce7-132">boolean</span></span>|<span data-ttu-id="34ce7-p104">省略可能。値の入っているセルのみを使用セルと見なします。</span><span class="sxs-lookup"><span data-stu-id="34ce7-p104">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="34ce7-135">応答</span><span class="sxs-lookup"><span data-stu-id="34ce7-135">Response</span></span>

<span data-ttu-id="34ce7-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRange](../resources/workbookrange.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="34ce7-136">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34ce7-137">例</span><span class="sxs-lookup"><span data-stu-id="34ce7-137">Example</span></span>
<span data-ttu-id="34ce7-138">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="34ce7-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="34ce7-139">要求</span><span class="sxs-lookup"><span data-stu-id="34ce7-139">Request</span></span>
<span data-ttu-id="34ce7-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="34ce7-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_usedrange"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/UsedRange
Content-type: application/json
Content-length: 24

{
  "valuesOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="34ce7-141">応答</span><span class="sxs-lookup"><span data-stu-id="34ce7-141">Response</span></span>
<span data-ttu-id="34ce7-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="34ce7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
