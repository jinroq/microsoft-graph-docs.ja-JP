---
title: 'Table: convertToRange'
description: テーブルを通常の範囲のセルに変換します。すべてのデータが保持されます。
author: lumine2008
ms.openlocfilehash: 7f05f21427e75ef3e86981f0ca52d1364ec86bf0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306812"
---
# <a name="table-converttorange"></a><span data-ttu-id="11f03-104">Table: convertToRange</span><span class="sxs-lookup"><span data-stu-id="11f03-104">Table: convertToRange</span></span>

> <span data-ttu-id="11f03-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="11f03-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11f03-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11f03-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="11f03-p103">テーブルを通常の範囲のセルに変換します。すべてのデータが保持されます。</span><span class="sxs-lookup"><span data-stu-id="11f03-p103">Converts the table into a normal range of cells. All data is preserved.</span></span>
## <a name="permissions"></a><span data-ttu-id="11f03-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="11f03-109">Permissions</span></span>
<span data-ttu-id="11f03-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="11f03-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11f03-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="11f03-112">Permission type</span></span>      | <span data-ttu-id="11f03-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="11f03-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11f03-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="11f03-114">Delegated (work or school account)</span></span> | <span data-ttu-id="11f03-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11f03-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="11f03-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="11f03-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11f03-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11f03-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="11f03-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="11f03-118">Application</span></span> | <span data-ttu-id="11f03-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11f03-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="11f03-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="11f03-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/convertToRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/convertToRange

```
## <a name="request-headers"></a><span data-ttu-id="11f03-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="11f03-121">Request headers</span></span>
| <span data-ttu-id="11f03-122">名前</span><span class="sxs-lookup"><span data-stu-id="11f03-122">Name</span></span>       | <span data-ttu-id="11f03-123">説明</span><span class="sxs-lookup"><span data-stu-id="11f03-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="11f03-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="11f03-124">Authorization</span></span>  | <span data-ttu-id="11f03-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="11f03-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="11f03-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="11f03-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="11f03-p106">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="11f03-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="11f03-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="11f03-130">Request body</span></span>

## <a name="response"></a><span data-ttu-id="11f03-131">応答</span><span class="sxs-lookup"><span data-stu-id="11f03-131">Response</span></span>

<span data-ttu-id="11f03-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="11f03-132">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11f03-133">例</span><span class="sxs-lookup"><span data-stu-id="11f03-133">Example</span></span>
<span data-ttu-id="11f03-134">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="11f03-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="11f03-135">要求</span><span class="sxs-lookup"><span data-stu-id="11f03-135">Request</span></span>
<span data-ttu-id="11f03-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="11f03-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_converttorange"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/convertToRange
```

##### <a name="response"></a><span data-ttu-id="11f03-137">応答</span><span class="sxs-lookup"><span data-stu-id="11f03-137">Response</span></span>
<span data-ttu-id="11f03-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="11f03-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Table: convertToRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->