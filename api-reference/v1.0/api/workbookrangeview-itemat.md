---
title: 'workbookRangeView: itemAt'
description: この API を呼び出すには、次のいずれかのアクセス許可が必要です。 アクセス許可の選択方法などの詳細については、「アクセス許可」を参照してください。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c9f453a6fa2dfb3c5777389683004af558f87b26
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36026279"
---
# <a name="workbookrangeview-itemat"></a><span data-ttu-id="602c1-104">workbookRangeView: itemAt</span><span class="sxs-lookup"><span data-stu-id="602c1-104">workbookRangeView: itemAt</span></span>


## <a name="permissions"></a><span data-ttu-id="602c1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="602c1-105">Permissions</span></span>
<span data-ttu-id="602c1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="602c1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="602c1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="602c1-108">Permission type</span></span>      | <span data-ttu-id="602c1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="602c1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="602c1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="602c1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="602c1-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="602c1-111">Files.ReadWrite</span></span> |
|<span data-ttu-id="602c1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="602c1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="602c1-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="602c1-113">Not supported.</span></span>    |
|<span data-ttu-id="602c1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="602c1-114">Application</span></span> | <span data-ttu-id="602c1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="602c1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="602c1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="602c1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/itemAt(index={n})

```
## <a name="request-headers"></a><span data-ttu-id="602c1-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="602c1-117">Request headers</span></span>
| <span data-ttu-id="602c1-118">名前</span><span class="sxs-lookup"><span data-stu-id="602c1-118">Name</span></span>       | <span data-ttu-id="602c1-119">説明</span><span class="sxs-lookup"><span data-stu-id="602c1-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="602c1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="602c1-120">Authorization</span></span>  | <span data-ttu-id="602c1-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="602c1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="602c1-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="602c1-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="602c1-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="602c1-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="602c1-126">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="602c1-126">Function parameters</span></span>
<span data-ttu-id="602c1-127">要求 URL に、次のクエリ パラメーターを値で指定します。</span><span class="sxs-lookup"><span data-stu-id="602c1-127">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="602c1-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="602c1-128">Parameter</span></span>    | <span data-ttu-id="602c1-129">型</span><span class="sxs-lookup"><span data-stu-id="602c1-129">Type</span></span>   |<span data-ttu-id="602c1-130">説明</span><span class="sxs-lookup"><span data-stu-id="602c1-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="602c1-131">index</span><span class="sxs-lookup"><span data-stu-id="602c1-131">index</span></span>|<span data-ttu-id="602c1-132">Int32</span><span class="sxs-lookup"><span data-stu-id="602c1-132">Int32</span></span>|<span data-ttu-id="602c1-133">返される項目のインデックス。</span><span class="sxs-lookup"><span data-stu-id="602c1-133">Index of the item to be returned.</span></span>|

## <a name="response"></a><span data-ttu-id="602c1-134">応答</span><span class="sxs-lookup"><span data-stu-id="602c1-134">Response</span></span>

<span data-ttu-id="602c1-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRangeView](../resources/workbookrangeview.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="602c1-135">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="602c1-136">例</span><span class="sxs-lookup"><span data-stu-id="602c1-136">Example</span></span>
<span data-ttu-id="602c1-137">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="602c1-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="602c1-138">要求</span><span class="sxs-lookup"><span data-stu-id="602c1-138">Request</span></span>
<span data-ttu-id="602c1-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="602c1-139">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrangeview_itemat"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/itemAt(index=0)

```

##### <a name="response"></a><span data-ttu-id="602c1-140">応答</span><span class="sxs-lookup"><span data-stu-id="602c1-140">Response</span></span>
<span data-ttu-id="602c1-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="602c1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
