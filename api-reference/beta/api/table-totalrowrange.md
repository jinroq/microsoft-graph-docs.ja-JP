---
title: Table:TotalRowRange
description: テーブルの集計行に関連付けられた範囲オブジェクトを取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 8e0294b778edf9c8b077cffeb5a5c3349b5abb93
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923790"
---
# <a name="table-totalrowrange"></a><span data-ttu-id="c4ece-103">Table:TotalRowRange</span><span class="sxs-lookup"><span data-stu-id="c4ece-103">Table: TotalRowRange</span></span>

> <span data-ttu-id="c4ece-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c4ece-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4ece-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4ece-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c4ece-106">テーブルの集計行に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="c4ece-106">Gets the range object associated with totals row of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="c4ece-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c4ece-107">Permissions</span></span>
<span data-ttu-id="c4ece-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c4ece-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4ece-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c4ece-110">Permission type</span></span>      | <span data-ttu-id="c4ece-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c4ece-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4ece-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c4ece-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c4ece-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4ece-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c4ece-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c4ece-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4ece-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4ece-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c4ece-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c4ece-116">Application</span></span> | <span data-ttu-id="c4ece-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4ece-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4ece-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c4ece-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/TotalRowRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/TotalRowRange

```
## <a name="request-headers"></a><span data-ttu-id="c4ece-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c4ece-119">Request headers</span></span>
| <span data-ttu-id="c4ece-120">名前</span><span class="sxs-lookup"><span data-stu-id="c4ece-120">Name</span></span>       | <span data-ttu-id="c4ece-121">説明</span><span class="sxs-lookup"><span data-stu-id="c4ece-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c4ece-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4ece-122">Authorization</span></span>  | <span data-ttu-id="c4ece-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c4ece-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c4ece-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c4ece-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="c4ece-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="c4ece-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4ece-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="c4ece-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="c4ece-129">応答</span><span class="sxs-lookup"><span data-stu-id="c4ece-129">Response</span></span>

<span data-ttu-id="c4ece-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c4ece-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4ece-131">例</span><span class="sxs-lookup"><span data-stu-id="c4ece-131">Example</span></span>
<span data-ttu-id="c4ece-132">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="c4ece-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c4ece-133">要求</span><span class="sxs-lookup"><span data-stu-id="c4ece-133">Request</span></span>
<span data-ttu-id="c4ece-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c4ece-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_totalrowrange"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/TotalRowRange
```

##### <a name="response"></a><span data-ttu-id="c4ece-135">応答</span><span class="sxs-lookup"><span data-stu-id="c4ece-135">Response</span></span>
<span data-ttu-id="c4ece-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c4ece-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Table: TotalRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
