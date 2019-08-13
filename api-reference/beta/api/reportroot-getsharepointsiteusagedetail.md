---
title: 'reportRoot: getSharePointSiteUsageDetail'
description: SharePoint サイトの使用状況に関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 9e10412f45ca14bbf9fe1f43d16f98a39e911379
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359705"
---
# <a name="reportroot-getsharepointsiteusagedetail"></a><span data-ttu-id="e7500-103">reportRoot: getSharePointSiteUsageDetail</span><span class="sxs-lookup"><span data-stu-id="e7500-103">reportRoot: getSharePointSiteUsageDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7500-104">SharePoint サイトの使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="e7500-104">Get details about SharePoint site usage.</span></span>

> <span data-ttu-id="e7500-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint サイトの使用状況](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7500-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="e7500-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e7500-106">Permissions</span></span>

<span data-ttu-id="e7500-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7500-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e7500-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e7500-109">Permission type</span></span>                        | <span data-ttu-id="e7500-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e7500-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e7500-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="e7500-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e7500-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7500-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e7500-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e7500-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7500-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7500-114">Not supported.</span></span>                           |
| <span data-ttu-id="e7500-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e7500-115">Application</span></span>                            | <span data-ttu-id="e7500-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7500-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e7500-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e7500-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageDetail(period='{period_value}')
GET /reports/getSharePointSiteUsageDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="e7500-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="e7500-118">Function parameters</span></span>

<span data-ttu-id="e7500-119">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="e7500-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="e7500-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e7500-120">Parameter</span></span> | <span data-ttu-id="e7500-121">型</span><span class="sxs-lookup"><span data-stu-id="e7500-121">Type</span></span>   | <span data-ttu-id="e7500-122">説明</span><span class="sxs-lookup"><span data-stu-id="e7500-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e7500-123">period</span><span class="sxs-lookup"><span data-stu-id="e7500-123">period</span></span>    | <span data-ttu-id="e7500-124">文字列</span><span class="sxs-lookup"><span data-stu-id="e7500-124">string</span></span> | <span data-ttu-id="e7500-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="e7500-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e7500-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="e7500-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e7500-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="e7500-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="e7500-128">date</span><span class="sxs-lookup"><span data-stu-id="e7500-128">date</span></span>      | <span data-ttu-id="e7500-129">日付</span><span class="sxs-lookup"><span data-stu-id="e7500-129">Date</span></span>   | <span data-ttu-id="e7500-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="e7500-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="e7500-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="e7500-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="e7500-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="e7500-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="e7500-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e7500-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="e7500-134">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e7500-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e7500-135">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="e7500-135">The default output type is text/csv.</span></span> <span data-ttu-id="e7500-136">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="e7500-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e7500-137">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7500-137">Request headers</span></span>

| <span data-ttu-id="e7500-138">名前</span><span class="sxs-lookup"><span data-stu-id="e7500-138">Name</span></span>          | <span data-ttu-id="e7500-139">説明</span><span class="sxs-lookup"><span data-stu-id="e7500-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e7500-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7500-140">Authorization</span></span> | <span data-ttu-id="e7500-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e7500-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e7500-143">応答</span><span class="sxs-lookup"><span data-stu-id="e7500-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e7500-144">CSV</span><span class="sxs-lookup"><span data-stu-id="e7500-144">CSV</span></span>

