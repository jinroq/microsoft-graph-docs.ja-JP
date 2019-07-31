---
title: 'reportRoot: getSharePointActivityUserDetail'
description: ユーザー別の SharePoint アクティビティに関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: b1e98560e91b8c33de7467f71470dcc4217c1530
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983223"
---
# <a name="reportroot-getsharepointactivityuserdetail"></a><span data-ttu-id="0b588-103">reportRoot: getSharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="0b588-103">reportRoot: getSharePointActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b588-104">ユーザー別の SharePoint アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="0b588-104">Get details about SharePoint activity by user.</span></span>

> <span data-ttu-id="0b588-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint アクティビティ](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0b588-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="0b588-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0b588-106">Permissions</span></span>

<span data-ttu-id="0b588-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0b588-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0b588-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0b588-109">Permission type</span></span>                        | <span data-ttu-id="0b588-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0b588-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0b588-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="0b588-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0b588-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b588-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0b588-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0b588-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b588-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0b588-114">Not supported.</span></span>                           |
| <span data-ttu-id="0b588-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0b588-115">Application</span></span>                            | <span data-ttu-id="0b588-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b588-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0b588-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0b588-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserDetail(period='{period_value}')
GET /reports/getSharePointActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="0b588-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="0b588-118">Function parameters</span></span>

<span data-ttu-id="0b588-119">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="0b588-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="0b588-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="0b588-120">Parameter</span></span> | <span data-ttu-id="0b588-121">型</span><span class="sxs-lookup"><span data-stu-id="0b588-121">Type</span></span>   | <span data-ttu-id="0b588-122">説明</span><span class="sxs-lookup"><span data-stu-id="0b588-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0b588-123">period</span><span class="sxs-lookup"><span data-stu-id="0b588-123">period</span></span>    | <span data-ttu-id="0b588-124">文字列</span><span class="sxs-lookup"><span data-stu-id="0b588-124">string</span></span> | <span data-ttu-id="0b588-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="0b588-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0b588-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="0b588-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0b588-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="0b588-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="0b588-128">date</span><span class="sxs-lookup"><span data-stu-id="0b588-128">date</span></span>      | <span data-ttu-id="0b588-129">日付</span><span class="sxs-lookup"><span data-stu-id="0b588-129">Date</span></span>   | <span data-ttu-id="0b588-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="0b588-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="0b588-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="0b588-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="0b588-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="0b588-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="0b588-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0b588-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="0b588-134">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0b588-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="0b588-135">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="0b588-135">The default output type is text/csv.</span></span> <span data-ttu-id="0b588-136">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="0b588-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b588-137">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0b588-137">Request headers</span></span>

| <span data-ttu-id="0b588-138">名前</span><span class="sxs-lookup"><span data-stu-id="0b588-138">Name</span></span>          | <span data-ttu-id="0b588-139">説明</span><span class="sxs-lookup"><span data-stu-id="0b588-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0b588-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b588-140">Authorization</span></span> | <span data-ttu-id="0b588-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0b588-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0b588-143">応答</span><span class="sxs-lookup"><span data-stu-id="0b588-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="0b588-144">CSV</span><span class="sxs-lookup"><span data-stu-id="0b588-144">CSV</span></span>

