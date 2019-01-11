---
title: Table:Range
description: テーブル全体に関連付けられた範囲オブジェクトを取得します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: edf42f4cbefe9572bb5c147e03489ec7317abc61
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806483"
---
# <a name="table-range"></a><span data-ttu-id="d689d-103">Table:Range</span><span class="sxs-lookup"><span data-stu-id="d689d-103">Table: Range</span></span>

> <span data-ttu-id="d689d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d689d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d689d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d689d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d689d-106">テーブル全体に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="d689d-106">Gets the range object associated with the entire table.</span></span>
## <a name="permissions"></a><span data-ttu-id="d689d-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d689d-107">Permissions</span></span>
<span data-ttu-id="d689d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d689d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d689d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d689d-110">Permission type</span></span>      | <span data-ttu-id="d689d-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d689d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d689d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d689d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d689d-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d689d-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d689d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d689d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d689d-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d689d-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d689d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d689d-116">Application</span></span> | <span data-ttu-id="d689d-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d689d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d689d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d689d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/Range
POST /workbook/worksheets/{id|name}/tables/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="d689d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d689d-119">Request headers</span></span>
| <span data-ttu-id="d689d-120">名前</span><span class="sxs-lookup"><span data-stu-id="d689d-120">Name</span></span>       | <span data-ttu-id="d689d-121">説明</span><span class="sxs-lookup"><span data-stu-id="d689d-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d689d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d689d-122">Authorization</span></span>  | <span data-ttu-id="d689d-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d689d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d689d-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d689d-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="d689d-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="d689d-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d689d-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="d689d-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="d689d-129">応答</span><span class="sxs-lookup"><span data-stu-id="d689d-129">Response</span></span>

<span data-ttu-id="d689d-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d689d-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d689d-131">例</span><span class="sxs-lookup"><span data-stu-id="d689d-131">Example</span></span>
<span data-ttu-id="d689d-132">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="d689d-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d689d-133">要求</span><span class="sxs-lookup"><span data-stu-id="d689d-133">Request</span></span>
<span data-ttu-id="d689d-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d689d-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_range"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/Range
```

##### <a name="response"></a><span data-ttu-id="d689d-135">応答</span><span class="sxs-lookup"><span data-stu-id="d689d-135">Response</span></span>
<span data-ttu-id="d689d-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d689d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Table: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
