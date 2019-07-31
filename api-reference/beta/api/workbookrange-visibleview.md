---
title: 'workbookRange: visibleView'
description: この API を呼び出すには、次のいずれかのアクセス許可が必要です。 アクセス許可の選択方法などの詳細については、「アクセス許可」を参照してください。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f91b5044c470430d8d508cab3585db48b51048bf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35995868"
---
# <a name="workbookrange-visibleview"></a><span data-ttu-id="00330-104">workbookRange: visibleView</span><span class="sxs-lookup"><span data-stu-id="00330-104">workbookRange: visibleView</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="00330-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="00330-105">Permissions</span></span>
<span data-ttu-id="00330-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="00330-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00330-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="00330-108">Permission type</span></span>      | <span data-ttu-id="00330-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="00330-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00330-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="00330-110">Delegated (work or school account)</span></span> | <span data-ttu-id="00330-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00330-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="00330-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="00330-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00330-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00330-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="00330-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="00330-114">Application</span></span> | <span data-ttu-id="00330-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00330-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="00330-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="00330-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView
```
## <a name="request-headers"></a><span data-ttu-id="00330-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="00330-117">Request headers</span></span>
| <span data-ttu-id="00330-118">名前</span><span class="sxs-lookup"><span data-stu-id="00330-118">Name</span></span>       | <span data-ttu-id="00330-119">説明</span><span class="sxs-lookup"><span data-stu-id="00330-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="00330-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="00330-120">Authorization</span></span>  | <span data-ttu-id="00330-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="00330-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="00330-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="00330-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="00330-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="00330-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="00330-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="00330-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="00330-127">応答</span><span class="sxs-lookup"><span data-stu-id="00330-127">Response</span></span>

<span data-ttu-id="00330-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRangeView](../resources/workbookrangeview.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="00330-128">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00330-129">例</span><span class="sxs-lookup"><span data-stu-id="00330-129">Example</span></span>
<span data-ttu-id="00330-130">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="00330-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="00330-131">要求</span><span class="sxs-lookup"><span data-stu-id="00330-131">Request</span></span>
<span data-ttu-id="00330-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="00330-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_visibleview"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView
```

##### <a name="response"></a><span data-ttu-id="00330-133">応答</span><span class="sxs-lookup"><span data-stu-id="00330-133">Response</span></span>
<span data-ttu-id="00330-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="00330-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
