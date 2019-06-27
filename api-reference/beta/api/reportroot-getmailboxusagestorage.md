---
title: 'reportRoot: getMailboxUsageStorage'
description: 組織で使用されているストレージの量を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 85243c1a924351b010a5e13c6e1235d0440a139e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267397"
---
# <a name="reportroot-getmailboxusagestorage"></a><span data-ttu-id="42056-103">reportRoot: getMailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="42056-103">reportRoot: getMailboxUsageStorage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42056-104">組織で使用されているストレージの量を取得します。</span><span class="sxs-lookup"><span data-stu-id="42056-104">Get the amount of storage used in your organization.</span></span>

> <span data-ttu-id="42056-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メールボックスの使用状況](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="42056-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="42056-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="42056-106">Permissions</span></span>

<span data-ttu-id="42056-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="42056-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="42056-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="42056-109">Permission type</span></span>                        | <span data-ttu-id="42056-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="42056-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="42056-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="42056-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="42056-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="42056-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="42056-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="42056-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42056-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="42056-114">Not supported.</span></span>                           |
| <span data-ttu-id="42056-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="42056-115">Application</span></span>                            | <span data-ttu-id="42056-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="42056-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="42056-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="42056-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="42056-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="42056-118">Function parameters</span></span>

<span data-ttu-id="42056-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="42056-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="42056-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="42056-120">Parameter</span></span> | <span data-ttu-id="42056-121">型</span><span class="sxs-lookup"><span data-stu-id="42056-121">Type</span></span>   | <span data-ttu-id="42056-122">説明</span><span class="sxs-lookup"><span data-stu-id="42056-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="42056-123">period</span><span class="sxs-lookup"><span data-stu-id="42056-123">period</span></span>    | <span data-ttu-id="42056-124">文字列</span><span class="sxs-lookup"><span data-stu-id="42056-124">string</span></span> | <span data-ttu-id="42056-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="42056-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="42056-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="42056-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="42056-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="42056-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="42056-128">必須。</span><span class="sxs-lookup"><span data-stu-id="42056-128">Required.</span></span> |

<span data-ttu-id="42056-129">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="42056-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="42056-130">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="42056-130">The default output type is text/csv.</span></span> <span data-ttu-id="42056-131">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="42056-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="42056-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="42056-132">Request headers</span></span>

| <span data-ttu-id="42056-133">名前</span><span class="sxs-lookup"><span data-stu-id="42056-133">Name</span></span>          | <span data-ttu-id="42056-134">説明</span><span class="sxs-lookup"><span data-stu-id="42056-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="42056-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="42056-135">Authorization</span></span> | <span data-ttu-id="42056-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="42056-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="42056-138">応答</span><span class="sxs-lookup"><span data-stu-id="42056-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="42056-139">CSV</span><span class="sxs-lookup"><span data-stu-id="42056-139">CSV</span></span>

<span data-ttu-id="42056-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="42056-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="42056-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="42056-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="42056-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="42056-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="42056-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="42056-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="42056-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="42056-144">Report Refresh Date</span></span>
- <span data-ttu-id="42056-145">使用済みストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="42056-145">Storage Used (Byte)</span></span>
- <span data-ttu-id="42056-146">レポート日付</span><span class="sxs-lookup"><span data-stu-id="42056-146">Report Date</span></span>
- <span data-ttu-id="42056-147">レポート期間</span><span class="sxs-lookup"><span data-stu-id="42056-147">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="42056-148">JSON</span><span class="sxs-lookup"><span data-stu-id="42056-148">JSON</span></span>

<span data-ttu-id="42056-149">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[mailboxUsageStorage](../resources/mailboxusagestorage.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="42056-149">If successful, this method returns a `200 OK` response code and a **[mailboxUsageStorage](../resources/mailboxusagestorage.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42056-150">例</span><span class="sxs-lookup"><span data-stu-id="42056-150">Example</span></span>

### <a name="csv"></a><span data-ttu-id="42056-151">CSV</span><span class="sxs-lookup"><span data-stu-id="42056-151">CSV</span></span>

<span data-ttu-id="42056-152">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="42056-152">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="42056-153">要求</span><span class="sxs-lookup"><span data-stu-id="42056-153">Request</span></span>

<span data-ttu-id="42056-154">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="42056-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagestorage_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageStorage(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="42056-155">応答</span><span class="sxs-lookup"><span data-stu-id="42056-155">Response</span></span>

<span data-ttu-id="42056-156">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="42056-156">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="42056-157">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="42056-157">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="42056-158">C#</span><span class="sxs-lookup"><span data-stu-id="42056-158">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusagestorage_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="42056-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="42056-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusagestorage_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="42056-160">目的-C</span><span class="sxs-lookup"><span data-stu-id="42056-160">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusagestorage_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="42056-161">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="42056-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Storage Used (Byte),Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="42056-162">JSON</span><span class="sxs-lookup"><span data-stu-id="42056-162">JSON</span></span>

<span data-ttu-id="42056-163">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="42056-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="42056-164">要求</span><span class="sxs-lookup"><span data-stu-id="42056-164">Request</span></span>

<span data-ttu-id="42056-165">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="42056-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagestorage_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageStorage(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="42056-166">応答</span><span class="sxs-lookup"><span data-stu-id="42056-166">Response</span></span>

<span data-ttu-id="42056-167">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="42056-167">The following is an example of the response.</span></span>

> <span data-ttu-id="42056-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="42056-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxUsageStorage"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 235

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.mailboxUsageStorage)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "storageUsedInBytes": 5159432679270, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="42056-170">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="42056-170">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="42056-171">C#</span><span class="sxs-lookup"><span data-stu-id="42056-171">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusagestorage_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="42056-172">Javascript</span><span class="sxs-lookup"><span data-stu-id="42056-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusagestorage_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="42056-173">目的-C</span><span class="sxs-lookup"><span data-stu-id="42056-173">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusagestorage_json-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/reportroot-getmailboxusagestorage.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getmailboxusagestorage.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getmailboxusagestorage.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getmailboxusagestorage.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getmailboxusagestorage.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
