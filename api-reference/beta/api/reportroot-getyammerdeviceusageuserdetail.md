---
title: 'reportRoot: getYammerDeviceUsageUserDetail function'
description: ユーザー別の Yammer デバイス使用状況に関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 4bb392b06ff5c5a96f2d4e7aabd354ef022703b2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358438"
---
# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="e10b4-103">reportRoot: getYammerDeviceUsageUserDetail function</span><span class="sxs-lookup"><span data-stu-id="e10b4-103">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e10b4-104">ユーザー別の Yammer デバイス使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="e10b4-104">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="e10b4-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer デバイスの使用状況](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e10b4-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="e10b4-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e10b4-106">Permissions</span></span>

<span data-ttu-id="e10b4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e10b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e10b4-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e10b4-109">Permission type</span></span>                        | <span data-ttu-id="e10b4-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e10b4-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e10b4-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="e10b4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e10b4-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e10b4-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e10b4-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e10b4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e10b4-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e10b4-114">Not supported.</span></span>                           |
| <span data-ttu-id="e10b4-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e10b4-115">Application</span></span>                            | <span data-ttu-id="e10b4-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e10b4-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e10b4-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e10b4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="e10b4-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="e10b4-118">Function parameters</span></span>

<span data-ttu-id="e10b4-119">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="e10b4-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="e10b4-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e10b4-120">Parameter</span></span> | <span data-ttu-id="e10b4-121">型</span><span class="sxs-lookup"><span data-stu-id="e10b4-121">Type</span></span>   | <span data-ttu-id="e10b4-122">説明</span><span class="sxs-lookup"><span data-stu-id="e10b4-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e10b4-123">period</span><span class="sxs-lookup"><span data-stu-id="e10b4-123">period</span></span>    | <span data-ttu-id="e10b4-124">文字列</span><span class="sxs-lookup"><span data-stu-id="e10b4-124">string</span></span> | <span data-ttu-id="e10b4-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="e10b4-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e10b4-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="e10b4-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e10b4-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="e10b4-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="e10b4-128">date</span><span class="sxs-lookup"><span data-stu-id="e10b4-128">date</span></span>      | <span data-ttu-id="e10b4-129">日付</span><span class="sxs-lookup"><span data-stu-id="e10b4-129">Date</span></span>   | <span data-ttu-id="e10b4-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="e10b4-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="e10b4-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="e10b4-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="e10b4-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="e10b4-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="e10b4-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e10b4-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="e10b4-134">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e10b4-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e10b4-135">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="e10b4-135">The default output type is text/csv.</span></span> <span data-ttu-id="e10b4-136">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="e10b4-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e10b4-137">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e10b4-137">Request headers</span></span>

| <span data-ttu-id="e10b4-138">名前</span><span class="sxs-lookup"><span data-stu-id="e10b4-138">Name</span></span>          | <span data-ttu-id="e10b4-139">説明</span><span class="sxs-lookup"><span data-stu-id="e10b4-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e10b4-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="e10b4-140">Authorization</span></span> | <span data-ttu-id="e10b4-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e10b4-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e10b4-143">応答</span><span class="sxs-lookup"><span data-stu-id="e10b4-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e10b4-144">CSV</span><span class="sxs-lookup"><span data-stu-id="e10b4-144">CSV</span></span>

