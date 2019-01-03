---
title: テーブルの作成
description: この API を使用して、新しいテーブルを作成します。
author: lumine2008
ms.openlocfilehash: 75d4199b4c5cefcb17acccfedfb5c45a3f296de0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321624"
---
# <a name="create-table"></a><span data-ttu-id="74496-103">テーブルの作成</span><span class="sxs-lookup"><span data-stu-id="74496-103">Create table</span></span>

> <span data-ttu-id="74496-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="74496-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74496-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74496-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="74496-106">この API を使用して、新しいテーブルを作成します。</span><span class="sxs-lookup"><span data-stu-id="74496-106">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="74496-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="74496-107">Permissions</span></span>
<span data-ttu-id="74496-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="74496-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74496-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="74496-110">Permission type</span></span>      | <span data-ttu-id="74496-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="74496-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74496-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="74496-112">Delegated (work or school account)</span></span> | <span data-ttu-id="74496-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74496-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="74496-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="74496-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74496-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74496-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="74496-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="74496-116">Application</span></span> | <span data-ttu-id="74496-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74496-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="74496-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="74496-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/$/add

```
## <a name="request-headers"></a><span data-ttu-id="74496-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="74496-119">Request headers</span></span>
| <span data-ttu-id="74496-120">名前</span><span class="sxs-lookup"><span data-stu-id="74496-120">Name</span></span>       | <span data-ttu-id="74496-121">説明</span><span class="sxs-lookup"><span data-stu-id="74496-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="74496-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="74496-122">Authorization</span></span>  | <span data-ttu-id="74496-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="74496-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="74496-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="74496-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="74496-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="74496-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="74496-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="74496-128">Request body</span></span>
<span data-ttu-id="74496-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="74496-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="74496-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="74496-130">Parameter</span></span>           | <span data-ttu-id="74496-131">種類</span><span class="sxs-lookup"><span data-stu-id="74496-131">Type</span></span>      |<span data-ttu-id="74496-132">説明</span><span class="sxs-lookup"><span data-stu-id="74496-132">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="74496-133">Address</span><span class="sxs-lookup"><span data-stu-id="74496-133">Address</span></span>  | <span data-ttu-id="74496-134">string</span><span class="sxs-lookup"><span data-stu-id="74496-134">string</span></span>| <span data-ttu-id="74496-p105">範囲のアドレスです。この API を `worksheets/{id or name}/tables/add` パスから呼び出す場合、アドレスにシート名のプレフィックスを指定する必要はありません。ただし、これを `workbook/tables/add` パスから呼び出す場合は、テーブルを作成する必要のあるシート名を指定する必要があります (例: `sheet1!A1:D4`)。</span><span class="sxs-lookup"><span data-stu-id="74496-p105">Range address. If you are calling this API off of `worksheets/{id or name}/tables/add` path, there is no need to for sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="74496-138">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="74496-138">hasHeaders</span></span>  | <span data-ttu-id="74496-139">boolean</span><span class="sxs-lookup"><span data-stu-id="74496-139">boolean</span></span>|<span data-ttu-id="74496-p106">範囲に列ラベルがあるかどうかを示すブール値。ソースにヘッダーが含まれていない場合 (このプロパティが false に設定されている場合)、Excel はデータを下方向に 1 行シフトして、自動的にヘッダーを生成します。</span><span class="sxs-lookup"><span data-stu-id="74496-p106">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="74496-143">応答</span><span class="sxs-lookup"><span data-stu-id="74496-143">Response</span></span>

<span data-ttu-id="74496-144">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[テーブル](../resources/table.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="74496-144">If successful, this method returns `201 Created` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74496-145">例</span><span class="sxs-lookup"><span data-stu-id="74496-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="74496-146">要求</span><span class="sxs-lookup"><span data-stu-id="74496-146">Request</span></span>
<span data-ttu-id="74496-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="74496-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_table_from_workbook"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/$/add
Content-type: application/json
Content-length: 109

{
  "address": "A1:D8",
  "hasHeaders": false
}
```
##### <a name="response"></a><span data-ttu-id="74496-148">応答</span><span class="sxs-lookup"><span data-stu-id="74496-148">Response</span></span>
<span data-ttu-id="74496-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="74496-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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