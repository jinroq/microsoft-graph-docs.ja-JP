---
title: 範囲:LastCell
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 56fd2adea1f2f3bd13e85b035f81835cd18ea0f3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966329"
---
# <a name="range-lastcell"></a><span data-ttu-id="c0afe-103">範囲:LastCell</span><span class="sxs-lookup"><span data-stu-id="c0afe-103">Range: LastCell</span></span>

> <span data-ttu-id="c0afe-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c0afe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0afe-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0afe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c0afe-p102">範囲内の最後のセルを取得します。たとえば、"B2:D5" の最後のセルは "D5" になります。</span><span class="sxs-lookup"><span data-stu-id="c0afe-p102">Gets the last cell within the range. For example, the last cell of "B2:D5" is "D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="c0afe-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c0afe-108">Permissions</span></span>
<span data-ttu-id="c0afe-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0afe-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0afe-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c0afe-111">Permission type</span></span>      | <span data-ttu-id="c0afe-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c0afe-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0afe-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c0afe-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c0afe-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0afe-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c0afe-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c0afe-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0afe-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0afe-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c0afe-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c0afe-117">Application</span></span> | <span data-ttu-id="c0afe-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0afe-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0afe-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c0afe-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/LastCell
GET /workbook/worksheets/{id|name}/range(address='<address>')/LastCell
GET /workbook/tables/{id|name}/columns/{id|name}/range/LastCell

```
## <a name="request-headers"></a><span data-ttu-id="c0afe-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c0afe-120">Request headers</span></span>
| <span data-ttu-id="c0afe-121">名前</span><span class="sxs-lookup"><span data-stu-id="c0afe-121">Name</span></span>       | <span data-ttu-id="c0afe-122">説明</span><span class="sxs-lookup"><span data-stu-id="c0afe-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c0afe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0afe-123">Authorization</span></span>  | <span data-ttu-id="c0afe-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c0afe-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c0afe-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c0afe-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="c0afe-p105">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="c0afe-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0afe-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="c0afe-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="c0afe-130">応答</span><span class="sxs-lookup"><span data-stu-id="c0afe-130">Response</span></span>

<span data-ttu-id="c0afe-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c0afe-131">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0afe-132">例</span><span class="sxs-lookup"><span data-stu-id="c0afe-132">Example</span></span>
<span data-ttu-id="c0afe-133">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="c0afe-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c0afe-134">要求</span><span class="sxs-lookup"><span data-stu-id="c0afe-134">Request</span></span>
<span data-ttu-id="c0afe-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c0afe-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_lastcell"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/LastCell
```

##### <a name="response"></a><span data-ttu-id="c0afe-136">応答</span><span class="sxs-lookup"><span data-stu-id="c0afe-136">Response</span></span>
<span data-ttu-id="c0afe-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c0afe-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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
<!-- {
  "type": "#page.annotation",
  "description": "Range: LastCell",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
