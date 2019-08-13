---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: グループ別の Yammer グループ アクティビティに関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 29a1af12c2700c789e9fb064dfa61fff95267589
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358378"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="dbdc0-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="dbdc0-103">reportRoot: getYammerGroupsActivityDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbdc0-104">グループ別の Yammer グループ アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-104">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="dbdc0-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer グループ アクティビティ](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="dbdc0-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dbdc0-106">Permissions</span></span>

<span data-ttu-id="dbdc0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dbdc0-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dbdc0-109">Permission type</span></span>                        | <span data-ttu-id="dbdc0-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dbdc0-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="dbdc0-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="dbdc0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dbdc0-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dbdc0-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="dbdc0-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dbdc0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbdc0-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-114">Not supported.</span></span>                           |
| <span data-ttu-id="dbdc0-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dbdc0-115">Application</span></span>                            | <span data-ttu-id="dbdc0-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dbdc0-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="dbdc0-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dbdc0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="dbdc0-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="dbdc0-118">Function parameters</span></span>

<span data-ttu-id="dbdc0-119">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="dbdc0-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="dbdc0-120">Parameter</span></span> | <span data-ttu-id="dbdc0-121">型</span><span class="sxs-lookup"><span data-stu-id="dbdc0-121">Type</span></span>   | <span data-ttu-id="dbdc0-122">説明</span><span class="sxs-lookup"><span data-stu-id="dbdc0-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="dbdc0-123">period</span><span class="sxs-lookup"><span data-stu-id="dbdc0-123">period</span></span>    | <span data-ttu-id="dbdc0-124">文字列</span><span class="sxs-lookup"><span data-stu-id="dbdc0-124">string</span></span> | <span data-ttu-id="dbdc0-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="dbdc0-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="dbdc0-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="dbdc0-128">date</span><span class="sxs-lookup"><span data-stu-id="dbdc0-128">date</span></span>      | <span data-ttu-id="dbdc0-129">日付</span><span class="sxs-lookup"><span data-stu-id="dbdc0-129">Date</span></span>   | <span data-ttu-id="dbdc0-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="dbdc0-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="dbdc0-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="dbdc0-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="dbdc0-134">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="dbdc0-135">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-135">The default output type is text/csv.</span></span> <span data-ttu-id="dbdc0-136">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dbdc0-137">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dbdc0-137">Request headers</span></span>

| <span data-ttu-id="dbdc0-138">名前</span><span class="sxs-lookup"><span data-stu-id="dbdc0-138">Name</span></span>          | <span data-ttu-id="dbdc0-139">説明</span><span class="sxs-lookup"><span data-stu-id="dbdc0-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="dbdc0-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbdc0-140">Authorization</span></span> | <span data-ttu-id="dbdc0-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="dbdc0-143">応答</span><span class="sxs-lookup"><span data-stu-id="dbdc0-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="dbdc0-144">CSV</span><span class="sxs-lookup"><span data-stu-id="dbdc0-144">CSV</span></span>

<span data-ttu-id="dbdc0-145">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="dbdc0-146">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="dbdc0-147">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="dbdc0-148">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="dbdc0-149">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="dbdc0-149">Report Refresh Date</span></span>
- <span data-ttu-id="dbdc0-150">グループ表示名</span><span class="sxs-lookup"><span data-stu-id="dbdc0-150">Group Display Name</span></span>
- <span data-ttu-id="dbdc0-151">削除済み</span><span class="sxs-lookup"><span data-stu-id="dbdc0-151">Is Deleted</span></span>
- <span data-ttu-id="dbdc0-152">所有者のプリンシパル名</span><span class="sxs-lookup"><span data-stu-id="dbdc0-152">Owner Principal Name</span></span>
- <span data-ttu-id="dbdc0-153">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="dbdc0-153">Last Activity Date</span></span>
- <span data-ttu-id="dbdc0-154">グループの種類</span><span class="sxs-lookup"><span data-stu-id="dbdc0-154">Group Type</span></span>
- <span data-ttu-id="dbdc0-155">Office 365 接続</span><span class="sxs-lookup"><span data-stu-id="dbdc0-155">Office 365 Connected</span></span>
- <span data-ttu-id="dbdc0-156">メンバー数</span><span class="sxs-lookup"><span data-stu-id="dbdc0-156">Member Count</span></span>
- <span data-ttu-id="dbdc0-157">投稿数</span><span class="sxs-lookup"><span data-stu-id="dbdc0-157">Posted Count</span></span>
- <span data-ttu-id="dbdc0-158">読み取り数</span><span class="sxs-lookup"><span data-stu-id="dbdc0-158">Read Count</span></span>
- <span data-ttu-id="dbdc0-159">「いいね!」の数</span><span class="sxs-lookup"><span data-stu-id="dbdc0-159">Liked Count</span></span>
- <span data-ttu-id="dbdc0-160">レポート期間</span><span class="sxs-lookup"><span data-stu-id="dbdc0-160">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="dbdc0-161">JSON</span><span class="sxs-lookup"><span data-stu-id="dbdc0-161">JSON</span></span>

