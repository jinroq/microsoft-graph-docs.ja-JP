---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: グループ別の Yammer グループ アクティビティに関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: cfe8dfd26bbc7de0806c7f41286800a9872d3eb9
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639024"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="41fc2-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="41fc2-103">reportRoot: getYammerGroupsActivityDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41fc2-104">グループ別の Yammer グループ アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="41fc2-104">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="41fc2-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer グループ アクティビティ](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="41fc2-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="41fc2-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="41fc2-106">Permissions</span></span>

<span data-ttu-id="41fc2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="41fc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="41fc2-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="41fc2-109">Permission type</span></span>                        | <span data-ttu-id="41fc2-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="41fc2-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="41fc2-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="41fc2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="41fc2-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="41fc2-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="41fc2-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="41fc2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41fc2-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="41fc2-114">Not supported.</span></span>                           |
| <span data-ttu-id="41fc2-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="41fc2-115">Application</span></span>                            | <span data-ttu-id="41fc2-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="41fc2-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="41fc2-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="41fc2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="41fc2-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="41fc2-118">Function parameters</span></span>

<span data-ttu-id="41fc2-119">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="41fc2-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="41fc2-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="41fc2-120">Parameter</span></span> | <span data-ttu-id="41fc2-121">型</span><span class="sxs-lookup"><span data-stu-id="41fc2-121">Type</span></span>   | <span data-ttu-id="41fc2-122">説明</span><span class="sxs-lookup"><span data-stu-id="41fc2-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="41fc2-123">period</span><span class="sxs-lookup"><span data-stu-id="41fc2-123">period</span></span>    | <span data-ttu-id="41fc2-124">文字列</span><span class="sxs-lookup"><span data-stu-id="41fc2-124">string</span></span> | <span data-ttu-id="41fc2-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="41fc2-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="41fc2-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="41fc2-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="41fc2-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="41fc2-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="41fc2-128">date</span><span class="sxs-lookup"><span data-stu-id="41fc2-128">date</span></span>      | <span data-ttu-id="41fc2-129">日付</span><span class="sxs-lookup"><span data-stu-id="41fc2-129">Date</span></span>   | <span data-ttu-id="41fc2-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="41fc2-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="41fc2-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="41fc2-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="41fc2-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="41fc2-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="41fc2-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="41fc2-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="41fc2-134">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="41fc2-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="41fc2-135">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="41fc2-135">The default output type is text/csv.</span></span> <span data-ttu-id="41fc2-136">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="41fc2-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41fc2-137">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="41fc2-137">Request headers</span></span>

| <span data-ttu-id="41fc2-138">名前</span><span class="sxs-lookup"><span data-stu-id="41fc2-138">Name</span></span>          | <span data-ttu-id="41fc2-139">説明</span><span class="sxs-lookup"><span data-stu-id="41fc2-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="41fc2-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="41fc2-140">Authorization</span></span> | <span data-ttu-id="41fc2-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="41fc2-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="41fc2-143">応答</span><span class="sxs-lookup"><span data-stu-id="41fc2-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="41fc2-144">CSV</span><span class="sxs-lookup"><span data-stu-id="41fc2-144">CSV</span></span>

<span data-ttu-id="41fc2-145">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="41fc2-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="41fc2-146">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="41fc2-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="41fc2-147">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="41fc2-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="41fc2-148">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="41fc2-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="41fc2-149">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="41fc2-149">Report Refresh Date</span></span>
- <span data-ttu-id="41fc2-150">グループ表示名</span><span class="sxs-lookup"><span data-stu-id="41fc2-150">Group Display Name</span></span>
- <span data-ttu-id="41fc2-151">削除済み</span><span class="sxs-lookup"><span data-stu-id="41fc2-151">Is Deleted</span></span>
- <span data-ttu-id="41fc2-152">所有者のプリンシパル名</span><span class="sxs-lookup"><span data-stu-id="41fc2-152">Owner Principal Name</span></span>
- <span data-ttu-id="41fc2-153">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="41fc2-153">Last Activity Date</span></span>
- <span data-ttu-id="41fc2-154">グループの種類</span><span class="sxs-lookup"><span data-stu-id="41fc2-154">Group Type</span></span>
- <span data-ttu-id="41fc2-155">Office 365 接続</span><span class="sxs-lookup"><span data-stu-id="41fc2-155">Office 365 Connected</span></span>
- <span data-ttu-id="41fc2-156">メンバー数</span><span class="sxs-lookup"><span data-stu-id="41fc2-156">Member Count</span></span>
- <span data-ttu-id="41fc2-157">投稿数</span><span class="sxs-lookup"><span data-stu-id="41fc2-157">Posted Count</span></span>
- <span data-ttu-id="41fc2-158">読み取り数</span><span class="sxs-lookup"><span data-stu-id="41fc2-158">Read Count</span></span>
- <span data-ttu-id="41fc2-159">「いいね!」の数</span><span class="sxs-lookup"><span data-stu-id="41fc2-159">Liked Count</span></span>
- <span data-ttu-id="41fc2-160">レポート期間</span><span class="sxs-lookup"><span data-stu-id="41fc2-160">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="41fc2-161">JSON</span><span class="sxs-lookup"><span data-stu-id="41fc2-161">JSON</span></span>

<span data-ttu-id="41fc2-162">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="41fc2-162">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="41fc2-163">この要求の既定のページサイズは200アイテムです。</span><span class="sxs-lookup"><span data-stu-id="41fc2-163">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="41fc2-164">例</span><span class="sxs-lookup"><span data-stu-id="41fc2-164">Example</span></span>

### <a name="csv"></a><span data-ttu-id="41fc2-165">CSV</span><span class="sxs-lookup"><span data-stu-id="41fc2-165">CSV</span></span>

<span data-ttu-id="41fc2-166">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="41fc2-166">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="41fc2-167">要求</span><span class="sxs-lookup"><span data-stu-id="41fc2-167">Request</span></span>

<span data-ttu-id="41fc2-168">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="41fc2-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="41fc2-169">応答</span><span class="sxs-lookup"><span data-stu-id="41fc2-169">Response</span></span>

<span data-ttu-id="41fc2-170">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="41fc2-170">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="41fc2-171">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="41fc2-171">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="41fc2-172">Visual</span><span class="sxs-lookup"><span data-stu-id="41fc2-172">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivitydetail_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="41fc2-173">Java</span><span class="sxs-lookup"><span data-stu-id="41fc2-173">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivitydetail_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="41fc2-174">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="41fc2-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="41fc2-175">JSON</span><span class="sxs-lookup"><span data-stu-id="41fc2-175">JSON</span></span>

<span data-ttu-id="41fc2-176">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="41fc2-176">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="41fc2-177">要求</span><span class="sxs-lookup"><span data-stu-id="41fc2-177">Request</span></span>

<span data-ttu-id="41fc2-178">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="41fc2-178">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="41fc2-179">応答</span><span class="sxs-lookup"><span data-stu-id="41fc2-179">Response</span></span>

<span data-ttu-id="41fc2-180">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="41fc2-180">The following is an example of the response.</span></span>

> <span data-ttu-id="41fc2-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="41fc2-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="41fc2-183">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="41fc2-183">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="41fc2-184">Visual</span><span class="sxs-lookup"><span data-stu-id="41fc2-184">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivitydetail_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="41fc2-185">Java</span><span class="sxs-lookup"><span data-stu-id="41fc2-185">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivitydetail_json-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/reportroot-getyammergroupsactivitydetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getyammergroupsactivitydetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getyammergroupsactivitydetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getyammergroupsactivitydetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
