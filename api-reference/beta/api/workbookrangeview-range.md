---
title: 'workbookRangeView: range'
description: rangeView リソースに関連付けられている範囲を返します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 616d65c490f7691ec8ab83ffd12eaba480f4734a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970907"
---
# <a name="workbookrangeview-range"></a><span data-ttu-id="86fbf-103">workbookRangeView: range</span><span class="sxs-lookup"><span data-stu-id="86fbf-103">workbookRangeView: range</span></span>

> <span data-ttu-id="86fbf-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="86fbf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="86fbf-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86fbf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="86fbf-106">rangeView リソースに関連付けられている範囲を返します。</span><span class="sxs-lookup"><span data-stu-id="86fbf-106">Return the range associated with the rangeView resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="86fbf-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="86fbf-107">Permissions</span></span>
<span data-ttu-id="86fbf-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="86fbf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="86fbf-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="86fbf-110">Permission type</span></span>      | <span data-ttu-id="86fbf-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="86fbf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86fbf-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="86fbf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="86fbf-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="86fbf-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="86fbf-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="86fbf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86fbf-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="86fbf-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="86fbf-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="86fbf-116">Application</span></span> | <span data-ttu-id="86fbf-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86fbf-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="86fbf-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="86fbf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/range

```
## <a name="request-headers"></a><span data-ttu-id="86fbf-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="86fbf-119">Request headers</span></span>
| <span data-ttu-id="86fbf-120">名前</span><span class="sxs-lookup"><span data-stu-id="86fbf-120">Name</span></span>       | <span data-ttu-id="86fbf-121">説明</span><span class="sxs-lookup"><span data-stu-id="86fbf-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="86fbf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="86fbf-122">Authorization</span></span>  | <span data-ttu-id="86fbf-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="86fbf-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="86fbf-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="86fbf-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="86fbf-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="86fbf-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="86fbf-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="86fbf-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="86fbf-129">応答</span><span class="sxs-lookup"><span data-stu-id="86fbf-129">Response</span></span>

<span data-ttu-id="86fbf-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRange](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="86fbf-130">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86fbf-131">例</span><span class="sxs-lookup"><span data-stu-id="86fbf-131">Example</span></span>
<span data-ttu-id="86fbf-132">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="86fbf-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="86fbf-133">要求</span><span class="sxs-lookup"><span data-stu-id="86fbf-133">Request</span></span>
<span data-ttu-id="86fbf-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="86fbf-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_range"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/range
```

##### <a name="response"></a><span data-ttu-id="86fbf-135">応答</span><span class="sxs-lookup"><span data-stu-id="86fbf-135">Response</span></span>
<span data-ttu-id="86fbf-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="86fbf-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
