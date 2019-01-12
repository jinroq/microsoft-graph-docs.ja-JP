---
title: 'TableColumnCollection: 追加'
description: テーブルに新しい列を追加します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f28b39b4ff0f7eee96be09b26bd12434a751a604
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940485"
---
# <a name="tablecolumncollection-add"></a><span data-ttu-id="ea410-103">TableColumnCollection: 追加</span><span class="sxs-lookup"><span data-stu-id="ea410-103">TableColumnCollection: add</span></span>

<span data-ttu-id="ea410-104">テーブルに新しい列を追加します。</span><span class="sxs-lookup"><span data-stu-id="ea410-104">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="ea410-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ea410-105">Permissions</span></span>
<span data-ttu-id="ea410-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ea410-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea410-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ea410-108">Permission type</span></span>      | <span data-ttu-id="ea410-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ea410-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea410-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ea410-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ea410-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea410-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ea410-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ea410-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea410-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ea410-113">Not supported.</span></span>    |
|<span data-ttu-id="ea410-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ea410-114">Application</span></span> | <span data-ttu-id="ea410-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ea410-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea410-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ea410-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="ea410-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ea410-117">Request headers</span></span>
| <span data-ttu-id="ea410-118">名前</span><span class="sxs-lookup"><span data-stu-id="ea410-118">Name</span></span>       | <span data-ttu-id="ea410-119">説明</span><span class="sxs-lookup"><span data-stu-id="ea410-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ea410-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea410-120">Authorization</span></span>  | <span data-ttu-id="ea410-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ea410-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ea410-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ea410-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="ea410-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="ea410-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea410-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ea410-126">Request body</span></span>
<span data-ttu-id="ea410-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="ea410-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ea410-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ea410-128">Parameter</span></span>    | <span data-ttu-id="ea410-129">Type</span><span class="sxs-lookup"><span data-stu-id="ea410-129">Type</span></span>   |<span data-ttu-id="ea410-130">説明</span><span class="sxs-lookup"><span data-stu-id="ea410-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea410-131">index</span><span class="sxs-lookup"><span data-stu-id="ea410-131">index</span></span>|<span data-ttu-id="ea410-132">Int32</span><span class="sxs-lookup"><span data-stu-id="ea410-132">Int32</span></span>|<span data-ttu-id="ea410-p104">新しい列の相対位置を指定します。この位置の前の列は右にシフトされます。インデックス値は、最後の列のインデックス値と等しいか、小さくなります。そのため、テーブルの末尾に列を追加するためには使用できません。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="ea410-p104">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="ea410-137">values</span><span class="sxs-lookup"><span data-stu-id="ea410-137">values</span></span>|<span data-ttu-id="ea410-138">Json</span><span class="sxs-lookup"><span data-stu-id="ea410-138">Json</span></span>|<span data-ttu-id="ea410-p105">省略可能。テーブルの列の、書式設定されていない値の 2 次元の配列。</span><span class="sxs-lookup"><span data-stu-id="ea410-p105">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|
|<span data-ttu-id="ea410-141">name</span><span class="sxs-lookup"><span data-stu-id="ea410-141">name</span></span>|<span data-ttu-id="ea410-142">文字列</span><span class="sxs-lookup"><span data-stu-id="ea410-142">string</span></span>|<span data-ttu-id="ea410-143">名前</span><span class="sxs-lookup"><span data-stu-id="ea410-143">name</span></span>
## <a name="response"></a><span data-ttu-id="ea410-144">応答</span><span class="sxs-lookup"><span data-stu-id="ea410-144">Response</span></span>

<span data-ttu-id="ea410-145">かどうかは成功すると、このメソッドを返します`200 OK`応答コードおよび応答の本文に[WorkbookTableColumn](../resources/tablecolumn.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="ea410-145">If successful, this method returns `200 OK` response code and [WorkbookTableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea410-146">例</span><span class="sxs-lookup"><span data-stu-id="ea410-146">Example</span></span>
<span data-ttu-id="ea410-147">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="ea410-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ea410-148">要求</span><span class="sxs-lookup"><span data-stu-id="ea410-148">Request</span></span>
<span data-ttu-id="ea410-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ea410-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumncollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/add
Content-type: application/json
Content-length: 51

{
  "index": 3,
  "values": [
    {
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="ea410-150">応答</span><span class="sxs-lookup"><span data-stu-id="ea410-150">Response</span></span>
<span data-ttu-id="ea410-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ea410-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumnCollection: add",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/api/tablecolumncollection-add.md/tablecolumncollection_add/values:
      Inconsistent types between parameter (Object) and table (None)",
    "Error: /api-reference/v1.0/api/tablecolumncollection-add.md/tablecolumncollection_add/values:
      Type mismatch between example and table. Parameter name: values; example type (Collection(Object)) is a collection, while the table description type (microsoft.graph.Json) is not."
  ],
  "tocPath": ""
}-->
