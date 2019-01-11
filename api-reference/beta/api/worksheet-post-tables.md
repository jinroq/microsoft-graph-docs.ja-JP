---
title: テーブルの作成
description: この API を使用して、新しいテーブルを作成します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 7e259e8a2d8cb6e725027baca803e94288dd3060
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882825"
---
# <a name="create-table"></a><span data-ttu-id="b4499-103">テーブルの作成</span><span class="sxs-lookup"><span data-stu-id="b4499-103">Create table</span></span>

> <span data-ttu-id="b4499-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b4499-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b4499-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4499-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b4499-106">この API を使用して、新しいテーブルを作成します。</span><span class="sxs-lookup"><span data-stu-id="b4499-106">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="b4499-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b4499-107">Permissions</span></span>
<span data-ttu-id="b4499-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b4499-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4499-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b4499-110">Permission type</span></span>      | <span data-ttu-id="b4499-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b4499-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4499-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b4499-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b4499-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4499-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b4499-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b4499-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4499-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4499-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b4499-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b4499-116">Application</span></span> | <span data-ttu-id="b4499-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4499-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4499-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b4499-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="b4499-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b4499-119">Request headers</span></span>
| <span data-ttu-id="b4499-120">名前</span><span class="sxs-lookup"><span data-stu-id="b4499-120">Name</span></span>       | <span data-ttu-id="b4499-121">説明</span><span class="sxs-lookup"><span data-stu-id="b4499-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b4499-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4499-122">Authorization</span></span>  | <span data-ttu-id="b4499-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b4499-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b4499-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b4499-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="b4499-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="b4499-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4499-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="b4499-128">Request body</span></span>
<span data-ttu-id="b4499-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="b4499-129">In the request body, provide a JSON object with the following parameters.</span></span> 

| <span data-ttu-id="b4499-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b4499-130">Parameter</span></span>       | <span data-ttu-id="b4499-131">Type</span><span class="sxs-lookup"><span data-stu-id="b4499-131">Type</span></span>|<span data-ttu-id="b4499-132">説明</span><span class="sxs-lookup"><span data-stu-id="b4499-132">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="b4499-133">Address</span><span class="sxs-lookup"><span data-stu-id="b4499-133">Address</span></span>  | <span data-ttu-id="b4499-134">文字列</span><span class="sxs-lookup"><span data-stu-id="b4499-134">string</span></span>| <span data-ttu-id="b4499-p105">範囲のアドレスです。API を次から呼び出す場合: \`worksheets/{id</span><span class="sxs-lookup"><span data-stu-id="b4499-p105">Range address. If you are calling this API off of \`worksheets/{id</span></span>|<span data-ttu-id="b4499-137">name}/tables/add` path, there is no need to support the sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4\`)</span><span class="sxs-lookup"><span data-stu-id="b4499-137">name}/tables/add` path, there is no need to support the sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4\`)</span></span>|
| <span data-ttu-id="b4499-138">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="b4499-138">hasHeaders</span></span>  | <span data-ttu-id="b4499-139">boolean</span><span class="sxs-lookup"><span data-stu-id="b4499-139">boolean</span></span>|<span data-ttu-id="b4499-p106">範囲に列ラベルがあるかどうかを示すブール値。ソースにヘッダーが含まれていない場合 (このプロパティが false に設定されている場合)、Excel はデータを下方向に 1 行シフトして、自動的にヘッダーを生成します。</span><span class="sxs-lookup"><span data-stu-id="b4499-p106">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="b4499-143">応答</span><span class="sxs-lookup"><span data-stu-id="b4499-143">Response</span></span>

<span data-ttu-id="b4499-144">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[テーブル](../resources/table.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b4499-144">If successful, this method returns `201 Created` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4499-145">例</span><span class="sxs-lookup"><span data-stu-id="b4499-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b4499-146">要求</span><span class="sxs-lookup"><span data-stu-id="b4499-146">Request</span></span>
<span data-ttu-id="b4499-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b4499-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_table_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/tables/$/add
Content-type: application/json
Content-length: 109

{
  "address": "",
  "hasHeaders": false
}
```
##### <a name="response"></a><span data-ttu-id="b4499-148">応答</span><span class="sxs-lookup"><span data-stu-id="b4499-148">Response</span></span>
<span data-ttu-id="b4499-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b4499-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table"
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
