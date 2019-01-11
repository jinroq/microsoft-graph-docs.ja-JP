---
title: 'workbookRange: visibleView'
description: この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「アクセス許可」を参照してください。
localization_priority: Normal
ms.openlocfilehash: f994866c8f55ec2ffbc0b680d4576fbc6a8b7bb8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875167"
---
# <a name="workbookrange-visibleview"></a><span data-ttu-id="27e53-104">workbookRange: visibleView</span><span class="sxs-lookup"><span data-stu-id="27e53-104">workbookRange: visibleView</span></span>

> <span data-ttu-id="27e53-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="27e53-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27e53-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27e53-106">Use of these APIs in production applications is not supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="27e53-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="27e53-107">Permissions</span></span>
<span data-ttu-id="27e53-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="27e53-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27e53-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="27e53-110">Permission type</span></span>      | <span data-ttu-id="27e53-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="27e53-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27e53-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="27e53-112">Delegated (work or school account)</span></span> | <span data-ttu-id="27e53-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27e53-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="27e53-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="27e53-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27e53-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27e53-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="27e53-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="27e53-116">Application</span></span> | <span data-ttu-id="27e53-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27e53-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="27e53-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="27e53-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView
```
## <a name="request-headers"></a><span data-ttu-id="27e53-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="27e53-119">Request headers</span></span>
| <span data-ttu-id="27e53-120">名前</span><span class="sxs-lookup"><span data-stu-id="27e53-120">Name</span></span>       | <span data-ttu-id="27e53-121">説明</span><span class="sxs-lookup"><span data-stu-id="27e53-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="27e53-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="27e53-122">Authorization</span></span>  | <span data-ttu-id="27e53-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="27e53-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="27e53-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="27e53-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="27e53-p105">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="27e53-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="27e53-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="27e53-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="27e53-129">応答</span><span class="sxs-lookup"><span data-stu-id="27e53-129">Response</span></span>

<span data-ttu-id="27e53-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRangeView](../resources/workbookrangeview.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="27e53-130">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27e53-131">例</span><span class="sxs-lookup"><span data-stu-id="27e53-131">Example</span></span>
<span data-ttu-id="27e53-132">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="27e53-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="27e53-133">要求</span><span class="sxs-lookup"><span data-stu-id="27e53-133">Request</span></span>
<span data-ttu-id="27e53-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="27e53-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_visibleview"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView
```

##### <a name="response"></a><span data-ttu-id="27e53-135">応答</span><span class="sxs-lookup"><span data-stu-id="27e53-135">Response</span></span>
<span data-ttu-id="27e53-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="27e53-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
