---
title: 'TableColumn: HeaderRowRange'
description: 列のヘッダー行に関連付けられた範囲オブジェクトを取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e3fdd98598189ee8d0e4d685176dd3ef494d888d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32520425"
---
# <a name="tablecolumn-headerrowrange"></a><span data-ttu-id="d121c-103">TableColumn: HeaderRowRange</span><span class="sxs-lookup"><span data-stu-id="d121c-103">TableColumn: HeaderRowRange</span></span>

<span data-ttu-id="d121c-104">列のヘッダー行に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="d121c-104">Gets the range object associated with the header row of the column.</span></span>
## <a name="permissions"></a><span data-ttu-id="d121c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d121c-105">Permissions</span></span>
<span data-ttu-id="d121c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d121c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d121c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d121c-108">Permission type</span></span>      | <span data-ttu-id="d121c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d121c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d121c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d121c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d121c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d121c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d121c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d121c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d121c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d121c-113">Not supported.</span></span>    |
|<span data-ttu-id="d121c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d121c-114">Application</span></span> | <span data-ttu-id="d121c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d121c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d121c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d121c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/headerRowRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/headerRowRange

```
## <a name="request-headers"></a><span data-ttu-id="d121c-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d121c-117">Request headers</span></span>
| <span data-ttu-id="d121c-118">名前</span><span class="sxs-lookup"><span data-stu-id="d121c-118">Name</span></span>       | <span data-ttu-id="d121c-119">説明</span><span class="sxs-lookup"><span data-stu-id="d121c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d121c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d121c-120">Authorization</span></span>  | <span data-ttu-id="d121c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d121c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d121c-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d121c-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d121c-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="d121c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d121c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d121c-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="d121c-127">応答</span><span class="sxs-lookup"><span data-stu-id="d121c-127">Response</span></span>

<span data-ttu-id="d121c-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d121c-128">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d121c-129">例</span><span class="sxs-lookup"><span data-stu-id="d121c-129">Example</span></span>
<span data-ttu-id="d121c-130">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="d121c-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d121c-131">要求</span><span class="sxs-lookup"><span data-stu-id="d121c-131">Request</span></span>
<span data-ttu-id="d121c-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d121c-132">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablecolumn_headerrowrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/headerRowRange
```

##### <a name="response"></a><span data-ttu-id="d121c-133">応答</span><span class="sxs-lookup"><span data-stu-id="d121c-133">Response</span></span>
<span data-ttu-id="d121c-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d121c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableColumn: HeaderRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
