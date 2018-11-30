---
title: 'workbookRangeView: itemAt'
description: この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「アクセス許可」を参照してください。
ms.openlocfilehash: b6af086e9867ca4c4d61a4102de1d2800163c453
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020264"
---
# <a name="workbookrangeview-itemat"></a><span data-ttu-id="24801-104">workbookRangeView: itemAt</span><span class="sxs-lookup"><span data-stu-id="24801-104">workbookRangeView: itemAt</span></span>


## <a name="permissions"></a><span data-ttu-id="24801-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="24801-105">Permissions</span></span>
<span data-ttu-id="24801-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="24801-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24801-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="24801-108">Permission type</span></span>      | <span data-ttu-id="24801-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="24801-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24801-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="24801-110">Delegated (work or school account)</span></span> | <span data-ttu-id="24801-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24801-111">Files.ReadWrite</span></span> |
|<span data-ttu-id="24801-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="24801-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24801-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24801-113">Not supported.</span></span>    |
|<span data-ttu-id="24801-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="24801-114">Application</span></span> | <span data-ttu-id="24801-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24801-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="24801-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="24801-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/itemAt(index={n})

```
## <a name="request-headers"></a><span data-ttu-id="24801-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="24801-117">Request headers</span></span>
| <span data-ttu-id="24801-118">名前</span><span class="sxs-lookup"><span data-stu-id="24801-118">Name</span></span>       | <span data-ttu-id="24801-119">説明</span><span class="sxs-lookup"><span data-stu-id="24801-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="24801-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="24801-120">Authorization</span></span>  | <span data-ttu-id="24801-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="24801-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="24801-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="24801-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="24801-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="24801-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="24801-126">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="24801-126">Function parameters</span></span>
<span data-ttu-id="24801-127">要求 URL に、次のクエリ パラメーターを値で指定します。</span><span class="sxs-lookup"><span data-stu-id="24801-127">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="24801-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="24801-128">Parameter</span></span>    | <span data-ttu-id="24801-129">型</span><span class="sxs-lookup"><span data-stu-id="24801-129">Type</span></span>   |<span data-ttu-id="24801-130">説明</span><span class="sxs-lookup"><span data-stu-id="24801-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24801-131">index</span><span class="sxs-lookup"><span data-stu-id="24801-131">index</span></span>|<span data-ttu-id="24801-132">Int32</span><span class="sxs-lookup"><span data-stu-id="24801-132">Int32</span></span>|<span data-ttu-id="24801-133">返される項目のインデックス。</span><span class="sxs-lookup"><span data-stu-id="24801-133">Index of the item to be returned.</span></span>|

## <a name="response"></a><span data-ttu-id="24801-134">応答</span><span class="sxs-lookup"><span data-stu-id="24801-134">Response</span></span>

<span data-ttu-id="24801-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRangeView](../resources/workbookrangeview.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="24801-135">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24801-136">例</span><span class="sxs-lookup"><span data-stu-id="24801-136">Example</span></span>
<span data-ttu-id="24801-137">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="24801-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="24801-138">要求</span><span class="sxs-lookup"><span data-stu-id="24801-138">Request</span></span>
<span data-ttu-id="24801-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="24801-139">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrangeview_itemat"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/itemAt(index=0)

```

##### <a name="response"></a><span data-ttu-id="24801-140">応答</span><span class="sxs-lookup"><span data-stu-id="24801-140">Response</span></span>
<span data-ttu-id="24801-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="24801-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