<span data-ttu-id="0b588-145">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="0b588-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0b588-146">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="0b588-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0b588-147">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="0b588-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0b588-148">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="0b588-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0b588-149">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="0b588-149">Report Refresh Date</span></span>
- <span data-ttu-id="0b588-150">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="0b588-150">User Principal Name</span></span>
- <span data-ttu-id="0b588-151">削除済み</span><span class="sxs-lookup"><span data-stu-id="0b588-151">Is Deleted</span></span>
- <span data-ttu-id="0b588-152">削除日</span><span class="sxs-lookup"><span data-stu-id="0b588-152">Deleted Date</span></span>
- <span data-ttu-id="0b588-153">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="0b588-153">Last Activity Date</span></span>
- <span data-ttu-id="0b588-154">表示済みまたは編集済みファイルの数</span><span class="sxs-lookup"><span data-stu-id="0b588-154">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="0b588-155">同期済みファイルの数</span><span class="sxs-lookup"><span data-stu-id="0b588-155">Synced File Count</span></span>
- <span data-ttu-id="0b588-156">社内で共有済みファイルの数</span><span class="sxs-lookup"><span data-stu-id="0b588-156">Shared Internally File Count</span></span>
- <span data-ttu-id="0b588-157">外部で共有済みファイルの数</span><span class="sxs-lookup"><span data-stu-id="0b588-157">Shared Externally File Count</span></span>
- <span data-ttu-id="0b588-158">アクセスしたページ数</span><span class="sxs-lookup"><span data-stu-id="0b588-158">Visited Page Count</span></span>
- <span data-ttu-id="0b588-159">割り当て済み製品</span><span class="sxs-lookup"><span data-stu-id="0b588-159">Assigned Products</span></span>
- <span data-ttu-id="0b588-160">レポート期間</span><span class="sxs-lookup"><span data-stu-id="0b588-160">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="0b588-161">JSON</span><span class="sxs-lookup"><span data-stu-id="0b588-161">JSON</span></span>

<span data-ttu-id="0b588-162">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[Sharepointactivityuserdetail](../resources/sharepointactivityuserdetail.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0b588-162">If successful, this method returns a `200 OK` response code and a **[sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="0b588-163">この要求の既定のページサイズは200アイテムです。</span><span class="sxs-lookup"><span data-stu-id="0b588-163">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="0b588-164">例</span><span class="sxs-lookup"><span data-stu-id="0b588-164">Example</span></span>

### <a name="csv"></a><span data-ttu-id="0b588-165">CSV</span><span class="sxs-lookup"><span data-stu-id="0b588-165">CSV</span></span>

<span data-ttu-id="0b588-166">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0b588-166">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="0b588-167">要求</span><span class="sxs-lookup"><span data-stu-id="0b588-167">Request</span></span>

<span data-ttu-id="0b588-168">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0b588-168">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0b588-169">プロトコル</span><span class="sxs-lookup"><span data-stu-id="0b588-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0b588-170">C#</span><span class="sxs-lookup"><span data-stu-id="0b588-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointactivityuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b588-171">Javascript</span><span class="sxs-lookup"><span data-stu-id="0b588-171">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointactivityuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0b588-172">目的-C</span><span class="sxs-lookup"><span data-stu-id="0b588-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointactivityuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0b588-173">Java</span><span class="sxs-lookup"><span data-stu-id="0b588-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointactivityuserdetail-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0b588-174">応答</span><span class="sxs-lookup"><span data-stu-id="0b588-174">Response</span></span>

<span data-ttu-id="0b588-175">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0b588-175">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="0b588-176">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="0b588-176">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Visited Page Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="0b588-177">JSON</span><span class="sxs-lookup"><span data-stu-id="0b588-177">JSON</span></span>

<span data-ttu-id="0b588-178">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="0b588-178">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="0b588-179">要求</span><span class="sxs-lookup"><span data-stu-id="0b588-179">Request</span></span>

<span data-ttu-id="0b588-180">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0b588-180">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0b588-181">プロトコル</span><span class="sxs-lookup"><span data-stu-id="0b588-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0b588-182">C#</span><span class="sxs-lookup"><span data-stu-id="0b588-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointactivityuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b588-183">Javascript</span><span class="sxs-lookup"><span data-stu-id="0b588-183">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointactivityuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0b588-184">目的-C</span><span class="sxs-lookup"><span data-stu-id="0b588-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointactivityuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0b588-185">Java</span><span class="sxs-lookup"><span data-stu-id="0b588-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointactivityuserdetail-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0b588-186">応答</span><span class="sxs-lookup"><span data-stu-id="0b588-186">Response</span></span>

<span data-ttu-id="0b588-187">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0b588-187">The following is an example of the response.</span></span>

> <span data-ttu-id="0b588-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0b588-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 473

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "viewedOrEditedFileCount": 4, 
      "syncedFileCount": 0, 
      "sharedInternallyFileCount": 0, 
      "sharedExternallyFileCount": 0, 
      "visitedPageCount": 1, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
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
