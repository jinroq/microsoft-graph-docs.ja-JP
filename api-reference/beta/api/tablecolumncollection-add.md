---
title: 'TableColumnCollection: 追加'
description: テーブルに新しい列を追加します。
ms.openlocfilehash: 64b6fd2c91642c3f7dd6f5d3e6aaa89b526a28a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073599"
---
# <a name="tablecolumncollection-add"></a><span data-ttu-id="7733b-103">TableColumnCollection: 追加</span><span class="sxs-lookup"><span data-stu-id="7733b-103">TableColumnCollection: add</span></span>

> <span data-ttu-id="7733b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7733b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7733b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7733b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7733b-106">テーブルに新しい列を追加します。</span><span class="sxs-lookup"><span data-stu-id="7733b-106">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="7733b-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7733b-107">Permissions</span></span>
<span data-ttu-id="7733b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7733b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7733b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7733b-110">Permission type</span></span>      | <span data-ttu-id="7733b-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7733b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7733b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7733b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7733b-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7733b-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7733b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7733b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7733b-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7733b-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7733b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7733b-116">Application</span></span> | <span data-ttu-id="7733b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7733b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7733b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7733b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="7733b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7733b-119">Request headers</span></span>
| <span data-ttu-id="7733b-120">名前</span><span class="sxs-lookup"><span data-stu-id="7733b-120">Name</span></span>       | <span data-ttu-id="7733b-121">説明</span><span class="sxs-lookup"><span data-stu-id="7733b-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7733b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7733b-122">Authorization</span></span>  | <span data-ttu-id="7733b-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7733b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7733b-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7733b-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="7733b-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="7733b-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7733b-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="7733b-128">Request body</span></span>
<span data-ttu-id="7733b-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="7733b-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7733b-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="7733b-130">Parameter</span></span>    | <span data-ttu-id="7733b-131">型</span><span class="sxs-lookup"><span data-stu-id="7733b-131">Type</span></span>   |<span data-ttu-id="7733b-132">説明</span><span class="sxs-lookup"><span data-stu-id="7733b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7733b-133">index</span><span class="sxs-lookup"><span data-stu-id="7733b-133">index</span></span>|<span data-ttu-id="7733b-134">数値</span><span class="sxs-lookup"><span data-stu-id="7733b-134">number</span></span>|<span data-ttu-id="7733b-p105">新しい列の相対位置を指定します。この位置の前の列は右にシフトされます。インデックス値は、最後の列のインデックス値と等しいか、小さくなります。そのため、テーブルの末尾に列を追加するためには使用できません。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="7733b-p105">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="7733b-139">values</span><span class="sxs-lookup"><span data-stu-id="7733b-139">values</span></span>|<span data-ttu-id="7733b-140">(boolean、string、または number)</span><span class="sxs-lookup"><span data-stu-id="7733b-140">(boolean or string or number)</span></span>|<span data-ttu-id="7733b-p106">省略可能。テーブルの列の、書式設定されていない値の 2 次元の配列。</span><span class="sxs-lookup"><span data-stu-id="7733b-p106">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|

## <a name="response"></a><span data-ttu-id="7733b-143">応答</span><span class="sxs-lookup"><span data-stu-id="7733b-143">Response</span></span>

<span data-ttu-id="7733b-144">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [TableColumn](../resources/tablecolumn.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7733b-144">If successful, this method returns `200 OK` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7733b-145">例</span><span class="sxs-lookup"><span data-stu-id="7733b-145">Example</span></span>
<span data-ttu-id="7733b-146">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="7733b-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7733b-147">要求</span><span class="sxs-lookup"><span data-stu-id="7733b-147">Request</span></span>
<span data-ttu-id="7733b-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7733b-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumncollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/add
Content-type: application/json
Content-length: 51

{
  "index": {
  },
  "values": [
    {
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="7733b-149">応答</span><span class="sxs-lookup"><span data-stu-id="7733b-149">Response</span></span>
<span data-ttu-id="7733b-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7733b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
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
  "tocPath": ""
}-->