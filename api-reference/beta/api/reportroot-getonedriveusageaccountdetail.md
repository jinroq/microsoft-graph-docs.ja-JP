---
title: 'reportRoot: getOneDriveUsageAccountDetail'
description: アカウント別の OneDrive の使用状況に関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0e5928b3d131a53e85f4560a98cdc00e222a5a29
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267323"
---
# <a name="reportroot-getonedriveusageaccountdetail"></a><span data-ttu-id="ad93d-103">reportRoot: getOneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="ad93d-103">reportRoot: getOneDriveUsageAccountDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad93d-104">アカウント別の OneDrive の使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="ad93d-104">Get details about OneDrive usage by account.</span></span>

> <span data-ttu-id="ad93d-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business の使用状況](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ad93d-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="ad93d-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ad93d-106">Permissions</span></span>

<span data-ttu-id="ad93d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ad93d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ad93d-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ad93d-109">Permission type</span></span>                        | <span data-ttu-id="ad93d-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ad93d-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ad93d-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="ad93d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ad93d-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad93d-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ad93d-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ad93d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad93d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad93d-114">Not supported.</span></span>                           |
| <span data-ttu-id="ad93d-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ad93d-115">Application</span></span>                            | <span data-ttu-id="ad93d-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad93d-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ad93d-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ad93d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountDetail(period='{period_value}')
GET /reports/getOneDriveUsageAccountDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="ad93d-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="ad93d-118">Function parameters</span></span>

<span data-ttu-id="ad93d-119">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="ad93d-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="ad93d-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ad93d-120">Parameter</span></span> | <span data-ttu-id="ad93d-121">型</span><span class="sxs-lookup"><span data-stu-id="ad93d-121">Type</span></span>   | <span data-ttu-id="ad93d-122">説明</span><span class="sxs-lookup"><span data-stu-id="ad93d-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ad93d-123">period</span><span class="sxs-lookup"><span data-stu-id="ad93d-123">period</span></span>    | <span data-ttu-id="ad93d-124">文字列</span><span class="sxs-lookup"><span data-stu-id="ad93d-124">string</span></span> | <span data-ttu-id="ad93d-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="ad93d-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ad93d-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="ad93d-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ad93d-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="ad93d-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="ad93d-128">date</span><span class="sxs-lookup"><span data-stu-id="ad93d-128">date</span></span>      | <span data-ttu-id="ad93d-129">日付</span><span class="sxs-lookup"><span data-stu-id="ad93d-129">Date</span></span>   | <span data-ttu-id="ad93d-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="ad93d-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="ad93d-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="ad93d-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="ad93d-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="ad93d-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="ad93d-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ad93d-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="ad93d-134">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ad93d-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="ad93d-135">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="ad93d-135">The default output type is text/csv.</span></span> <span data-ttu-id="ad93d-136">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="ad93d-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ad93d-137">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad93d-137">Request headers</span></span>

| <span data-ttu-id="ad93d-138">名前</span><span class="sxs-lookup"><span data-stu-id="ad93d-138">Name</span></span>          | <span data-ttu-id="ad93d-139">説明</span><span class="sxs-lookup"><span data-stu-id="ad93d-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ad93d-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad93d-140">Authorization</span></span> | <span data-ttu-id="ad93d-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ad93d-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ad93d-143">応答</span><span class="sxs-lookup"><span data-stu-id="ad93d-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="ad93d-144">CSV</span><span class="sxs-lookup"><span data-stu-id="ad93d-144">CSV</span></span>

<span data-ttu-id="ad93d-145">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="ad93d-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ad93d-146">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="ad93d-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ad93d-147">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="ad93d-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ad93d-148">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="ad93d-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ad93d-149">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="ad93d-149">Report Refresh Date</span></span>
- <span data-ttu-id="ad93d-150">サイトの URL</span><span class="sxs-lookup"><span data-stu-id="ad93d-150">Site URL</span></span>
- <span data-ttu-id="ad93d-151">所有者の表示名</span><span class="sxs-lookup"><span data-stu-id="ad93d-151">Owner Display Name</span></span>
- <span data-ttu-id="ad93d-152">削除済み</span><span class="sxs-lookup"><span data-stu-id="ad93d-152">Is Deleted</span></span>
- <span data-ttu-id="ad93d-153">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="ad93d-153">Last Activity Date</span></span>
- <span data-ttu-id="ad93d-154">ファイル数</span><span class="sxs-lookup"><span data-stu-id="ad93d-154">File Count</span></span>
- <span data-ttu-id="ad93d-155">アクティブなファイル数</span><span class="sxs-lookup"><span data-stu-id="ad93d-155">Active File Count</span></span>
- <span data-ttu-id="ad93d-156">使用済みストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="ad93d-156">Storage Used (Byte)</span></span>
- <span data-ttu-id="ad93d-157">割り当て済みストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="ad93d-157">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="ad93d-158">所有者のプリンシパル名</span><span class="sxs-lookup"><span data-stu-id="ad93d-158">Owner Principal Name</span></span>
- <span data-ttu-id="ad93d-159">レポート期間</span><span class="sxs-lookup"><span data-stu-id="ad93d-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="ad93d-160">JSON</span><span class="sxs-lookup"><span data-stu-id="ad93d-160">JSON</span></span>

