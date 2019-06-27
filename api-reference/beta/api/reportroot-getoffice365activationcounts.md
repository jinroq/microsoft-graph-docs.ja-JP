---
title: 'reportRoot: getOffice365ActivationCounts'
description: デスクトップとデバイスでの Office 365 のライセンス認証の数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 757a7d6fe8b6fca0ee980a0ef93852fe1ab6d433
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265395"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="901ca-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="901ca-103">reportRoot: getOffice365ActivationCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="901ca-104">デスクトップとデバイスでの Office 365 のライセンス認証の数を取得します。</span><span class="sxs-lookup"><span data-stu-id="901ca-104">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="901ca-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Microsoft Office ライセンス認証](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="901ca-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="901ca-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="901ca-106">Permissions</span></span>

<span data-ttu-id="901ca-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="901ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="901ca-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="901ca-109">Permission type</span></span>                        | <span data-ttu-id="901ca-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="901ca-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="901ca-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="901ca-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="901ca-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="901ca-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="901ca-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="901ca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="901ca-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="901ca-114">Not supported.</span></span>                           |
| <span data-ttu-id="901ca-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="901ca-115">Application</span></span>                            | <span data-ttu-id="901ca-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="901ca-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="901ca-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="901ca-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="query-parameters"></a><span data-ttu-id="901ca-118">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="901ca-118">Query parameters</span></span>

<span data-ttu-id="901ca-119">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="901ca-119">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="901ca-120">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="901ca-120">The default output type is text/csv.</span></span> <span data-ttu-id="901ca-121">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="901ca-121">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="901ca-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="901ca-122">Request headers</span></span>

| <span data-ttu-id="901ca-123">名前</span><span class="sxs-lookup"><span data-stu-id="901ca-123">Name</span></span>          | <span data-ttu-id="901ca-124">説明</span><span class="sxs-lookup"><span data-stu-id="901ca-124">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="901ca-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="901ca-125">Authorization</span></span> | <span data-ttu-id="901ca-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="901ca-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="901ca-128">応答</span><span class="sxs-lookup"><span data-stu-id="901ca-128">Response</span></span>

### <a name="csv"></a><span data-ttu-id="901ca-129">CSV</span><span class="sxs-lookup"><span data-stu-id="901ca-129">CSV</span></span>

<span data-ttu-id="901ca-130">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="901ca-130">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="901ca-131">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="901ca-131">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="901ca-132">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="901ca-132">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="901ca-133">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="901ca-133">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="901ca-134">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="901ca-134">Report Refresh Date</span></span>
- <span data-ttu-id="901ca-135">製品の種類</span><span class="sxs-lookup"><span data-stu-id="901ca-135">Product Type</span></span>
- <span data-ttu-id="901ca-136">Windows</span><span class="sxs-lookup"><span data-stu-id="901ca-136">Windows</span></span>
- <span data-ttu-id="901ca-137">Mac</span><span class="sxs-lookup"><span data-stu-id="901ca-137">Mac</span></span>
- <span data-ttu-id="901ca-138">Android</span><span class="sxs-lookup"><span data-stu-id="901ca-138">Android</span></span>
- <span data-ttu-id="901ca-139">iOS</span><span class="sxs-lookup"><span data-stu-id="901ca-139">iOS</span></span>
- <span data-ttu-id="901ca-140">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="901ca-140">Windows 10 Mobile</span></span>

### <a name="json"></a><span data-ttu-id="901ca-141">JSON</span><span class="sxs-lookup"><span data-stu-id="901ca-141">JSON</span></span>

<span data-ttu-id="901ca-142">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[office365ActivationCounts](../resources/office365activationcounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="901ca-142">If successful, this method returns a `200 OK` response code and an **[office365ActivationCounts](../resources/office365activationcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="901ca-143">例</span><span class="sxs-lookup"><span data-stu-id="901ca-143">Example</span></span>

### <a name="csv"></a><span data-ttu-id="901ca-144">CSV</span><span class="sxs-lookup"><span data-stu-id="901ca-144">CSV</span></span>

<span data-ttu-id="901ca-145">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="901ca-145">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="901ca-146">要求</span><span class="sxs-lookup"><span data-stu-id="901ca-146">Request</span></span>

<span data-ttu-id="901ca-147">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="901ca-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="901ca-148">応答</span><span class="sxs-lookup"><span data-stu-id="901ca-148">Response</span></span>

<span data-ttu-id="901ca-149">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="901ca-149">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="901ca-150">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="901ca-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="901ca-151">C#</span><span class="sxs-lookup"><span data-stu-id="901ca-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationcounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="901ca-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="901ca-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationcounts_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="901ca-153">目的-C</span><span class="sxs-lookup"><span data-stu-id="901ca-153">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationcounts_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="901ca-154">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="901ca-154">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Windows,Mac,Android,iOS,Windows 10 Mobile
```

### <a name="json"></a><span data-ttu-id="901ca-155">JSON</span><span class="sxs-lookup"><span data-stu-id="901ca-155">JSON</span></span>

<span data-ttu-id="901ca-156">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="901ca-156">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="901ca-157">要求</span><span class="sxs-lookup"><span data-stu-id="901ca-157">Request</span></span>

<span data-ttu-id="901ca-158">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="901ca-158">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="901ca-159">応答</span><span class="sxs-lookup"><span data-stu-id="901ca-159">Response</span></span>

<span data-ttu-id="901ca-160">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="901ca-160">The following example shows the response.</span></span>

> <span data-ttu-id="901ca-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="901ca-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActivationCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 268

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActivationCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "productType": "Office 365 ProPlus", 
      "windows": 9157, 
      "mac": 576, 
      "android": 358, 
      "ios": 1452, 
      "windows10Mobile": 2309
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="901ca-163">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="901ca-163">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="901ca-164">C#</span><span class="sxs-lookup"><span data-stu-id="901ca-164">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationcounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="901ca-165">Javascript</span><span class="sxs-lookup"><span data-stu-id="901ca-165">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationcounts_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="901ca-166">目的-C</span><span class="sxs-lookup"><span data-stu-id="901ca-166">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationcounts_json-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365activationcounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getoffice365activationcounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getoffice365activationcounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getoffice365activationcounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getoffice365activationcounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
