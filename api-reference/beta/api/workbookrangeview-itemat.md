---
title: 'workbookRangeView: itemAt'
description: この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「アクセス許可」を参照してください。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 423c20f6cbdcbfe65a2f8db965a4765c93079f18
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960582"
---
# <a name="workbookrangeview-itemat"></a><span data-ttu-id="475e2-104">workbookRangeView: itemAt</span><span class="sxs-lookup"><span data-stu-id="475e2-104">workbookRangeView: itemAt</span></span>

> <span data-ttu-id="475e2-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="475e2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="475e2-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="475e2-106">Use of these APIs in production applications is not supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="475e2-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="475e2-107">Permissions</span></span>
<span data-ttu-id="475e2-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="475e2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="475e2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="475e2-110">Permission type</span></span>      | <span data-ttu-id="475e2-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="475e2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="475e2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="475e2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="475e2-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="475e2-113">Not supported.</span></span>    |
|<span data-ttu-id="475e2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="475e2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="475e2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="475e2-115">Not supported.</span></span>    |
|<span data-ttu-id="475e2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="475e2-116">Application</span></span> | <span data-ttu-id="475e2-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="475e2-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="475e2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="475e2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/itemAt(index={n})

```
## <a name="request-headers"></a><span data-ttu-id="475e2-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="475e2-119">Request headers</span></span>
| <span data-ttu-id="475e2-120">名前</span><span class="sxs-lookup"><span data-stu-id="475e2-120">Name</span></span>       | <span data-ttu-id="475e2-121">説明</span><span class="sxs-lookup"><span data-stu-id="475e2-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="475e2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="475e2-122">Authorization</span></span>  | <span data-ttu-id="475e2-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="475e2-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="475e2-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="475e2-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="475e2-p105">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="475e2-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="475e2-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="475e2-128">Request body</span></span>
<span data-ttu-id="475e2-129">要求 URL に、次のクエリ パラメーターを値で指定します。</span><span class="sxs-lookup"><span data-stu-id="475e2-129">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="475e2-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="475e2-130">Parameter</span></span>    | <span data-ttu-id="475e2-131">型</span><span class="sxs-lookup"><span data-stu-id="475e2-131">Type</span></span>   |<span data-ttu-id="475e2-132">説明</span><span class="sxs-lookup"><span data-stu-id="475e2-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="475e2-133">index</span><span class="sxs-lookup"><span data-stu-id="475e2-133">index</span></span>|<span data-ttu-id="475e2-134">Int32</span><span class="sxs-lookup"><span data-stu-id="475e2-134">Int32</span></span>|<span data-ttu-id="475e2-135">返される項目のインデックス。</span><span class="sxs-lookup"><span data-stu-id="475e2-135">Index of the item to be returned.</span></span>|

## <a name="response"></a><span data-ttu-id="475e2-136">応答</span><span class="sxs-lookup"><span data-stu-id="475e2-136">Response</span></span>

<span data-ttu-id="475e2-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRangeView](../resources/workbookrangeview.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="475e2-137">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="475e2-138">例</span><span class="sxs-lookup"><span data-stu-id="475e2-138">Example</span></span>
<span data-ttu-id="475e2-139">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="475e2-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="475e2-140">要求</span><span class="sxs-lookup"><span data-stu-id="475e2-140">Request</span></span>
<span data-ttu-id="475e2-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="475e2-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_itemat"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/itemAt(index=0)

```

##### <a name="response"></a><span data-ttu-id="475e2-142">応答</span><span class="sxs-lookup"><span data-stu-id="475e2-142">Response</span></span>
<span data-ttu-id="475e2-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="475e2-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeView"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

{
  "cellAddresses": "cellAddresses-value",
  "columnCount": 99,
  "formulas": "formulas-value",
  "formulasLocal": "formulasLocal-value",
  "formulasR1C1": "formulasR1C1-value",
  "index": 99
}
```
