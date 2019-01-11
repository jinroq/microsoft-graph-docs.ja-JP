---
title: テーブルの作成
description: この API を使用して、新しいテーブルを作成します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 893ca43eb27069e8a9d333143ad3620b43e591a4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894405"
---
# <a name="create-table"></a><span data-ttu-id="127a5-103">テーブルの作成</span><span class="sxs-lookup"><span data-stu-id="127a5-103">Create table</span></span>

<span data-ttu-id="127a5-104">この API を使用して、新しいテーブルを作成します。</span><span class="sxs-lookup"><span data-stu-id="127a5-104">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="127a5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="127a5-105">Permissions</span></span>
<span data-ttu-id="127a5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="127a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="127a5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="127a5-108">Permission type</span></span>      | <span data-ttu-id="127a5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="127a5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="127a5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="127a5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="127a5-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="127a5-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="127a5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="127a5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="127a5-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="127a5-113">Not supported.</span></span>    |
|<span data-ttu-id="127a5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="127a5-114">Application</span></span> | <span data-ttu-id="127a5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="127a5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="127a5-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="127a5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="127a5-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="127a5-117">Request headers</span></span>
| <span data-ttu-id="127a5-118">名前</span><span class="sxs-lookup"><span data-stu-id="127a5-118">Name</span></span>       | <span data-ttu-id="127a5-119">説明</span><span class="sxs-lookup"><span data-stu-id="127a5-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="127a5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="127a5-120">Authorization</span></span>  | <span data-ttu-id="127a5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="127a5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="127a5-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="127a5-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="127a5-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="127a5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="127a5-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="127a5-126">Request body</span></span>
<span data-ttu-id="127a5-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="127a5-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="127a5-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="127a5-128">Parameter</span></span>           | <span data-ttu-id="127a5-129">Type</span><span class="sxs-lookup"><span data-stu-id="127a5-129">Type</span></span>      |<span data-ttu-id="127a5-130">説明</span><span class="sxs-lookup"><span data-stu-id="127a5-130">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="127a5-131">Address</span><span class="sxs-lookup"><span data-stu-id="127a5-131">Address</span></span>  | <span data-ttu-id="127a5-132">文字列</span><span class="sxs-lookup"><span data-stu-id="127a5-132">string</span></span>| <span data-ttu-id="127a5-p104">範囲のアドレスです。この API を `worksheets/{id or name}/tables/add` パスから呼び出す場合、アドレスにシート名のプレフィックスを指定する必要はありません。ただし、これを `workbook/tables/add` パスから呼び出す場合は、テーブルを作成する必要のあるシート名を指定する必要があります (例: `sheet1!A1:D4`)。</span><span class="sxs-lookup"><span data-stu-id="127a5-p104">Range address. If you are calling this API off of `worksheets/{id or name}/tables/add` path, there is no need to for sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="127a5-136">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="127a5-136">hasHeaders</span></span>  | <span data-ttu-id="127a5-137">boolean</span><span class="sxs-lookup"><span data-stu-id="127a5-137">boolean</span></span>|<span data-ttu-id="127a5-p105">範囲に列ラベルがあるかどうかを示すブール値。ソースにヘッダーが含まれていない場合 (このプロパティが false に設定されている場合)、Excel はデータを下方向に 1 行シフトして、自動的にヘッダーを生成します。</span><span class="sxs-lookup"><span data-stu-id="127a5-p105">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="127a5-141">応答</span><span class="sxs-lookup"><span data-stu-id="127a5-141">Response</span></span>

<span data-ttu-id="127a5-142">かどうかは成功すると、このメソッドを返します`201 Created`応答コードおよび応答の本文に[WorkbookTable](../resources/table.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="127a5-142">If successful, this method returns `201 Created` response code and [WorkbookTable](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="127a5-143">例</span><span class="sxs-lookup"><span data-stu-id="127a5-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="127a5-144">要求</span><span class="sxs-lookup"><span data-stu-id="127a5-144">Request</span></span>
<span data-ttu-id="127a5-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="127a5-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_table_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id}/add
Content-type: application/json
Content-length: 109

{
  "address": "A1:D8",
  "hasHeaders": false
}
```
##### <a name="response"></a><span data-ttu-id="127a5-146">応答</span><span class="sxs-lookup"><span data-stu-id="127a5-146">Response</span></span>
<span data-ttu-id="127a5-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="127a5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