<span data-ttu-id="ad93d-161">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[onedrive の使い方 accountdetail](../resources/onedriveusageaccountdetail.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ad93d-161">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md)** object in the response body.</span></span>

<span data-ttu-id="ad93d-162">この要求の既定のページサイズは200アイテムです。</span><span class="sxs-lookup"><span data-stu-id="ad93d-162">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="ad93d-163">例</span><span class="sxs-lookup"><span data-stu-id="ad93d-163">Example</span></span>

<span data-ttu-id="ad93d-164">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ad93d-164">The following is an example that outputs CSV.</span></span>

### <a name="csv"></a><span data-ttu-id="ad93d-165">CSV</span><span class="sxs-lookup"><span data-stu-id="ad93d-165">CSV</span></span>

#### <a name="request"></a><span data-ttu-id="ad93d-166">要求</span><span class="sxs-lookup"><span data-stu-id="ad93d-166">Request</span></span>

<span data-ttu-id="ad93d-167">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ad93d-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="ad93d-168">応答</span><span class="sxs-lookup"><span data-stu-id="ad93d-168">Response</span></span>

<span data-ttu-id="ad93d-169">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ad93d-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ad93d-170">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="ad93d-170">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ad93d-171">C#</span><span class="sxs-lookup"><span data-stu-id="ad93d-171">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveusageaccountdetail_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ad93d-172">Javascript</span><span class="sxs-lookup"><span data-stu-id="ad93d-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveusageaccountdetail_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ad93d-173">目的-C</span><span class="sxs-lookup"><span data-stu-id="ad93d-173">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveusageaccountdetail_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="ad93d-174">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="ad93d-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Storage Used (Byte),Storage Allocated (Byte),Owner Principal Name,Report Period
```

### <a name="json"></a><span data-ttu-id="ad93d-175">JSON</span><span class="sxs-lookup"><span data-stu-id="ad93d-175">JSON</span></span>

<span data-ttu-id="ad93d-176">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="ad93d-176">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="ad93d-177">要求</span><span class="sxs-lookup"><span data-stu-id="ad93d-177">Request</span></span>

<span data-ttu-id="ad93d-178">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ad93d-178">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="ad93d-179">応答</span><span class="sxs-lookup"><span data-stu-id="ad93d-179">Response</span></span>

<span data-ttu-id="ad93d-180">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ad93d-180">The following is an example of the response.</span></span>

> <span data-ttu-id="ad93d-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ad93d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveUsageAccountDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveUsageAccountDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteUrl": "siteUrl-value", 
      "ownerDisplayName": "ownerDisplayName-value", 
      "ownerPrincipalName": "ownerPrincipalName-value", 
      "isDeleted": false, 
      "lastActivityDate": "2017-09-01", 
      "fileCount": 9, 
      "activeFileCount": 5, 
      "storageUsedInBytes": 12190375, 
      "storageAllocatedInBytes": 549755813880, 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ad93d-183">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="ad93d-183">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ad93d-184">C#</span><span class="sxs-lookup"><span data-stu-id="ad93d-184">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveusageaccountdetail_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ad93d-185">Javascript</span><span class="sxs-lookup"><span data-stu-id="ad93d-185">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveusageaccountdetail_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ad93d-186">目的-C</span><span class="sxs-lookup"><span data-stu-id="ad93d-186">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveusageaccountdetail_json-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/reportroot-getonedriveusageaccountdetail.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getonedriveusageaccountdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getonedriveusageaccountdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getonedriveusageaccountdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getonedriveusageaccountdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