<span data-ttu-id="dbdc0-162">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-162">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="dbdc0-163">この要求の既定のページサイズは200アイテムです。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-163">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="dbdc0-164">例</span><span class="sxs-lookup"><span data-stu-id="dbdc0-164">Example</span></span>

### <a name="csv"></a><span data-ttu-id="dbdc0-165">CSV</span><span class="sxs-lookup"><span data-stu-id="dbdc0-165">CSV</span></span>

<span data-ttu-id="dbdc0-166">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-166">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="dbdc0-167">要求</span><span class="sxs-lookup"><span data-stu-id="dbdc0-167">Request</span></span>

<span data-ttu-id="dbdc0-168">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-168">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dbdc0-169">プロトコル</span><span class="sxs-lookup"><span data-stu-id="dbdc0-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dbdc0-170">C#</span><span class="sxs-lookup"><span data-stu-id="dbdc0-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivitydetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dbdc0-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dbdc0-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivitydetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dbdc0-172">目的-C</span><span class="sxs-lookup"><span data-stu-id="dbdc0-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivitydetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dbdc0-173">Java</span><span class="sxs-lookup"><span data-stu-id="dbdc0-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammergroupsactivitydetail-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dbdc0-174">応答</span><span class="sxs-lookup"><span data-stu-id="dbdc0-174">Response</span></span>

<span data-ttu-id="dbdc0-175">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-175">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="dbdc0-176">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-176">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Office 365 Connected,Member Count,Posted Count,Read Count,Liked Count,Report Period
```

### <a name="json"></a><span data-ttu-id="dbdc0-177">JSON</span><span class="sxs-lookup"><span data-stu-id="dbdc0-177">JSON</span></span>

<span data-ttu-id="dbdc0-178">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-178">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="dbdc0-179">要求</span><span class="sxs-lookup"><span data-stu-id="dbdc0-179">Request</span></span>

<span data-ttu-id="dbdc0-180">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-180">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dbdc0-181">プロトコル</span><span class="sxs-lookup"><span data-stu-id="dbdc0-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dbdc0-182">C#</span><span class="sxs-lookup"><span data-stu-id="dbdc0-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivitydetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dbdc0-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dbdc0-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivitydetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dbdc0-184">目的-C</span><span class="sxs-lookup"><span data-stu-id="dbdc0-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivitydetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dbdc0-185">Java</span><span class="sxs-lookup"><span data-stu-id="dbdc0-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammergroupsactivitydetail-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dbdc0-186">応答</span><span class="sxs-lookup"><span data-stu-id="dbdc0-186">Response</span></span>

<span data-ttu-id="dbdc0-187">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-187">The following is an example of the response.</span></span>

> <span data-ttu-id="dbdc0-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="dbdc0-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerGroupsActivityDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 441

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerGroupsActivityDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "groupDisplayName": "groupDisplayName-value", 
      "isDeleted": false, 
      "ownerPrincipalName": "ownerPrincipalName-value", 
      "lastActivityDate": "2017-08-30", 
      "groupType": "private", 
      "office365Connected": true, 
      "memberCount": 176, 
      "postedCount": 15, 
      "readCount": 24, 
      "likedCount": 3, 
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
