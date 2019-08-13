---
title: 'reportRoot: getYammerActivityUserDetail'
description: ユーザー別の Yammer アクティビティに関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 3047ad54abe54df5beefec97180d7c5f7b8d60e7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358601"
---
# <a name="reportroot-getyammeractivityuserdetail"></a><span data-ttu-id="96970-103">reportRoot: getYammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="96970-103">reportRoot: getYammerActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96970-104">ユーザー別の Yammer アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="96970-104">Get details about Yammer activity by user.</span></span>

> <span data-ttu-id="96970-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer アクティビティ](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="96970-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="96970-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="96970-106">Permissions</span></span>

<span data-ttu-id="96970-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="96970-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="96970-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="96970-109">Permission type</span></span>                        | <span data-ttu-id="96970-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="96970-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="96970-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="96970-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="96970-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="96970-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="96970-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="96970-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96970-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96970-114">Not supported.</span></span>                           |
| <span data-ttu-id="96970-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="96970-115">Application</span></span>                            | <span data-ttu-id="96970-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="96970-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="96970-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="96970-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserDetail(period='{period_value}')
GET /reports/getYammerActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="96970-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="96970-118">Function parameters</span></span>

<span data-ttu-id="96970-119">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="96970-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="96970-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="96970-120">Parameter</span></span> | <span data-ttu-id="96970-121">型</span><span class="sxs-lookup"><span data-stu-id="96970-121">Type</span></span>   | <span data-ttu-id="96970-122">説明</span><span class="sxs-lookup"><span data-stu-id="96970-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="96970-123">period</span><span class="sxs-lookup"><span data-stu-id="96970-123">period</span></span>    | <span data-ttu-id="96970-124">文字列</span><span class="sxs-lookup"><span data-stu-id="96970-124">string</span></span> | <span data-ttu-id="96970-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="96970-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="96970-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="96970-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="96970-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="96970-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="96970-128">date</span><span class="sxs-lookup"><span data-stu-id="96970-128">date</span></span>      | <span data-ttu-id="96970-129">日付</span><span class="sxs-lookup"><span data-stu-id="96970-129">Date</span></span>   | <span data-ttu-id="96970-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="96970-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="96970-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="96970-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="96970-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="96970-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="96970-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="96970-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="96970-134">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="96970-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="96970-135">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="96970-135">The default output type is text/csv.</span></span> <span data-ttu-id="96970-136">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="96970-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="96970-137">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="96970-137">Request headers</span></span>

| <span data-ttu-id="96970-138">名前</span><span class="sxs-lookup"><span data-stu-id="96970-138">Name</span></span>          | <span data-ttu-id="96970-139">説明</span><span class="sxs-lookup"><span data-stu-id="96970-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="96970-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="96970-140">Authorization</span></span> | <span data-ttu-id="96970-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="96970-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="96970-143">応答</span><span class="sxs-lookup"><span data-stu-id="96970-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="96970-144">CSV</span><span class="sxs-lookup"><span data-stu-id="96970-144">CSV</span></span>

<span data-ttu-id="96970-145">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="96970-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="96970-146">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="96970-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="96970-147">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="96970-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="96970-148">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="96970-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="96970-149">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="96970-149">Report Refresh Date</span></span>
- <span data-ttu-id="96970-150">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="96970-150">User Principal Name</span></span>
- <span data-ttu-id="96970-151">表示名</span><span class="sxs-lookup"><span data-stu-id="96970-151">Display Name</span></span>
- <span data-ttu-id="96970-152">ユーザーの状態</span><span class="sxs-lookup"><span data-stu-id="96970-152">User State</span></span>
- <span data-ttu-id="96970-153">状態変更日付</span><span class="sxs-lookup"><span data-stu-id="96970-153">State Change Date</span></span>
- <span data-ttu-id="96970-154">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="96970-154">Last Activity Date</span></span>
- <span data-ttu-id="96970-155">投稿数</span><span class="sxs-lookup"><span data-stu-id="96970-155">Posted Count</span></span>
- <span data-ttu-id="96970-156">読み取り数</span><span class="sxs-lookup"><span data-stu-id="96970-156">Read Count</span></span>
- <span data-ttu-id="96970-157">「いいね!」の数</span><span class="sxs-lookup"><span data-stu-id="96970-157">Liked Count</span></span>
- <span data-ttu-id="96970-158">割り当て済み製品</span><span class="sxs-lookup"><span data-stu-id="96970-158">Assigned Products</span></span>
- <span data-ttu-id="96970-159">レポート期間</span><span class="sxs-lookup"><span data-stu-id="96970-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="96970-160">JSON</span><span class="sxs-lookup"><span data-stu-id="96970-160">JSON</span></span>

<span data-ttu-id="96970-161">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[yammerActivityUserDetail](../resources/yammeractivityuserdetail.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="96970-161">If successful, this method returns a `200 OK` response code and a **[yammerActivityUserDetail](../resources/yammeractivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="96970-162">この要求の既定のページサイズは200アイテムです。</span><span class="sxs-lookup"><span data-stu-id="96970-162">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="96970-163">例</span><span class="sxs-lookup"><span data-stu-id="96970-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="96970-164">CSV</span><span class="sxs-lookup"><span data-stu-id="96970-164">CSV</span></span>

<span data-ttu-id="96970-165">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="96970-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="96970-166">要求</span><span class="sxs-lookup"><span data-stu-id="96970-166">Request</span></span>

<span data-ttu-id="96970-167">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="96970-167">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="96970-168">プロトコル</span><span class="sxs-lookup"><span data-stu-id="96970-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="96970-169">C#</span><span class="sxs-lookup"><span data-stu-id="96970-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammeractivityuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="96970-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96970-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammeractivityuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="96970-171">目的-C</span><span class="sxs-lookup"><span data-stu-id="96970-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammeractivityuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="96970-172">Java</span><span class="sxs-lookup"><span data-stu-id="96970-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammeractivityuserdetail-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="96970-173">応答</span><span class="sxs-lookup"><span data-stu-id="96970-173">Response</span></span>

<span data-ttu-id="96970-174">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="96970-174">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="96970-175">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="96970-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Posted Count,Read Count,Liked Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="96970-176">JSON</span><span class="sxs-lookup"><span data-stu-id="96970-176">JSON</span></span>

<span data-ttu-id="96970-177">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="96970-177">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="96970-178">要求</span><span class="sxs-lookup"><span data-stu-id="96970-178">Request</span></span>

<span data-ttu-id="96970-179">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="96970-179">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="96970-180">プロトコル</span><span class="sxs-lookup"><span data-stu-id="96970-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="96970-181">C#</span><span class="sxs-lookup"><span data-stu-id="96970-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammeractivityuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="96970-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96970-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammeractivityuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="96970-183">目的-C</span><span class="sxs-lookup"><span data-stu-id="96970-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammeractivityuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="96970-184">Java</span><span class="sxs-lookup"><span data-stu-id="96970-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammeractivityuserdetail-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="96970-185">応答</span><span class="sxs-lookup"><span data-stu-id="96970-185">Response</span></span>

<span data-ttu-id="96970-186">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="96970-186">The following is an example of the response.</span></span>

> <span data-ttu-id="96970-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="96970-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 434

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "userState": "active", 
      "stateChangeDate": "2015-08-26", 
      "lastActivityDate": "2017-09-01", 
      "postedCount": 2, 
      "readCount": 5, 
      "likedCount": 0, 
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