<span data-ttu-id="e7500-145">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="e7500-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e7500-146">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="e7500-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e7500-147">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="e7500-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e7500-148">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="e7500-148">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="e7500-149">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="e7500-149">Report Refresh Date</span></span>
- <span data-ttu-id="e7500-150">サイト Id</span><span class="sxs-lookup"><span data-stu-id="e7500-150">Site Id</span></span>
- <span data-ttu-id="e7500-151">サイトの URL</span><span class="sxs-lookup"><span data-stu-id="e7500-151">Site URL</span></span>
- <span data-ttu-id="e7500-152">所有者の表示名</span><span class="sxs-lookup"><span data-stu-id="e7500-152">Owner Display Name</span></span>
- <span data-ttu-id="e7500-153">削除済み</span><span class="sxs-lookup"><span data-stu-id="e7500-153">Is Deleted</span></span>
- <span data-ttu-id="e7500-154">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="e7500-154">Last Activity Date</span></span>
- <span data-ttu-id="e7500-155">ファイル数</span><span class="sxs-lookup"><span data-stu-id="e7500-155">File Count</span></span>
- <span data-ttu-id="e7500-156">アクティブなファイル数</span><span class="sxs-lookup"><span data-stu-id="e7500-156">Active File Count</span></span>
- <span data-ttu-id="e7500-157">ページ ビューの数</span><span class="sxs-lookup"><span data-stu-id="e7500-157">Page View Count</span></span>
- <span data-ttu-id="e7500-158">アクセスしたページ数</span><span class="sxs-lookup"><span data-stu-id="e7500-158">Visited Page Count</span></span>
- <span data-ttu-id="e7500-159">使用済みストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="e7500-159">Storage Used (Byte)</span></span>
- <span data-ttu-id="e7500-160">割り当て済みストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="e7500-160">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="e7500-161">ルート Web テンプレート</span><span class="sxs-lookup"><span data-stu-id="e7500-161">Root Web Template</span></span>
- <span data-ttu-id="e7500-162">所有者のプリンシパル名</span><span class="sxs-lookup"><span data-stu-id="e7500-162">Owner Principal Name</span></span>
- <span data-ttu-id="e7500-163">レポート期間</span><span class="sxs-lookup"><span data-stu-id="e7500-163">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="e7500-164">JSON</span><span class="sxs-lookup"><span data-stu-id="e7500-164">JSON</span></span>

<span data-ttu-id="e7500-165">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[Sharepointsite使い方詳細](../resources/sharepointsiteusagedetail.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e7500-165">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="e7500-166">この要求の既定のページサイズは200アイテムです。</span><span class="sxs-lookup"><span data-stu-id="e7500-166">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="e7500-167">例</span><span class="sxs-lookup"><span data-stu-id="e7500-167">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e7500-168">CSV</span><span class="sxs-lookup"><span data-stu-id="e7500-168">CSV</span></span>

<span data-ttu-id="e7500-169">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e7500-169">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e7500-170">要求</span><span class="sxs-lookup"><span data-stu-id="e7500-170">Request</span></span>

<span data-ttu-id="e7500-171">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e7500-171">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e7500-172">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e7500-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagedetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e7500-173">C#</span><span class="sxs-lookup"><span data-stu-id="e7500-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagedetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e7500-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e7500-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagedetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e7500-175">目的-C</span><span class="sxs-lookup"><span data-stu-id="e7500-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagedetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e7500-176">Java</span><span class="sxs-lookup"><span data-stu-id="e7500-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointsiteusagedetail-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e7500-177">応答</span><span class="sxs-lookup"><span data-stu-id="e7500-177">Response</span></span>

<span data-ttu-id="e7500-178">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e7500-178">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="e7500-179">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="e7500-179">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Id,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Page View Count,Visited Page Count,Storage Used (Byte),Storage Allocated (Byte),Root Web Template,Owner Principal Name,Report Period
```

### <a name="json"></a><span data-ttu-id="e7500-180">JSON</span><span class="sxs-lookup"><span data-stu-id="e7500-180">JSON</span></span>

<span data-ttu-id="e7500-181">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="e7500-181">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e7500-182">要求</span><span class="sxs-lookup"><span data-stu-id="e7500-182">Request</span></span>

<span data-ttu-id="e7500-183">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e7500-183">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e7500-184">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e7500-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagedetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e7500-185">C#</span><span class="sxs-lookup"><span data-stu-id="e7500-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagedetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e7500-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e7500-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagedetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e7500-187">目的-C</span><span class="sxs-lookup"><span data-stu-id="e7500-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagedetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e7500-188">Java</span><span class="sxs-lookup"><span data-stu-id="e7500-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointsiteusagedetail-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e7500-189">応答</span><span class="sxs-lookup"><span data-stu-id="e7500-189">Response</span></span>

<span data-ttu-id="e7500-190">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e7500-190">The following is an example of the response.</span></span>

> <span data-ttu-id="e7500-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e7500-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointSiteUsageDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 484

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointSiteUsageDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteId": "siteId-value", 
      "siteUrl": "siteUrl-value", 
      "ownerDisplayName": "ownerDisplayName-value", 
      "ownerPrincipalName": "ownerPrincipalName-value", 
      "isDeleted": false, 
      "lastActivityDate": "2017-09-01", 
      "fileCount": 170, 
      "activeFileCount": 25, 
      "pageViewCount": 7, 
      "visitedPageCount": 3, 
      "storageUsedInBytes": 63442116, 
      "storageAllocatedInBytes": 2748779094400, 
      "rootWebTemplate": "Publishing Site", 
      "reportPeriod": "7"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
