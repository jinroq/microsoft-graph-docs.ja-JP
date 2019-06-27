---
title: 'TableCollection: 追加'
description: 新しいテーブルを作成します。範囲のソース アドレスにより、テーブルが追加されるワークシートが判断されます。テーブルが追加できない場合 (たとえば、アドレスが無効な場合や、テーブルが別のテーブルと重複している場合) は、エラーがスローされます。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: f5c078c90133490e216756b23643751b65cac934
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278885"
---
# <a name="tablecollection-add"></a><span data-ttu-id="b16c3-105">TableCollection: 追加</span><span class="sxs-lookup"><span data-stu-id="b16c3-105">TableCollection: add</span></span>

<span data-ttu-id="b16c3-p102">新しいテーブルを作成します。範囲のソース アドレスにより、テーブルが追加されるワークシートが判断されます。テーブルが追加できない場合 (たとえば、アドレスが無効な場合や、テーブルが別のテーブルと重複している場合) は、エラーがスローされます。</span><span class="sxs-lookup"><span data-stu-id="b16c3-p102">Create a new table. The range source address determines the worksheet under which the table will be added. If the table cannot be added (e.g., because the address is invalid, or the table would overlap with another table), an error will be thrown.</span></span>

## <a name="error-handling"></a><span data-ttu-id="b16c3-109">エラー処理</span><span class="sxs-lookup"><span data-stu-id="b16c3-109">Error Handling</span></span>

<span data-ttu-id="b16c3-110">この要求に対して、504 HTTP エラーが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b16c3-110">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="b16c3-111">このエラーに対する適切な対応は、要求を繰り返すことです。</span><span class="sxs-lookup"><span data-stu-id="b16c3-111">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="b16c3-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b16c3-112">Permissions</span></span>
<span data-ttu-id="b16c3-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b16c3-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b16c3-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b16c3-115">Permission type</span></span>      | <span data-ttu-id="b16c3-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b16c3-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b16c3-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b16c3-117">Delegated (work or school account)</span></span> | <span data-ttu-id="b16c3-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b16c3-118">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b16c3-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b16c3-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b16c3-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b16c3-120">Not supported.</span></span>    |
|<span data-ttu-id="b16c3-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b16c3-121">Application</span></span> | <span data-ttu-id="b16c3-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b16c3-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b16c3-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b16c3-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/add
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="b16c3-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b16c3-124">Request headers</span></span>
| <span data-ttu-id="b16c3-125">名前</span><span class="sxs-lookup"><span data-stu-id="b16c3-125">Name</span></span>       | <span data-ttu-id="b16c3-126">説明</span><span class="sxs-lookup"><span data-stu-id="b16c3-126">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b16c3-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b16c3-127">Authorization</span></span>  | <span data-ttu-id="b16c3-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b16c3-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b16c3-130">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b16c3-130">Workbook-Session-Id</span></span>  | <span data-ttu-id="b16c3-p106">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="b16c3-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b16c3-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="b16c3-133">Request body</span></span>
<span data-ttu-id="b16c3-134">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="b16c3-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b16c3-135">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b16c3-135">Parameter</span></span>    | <span data-ttu-id="b16c3-136">型</span><span class="sxs-lookup"><span data-stu-id="b16c3-136">Type</span></span>   |<span data-ttu-id="b16c3-137">説明</span><span class="sxs-lookup"><span data-stu-id="b16c3-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b16c3-138">address</span><span class="sxs-lookup"><span data-stu-id="b16c3-138">address</span></span>|<span data-ttu-id="b16c3-139">string</span><span class="sxs-lookup"><span data-stu-id="b16c3-139">string</span></span>|<span data-ttu-id="b16c3-p107">データ ソースを表す Range オブジェクトのアドレスまたは名前。アドレスにシート名が含まれていない場合は、現在作業中のシートが使用されます。</span><span class="sxs-lookup"><span data-stu-id="b16c3-p107">Address or name of the range object representing the data source. If the address does not contain a sheet name, the currently-active sheet is used.</span></span>|
|<span data-ttu-id="b16c3-142">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="b16c3-142">hasHeaders</span></span>|<span data-ttu-id="b16c3-143">ブール値</span><span class="sxs-lookup"><span data-stu-id="b16c3-143">boolean</span></span>|<span data-ttu-id="b16c3-p108">インポートされたデータに列ラベルがあるかどうかを示すブール値。ソースにヘッダーが含まれていない場合 (このプロパティが false に設定されている場合)、Excel はデータを下方向に 1 行シフトして、自動的にヘッダーを生成します。</span><span class="sxs-lookup"><span data-stu-id="b16c3-p108">Boolean value that indicates whether the data being imported has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="b16c3-147">応答</span><span class="sxs-lookup"><span data-stu-id="b16c3-147">Response</span></span>

<span data-ttu-id="b16c3-148">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[WorkbookTable](../resources/table.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b16c3-148">If successful, this method returns `200 OK` response code and [WorkbookTable](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b16c3-149">例</span><span class="sxs-lookup"><span data-stu-id="b16c3-149">Example</span></span>
<span data-ttu-id="b16c3-150">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="b16c3-150">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b16c3-151">要求</span><span class="sxs-lookup"><span data-stu-id="b16c3-151">Request</span></span>
<span data-ttu-id="b16c3-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b16c3-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/add
Content-type: application/json
Content-length: 54

{
  "address": "Sheet1!A1:D5",
  "hasHeaders": true
}
```

##### <a name="response"></a><span data-ttu-id="b16c3-153">応答</span><span class="sxs-lookup"><span data-stu-id="b16c3-153">Response</span></span>
<span data-ttu-id="b16c3-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b16c3-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b16c3-157">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="b16c3-157">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b16c3-158">C#</span><span class="sxs-lookup"><span data-stu-id="b16c3-158">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/tablecollection_add-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b16c3-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="b16c3-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tablecollection_add-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b16c3-160">目的-C</span><span class="sxs-lookup"><span data-stu-id="b16c3-160">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/tablecollection_add-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/tablecollection-add.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/tablecollection-add.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/tablecollection-add.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