<span data-ttu-id="e10b4-145">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="e10b4-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e10b4-146">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="e10b4-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e10b4-147">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="e10b4-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e10b4-148">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="e10b4-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e10b4-149">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="e10b4-149">Report Refresh Date</span></span>
- <span data-ttu-id="e10b4-150">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="e10b4-150">User Principal Name</span></span>
- <span data-ttu-id="e10b4-151">表示名</span><span class="sxs-lookup"><span data-stu-id="e10b4-151">Display Name</span></span>
- <span data-ttu-id="e10b4-152">ユーザーの状態</span><span class="sxs-lookup"><span data-stu-id="e10b4-152">User State</span></span>
- <span data-ttu-id="e10b4-153">状態変更日付</span><span class="sxs-lookup"><span data-stu-id="e10b4-153">State Change Date</span></span>
- <span data-ttu-id="e10b4-154">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="e10b4-154">Last Activity Date</span></span>
- <span data-ttu-id="e10b4-155">Web の使用</span><span class="sxs-lookup"><span data-stu-id="e10b4-155">Used Web</span></span>
- <span data-ttu-id="e10b4-156">Windows スマートフォンの使用</span><span class="sxs-lookup"><span data-stu-id="e10b4-156">Used Windows Phone</span></span>
- <span data-ttu-id="e10b4-157">Android スマートフォンの使用</span><span class="sxs-lookup"><span data-stu-id="e10b4-157">Used Android Phone</span></span>
- <span data-ttu-id="e10b4-158">iPhone の使用</span><span class="sxs-lookup"><span data-stu-id="e10b4-158">Used iPhone</span></span>
- <span data-ttu-id="e10b4-159">IPad の使用</span><span class="sxs-lookup"><span data-stu-id="e10b4-159">Used iPad</span></span>
- <span data-ttu-id="e10b4-160">その他の使用</span><span class="sxs-lookup"><span data-stu-id="e10b4-160">Used Others</span></span>
- <span data-ttu-id="e10b4-161">レポート期間</span><span class="sxs-lookup"><span data-stu-id="e10b4-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="e10b4-162">JSON</span><span class="sxs-lookup"><span data-stu-id="e10b4-162">JSON</span></span>

<span data-ttu-id="e10b4-163">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e10b4-163">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="e10b4-164">この要求の既定のページサイズは200アイテムです。</span><span class="sxs-lookup"><span data-stu-id="e10b4-164">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="e10b4-165">例</span><span class="sxs-lookup"><span data-stu-id="e10b4-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e10b4-166">CSV</span><span class="sxs-lookup"><span data-stu-id="e10b4-166">CSV</span></span>

<span data-ttu-id="e10b4-167">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e10b4-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e10b4-168">要求</span><span class="sxs-lookup"><span data-stu-id="e10b4-168">Request</span></span>

<span data-ttu-id="e10b4-169">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e10b4-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e10b4-170">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e10b4-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e10b4-171">C#</span><span class="sxs-lookup"><span data-stu-id="e10b4-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammerdeviceusageuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e10b4-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e10b4-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammerdeviceusageuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e10b4-173">目的-C</span><span class="sxs-lookup"><span data-stu-id="e10b4-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammerdeviceusageuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e10b4-174">Java</span><span class="sxs-lookup"><span data-stu-id="e10b4-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammerdeviceusageuserdetail-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e10b4-175">応答</span><span class="sxs-lookup"><span data-stu-id="e10b4-175">Response</span></span>

<span data-ttu-id="e10b4-176">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e10b4-176">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="e10b4-177">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="e10b4-177">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Used Web,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Used Others,Report Period
```

### <a name="json"></a><span data-ttu-id="e10b4-178">JSON</span><span class="sxs-lookup"><span data-stu-id="e10b4-178">JSON</span></span>

<span data-ttu-id="e10b4-179">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="e10b4-179">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e10b4-180">要求</span><span class="sxs-lookup"><span data-stu-id="e10b4-180">Request</span></span>

<span data-ttu-id="e10b4-181">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e10b4-181">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e10b4-182">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e10b4-182">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e10b4-183">C#</span><span class="sxs-lookup"><span data-stu-id="e10b4-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammerdeviceusageuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e10b4-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e10b4-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammerdeviceusageuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e10b4-185">目的-C</span><span class="sxs-lookup"><span data-stu-id="e10b4-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammerdeviceusageuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e10b4-186">Java</span><span class="sxs-lookup"><span data-stu-id="e10b4-186">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammerdeviceusageuserdetail-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e10b4-187">応答</span><span class="sxs-lookup"><span data-stu-id="e10b4-187">Response</span></span>

<span data-ttu-id="e10b4-188">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e10b4-188">The following is an example of the response.</span></span>

> <span data-ttu-id="e10b4-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e10b4-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 442

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerDeviceUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-06", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "userState": "active", 
      "stateChangeDate": "2012-06-26", 
      "lastActivityDate": "2017-09-06", 
      "usedWeb": true, 
      "usedWindowsPhone": false, 
      "usedAndroidPhone": false, 
      "usediPhone": false, 
      "usediPad": false, 
      "usedOthers": false, 
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
