---
title: Table:HeaderRowRange
description: テーブルのヘッダー行に関連付けられた範囲オブジェクトを取得します。
author: lumine2008
ms.openlocfilehash: 82756ac13455b7e70f365d163823d0f4b148d5a8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351682"
---
# <a name="table-headerrowrange"></a><span data-ttu-id="506ed-103">Table:HeaderRowRange</span><span class="sxs-lookup"><span data-stu-id="506ed-103">Table: HeaderRowRange</span></span>

<span data-ttu-id="506ed-104">テーブルのヘッダー行に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="506ed-104">Gets the range object associated with header row of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="506ed-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="506ed-105">Permissions</span></span>
<span data-ttu-id="506ed-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="506ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="506ed-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="506ed-108">Permission type</span></span>      | <span data-ttu-id="506ed-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="506ed-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="506ed-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="506ed-110">Delegated (work or school account)</span></span> | <span data-ttu-id="506ed-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="506ed-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="506ed-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="506ed-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="506ed-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="506ed-113">Not supported.</span></span>    |
|<span data-ttu-id="506ed-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="506ed-114">Application</span></span> | <span data-ttu-id="506ed-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="506ed-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="506ed-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="506ed-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/headerRowRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/headerRowRange

```
## <a name="request-headers"></a><span data-ttu-id="506ed-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="506ed-117">Request headers</span></span>
| <span data-ttu-id="506ed-118">名前</span><span class="sxs-lookup"><span data-stu-id="506ed-118">Name</span></span>       | <span data-ttu-id="506ed-119">説明</span><span class="sxs-lookup"><span data-stu-id="506ed-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="506ed-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="506ed-120">Authorization</span></span>  | <span data-ttu-id="506ed-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="506ed-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="506ed-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="506ed-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="506ed-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="506ed-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="506ed-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="506ed-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="506ed-127">応答</span><span class="sxs-lookup"><span data-stu-id="506ed-127">Response</span></span>

<span data-ttu-id="506ed-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="506ed-128">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="506ed-129">例</span><span class="sxs-lookup"><span data-stu-id="506ed-129">Example</span></span>
<span data-ttu-id="506ed-130">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="506ed-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="506ed-131">要求</span><span class="sxs-lookup"><span data-stu-id="506ed-131">Request</span></span>
<span data-ttu-id="506ed-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="506ed-132">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "table_headerrowrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/headerRowRange
```

##### <a name="response"></a><span data-ttu-id="506ed-133">応答</span><span class="sxs-lookup"><span data-stu-id="506ed-133">Response</span></span>
<span data-ttu-id="506ed-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="506ed-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
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
  "description": "Table: HeaderRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->