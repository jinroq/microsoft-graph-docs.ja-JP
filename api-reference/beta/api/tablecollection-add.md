---
title: 'TableCollection: 追加'
description: 新しいテーブルを作成します。範囲のソース アドレスにより、テーブルが追加されるワークシートが判断されます。テーブルが追加できない場合 (たとえば、アドレスが無効な場合や、テーブルが別のテーブルと重複している場合) は、エラーがスローされます。
localization_priority: Normal
ms.openlocfilehash: 8053ce8e8d0ac62e096fa70255064e82a03630f6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868447"
---
# <a name="tablecollection-add"></a><span data-ttu-id="1104a-105">TableCollection: 追加</span><span class="sxs-lookup"><span data-stu-id="1104a-105">TableCollection: add</span></span>

> <span data-ttu-id="1104a-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1104a-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1104a-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1104a-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1104a-p103">新しいテーブルを作成します。範囲のソース アドレスにより、テーブルが追加されるワークシートが判断されます。テーブルが追加できない場合 (たとえば、アドレスが無効な場合や、テーブルが別のテーブルと重複している場合) は、エラーがスローされます。</span><span class="sxs-lookup"><span data-stu-id="1104a-p103">Create a new table. The range source address determines the worksheet under which the table will be added. If the table cannot be added (e.g., because the address is invalid, or the table would overlap with another table), an error will be thrown.</span></span>

## <a name="error-handling"></a><span data-ttu-id="1104a-111">エラー処理</span><span class="sxs-lookup"><span data-stu-id="1104a-111">Error Handling</span></span>

<span data-ttu-id="1104a-112">この要求に対して、504 HTTP エラーが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1104a-112">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="1104a-113">このエラーに対する適切な対応は、要求を繰り返すことです。</span><span class="sxs-lookup"><span data-stu-id="1104a-113">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="1104a-114">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1104a-114">Permissions</span></span>
<span data-ttu-id="1104a-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1104a-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1104a-117">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1104a-117">Permission type</span></span>      | <span data-ttu-id="1104a-118">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1104a-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1104a-119">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1104a-119">Delegated (work or school account)</span></span> | <span data-ttu-id="1104a-120">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1104a-120">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1104a-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1104a-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1104a-122">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1104a-122">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1104a-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1104a-123">Application</span></span> | <span data-ttu-id="1104a-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1104a-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1104a-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1104a-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/add
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="1104a-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1104a-126">Request headers</span></span>
| <span data-ttu-id="1104a-127">名前</span><span class="sxs-lookup"><span data-stu-id="1104a-127">Name</span></span>       | <span data-ttu-id="1104a-128">説明</span><span class="sxs-lookup"><span data-stu-id="1104a-128">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1104a-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="1104a-129">Authorization</span></span>  | <span data-ttu-id="1104a-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1104a-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1104a-132">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1104a-132">Workbook-Session-Id</span></span>  | <span data-ttu-id="1104a-p107">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="1104a-p107">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1104a-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="1104a-135">Request body</span></span>
<span data-ttu-id="1104a-136">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="1104a-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1104a-137">パラメーター</span><span class="sxs-lookup"><span data-stu-id="1104a-137">Parameter</span></span>    | <span data-ttu-id="1104a-138">Type</span><span class="sxs-lookup"><span data-stu-id="1104a-138">Type</span></span>   |<span data-ttu-id="1104a-139">説明</span><span class="sxs-lookup"><span data-stu-id="1104a-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1104a-140">address</span><span class="sxs-lookup"><span data-stu-id="1104a-140">address</span></span>|<span data-ttu-id="1104a-141">文字列</span><span class="sxs-lookup"><span data-stu-id="1104a-141">string</span></span>|<span data-ttu-id="1104a-p108">データ ソースを表す Range オブジェクトのアドレスまたは名前。アドレスにシート名が含まれていない場合は、現在作業中のシートが使用されます。</span><span class="sxs-lookup"><span data-stu-id="1104a-p108">Address or name of the range object representing the data source. If the address does not contain a sheet name, the currently-active sheet is used.</span></span>|
|<span data-ttu-id="1104a-144">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="1104a-144">hasHeaders</span></span>|<span data-ttu-id="1104a-145">ブール値</span><span class="sxs-lookup"><span data-stu-id="1104a-145">boolean</span></span>|<span data-ttu-id="1104a-p109">インポートされたデータに列ラベルがあるかどうかを示すブール値。ソースにヘッダーが含まれていない場合 (このプロパティが false に設定されている場合)、Excel はデータを下方向に 1 行シフトして、自動的にヘッダーを生成します。</span><span class="sxs-lookup"><span data-stu-id="1104a-p109">Boolean value that indicates whether the data being imported has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="1104a-149">応答</span><span class="sxs-lookup"><span data-stu-id="1104a-149">Response</span></span>

<span data-ttu-id="1104a-150">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[テーブル](../resources/table.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1104a-150">If successful, this method returns `200 OK` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1104a-151">例</span><span class="sxs-lookup"><span data-stu-id="1104a-151">Example</span></span>
<span data-ttu-id="1104a-152">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="1104a-152">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1104a-153">要求</span><span class="sxs-lookup"><span data-stu-id="1104a-153">Request</span></span>
<span data-ttu-id="1104a-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1104a-154">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/add
Content-type: application/json
Content-length: 54

{
  "address": "Sheet1!A1:D5",
  "hasHeaders": true
}
```

##### <a name="response"></a><span data-ttu-id="1104a-155">応答</span><span class="sxs-lookup"><span data-stu-id="1104a-155">Response</span></span>
<span data-ttu-id="1104a-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1104a-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "TableCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
