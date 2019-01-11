---
title: 'workbookRangeView: range'
description: rangeView リソースに関連付けられている範囲を返します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 8c116a80e01c0b649ff1846de3e324874e7dd837
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863421"
---
# <a name="workbookrangeview-range"></a><span data-ttu-id="c0eb6-103">workbookRangeView: range</span><span class="sxs-lookup"><span data-stu-id="c0eb6-103">workbookRangeView: range</span></span>

> <span data-ttu-id="c0eb6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c0eb6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0eb6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0eb6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c0eb6-106">rangeView リソースに関連付けられている範囲を返します。</span><span class="sxs-lookup"><span data-stu-id="c0eb6-106">Return the range associated with the rangeView resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0eb6-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c0eb6-107">Permissions</span></span>
<span data-ttu-id="c0eb6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0eb6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c0eb6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c0eb6-110">Permission type</span></span>      | <span data-ttu-id="c0eb6-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c0eb6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0eb6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c0eb6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c0eb6-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0eb6-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c0eb6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c0eb6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0eb6-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0eb6-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c0eb6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c0eb6-116">Application</span></span> | <span data-ttu-id="c0eb6-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0eb6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0eb6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c0eb6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/range

```
## <a name="request-headers"></a><span data-ttu-id="c0eb6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c0eb6-119">Request headers</span></span>
| <span data-ttu-id="c0eb6-120">名前</span><span class="sxs-lookup"><span data-stu-id="c0eb6-120">Name</span></span>       | <span data-ttu-id="c0eb6-121">説明</span><span class="sxs-lookup"><span data-stu-id="c0eb6-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c0eb6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0eb6-122">Authorization</span></span>  | <span data-ttu-id="c0eb6-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c0eb6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c0eb6-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c0eb6-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="c0eb6-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="c0eb6-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0eb6-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="c0eb6-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="c0eb6-129">応答</span><span class="sxs-lookup"><span data-stu-id="c0eb6-129">Response</span></span>

<span data-ttu-id="c0eb6-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRange](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c0eb6-130">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0eb6-131">例</span><span class="sxs-lookup"><span data-stu-id="c0eb6-131">Example</span></span>
<span data-ttu-id="c0eb6-132">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="c0eb6-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c0eb6-133">要求</span><span class="sxs-lookup"><span data-stu-id="c0eb6-133">Request</span></span>
<span data-ttu-id="c0eb6-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c0eb6-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_range"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/range
```

##### <a name="response"></a><span data-ttu-id="c0eb6-135">応答</span><span class="sxs-lookup"><span data-stu-id="c0eb6-135">Response</span></span>
<span data-ttu-id="c0eb6-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c0eb6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
