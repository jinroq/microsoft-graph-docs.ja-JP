---
title: 'reportRoot: getSkypeForBusinessActivityUserDetail'
description: ユーザー別の Skype for Business アクティビティに関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: ab502e9cbc1df0d714c4733038157da872455c07
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639258"
---
# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="6e647-103">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="6e647-103">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e647-104">ユーザー別の Skype for Business アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="6e647-104">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="6e647-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business アクティビティ](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6e647-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="6e647-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6e647-106">Permissions</span></span>

<span data-ttu-id="6e647-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6e647-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6e647-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6e647-109">Permission type</span></span>                        | <span data-ttu-id="6e647-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6e647-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6e647-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="6e647-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6e647-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e647-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6e647-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6e647-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e647-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6e647-114">Not supported.</span></span>                           |
| <span data-ttu-id="6e647-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6e647-115">Application</span></span>                            | <span data-ttu-id="6e647-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e647-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6e647-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6e647-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="6e647-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="6e647-118">Function parameters</span></span>

<span data-ttu-id="6e647-119">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="6e647-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="6e647-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="6e647-120">Parameter</span></span> | <span data-ttu-id="6e647-121">型</span><span class="sxs-lookup"><span data-stu-id="6e647-121">Type</span></span>   | <span data-ttu-id="6e647-122">説明</span><span class="sxs-lookup"><span data-stu-id="6e647-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6e647-123">period</span><span class="sxs-lookup"><span data-stu-id="6e647-123">period</span></span>    | <span data-ttu-id="6e647-124">文字列</span><span class="sxs-lookup"><span data-stu-id="6e647-124">string</span></span> | <span data-ttu-id="6e647-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="6e647-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6e647-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="6e647-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6e647-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="6e647-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="6e647-128">date</span><span class="sxs-lookup"><span data-stu-id="6e647-128">date</span></span>      | <span data-ttu-id="6e647-129">日付</span><span class="sxs-lookup"><span data-stu-id="6e647-129">Date</span></span>   | <span data-ttu-id="6e647-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="6e647-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="6e647-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="6e647-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="6e647-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="6e647-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="6e647-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6e647-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="6e647-134">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6e647-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="6e647-135">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="6e647-135">The default output type is text/csv.</span></span> <span data-ttu-id="6e647-136">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="6e647-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e647-137">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6e647-137">Request headers</span></span>

| <span data-ttu-id="6e647-138">名前</span><span class="sxs-lookup"><span data-stu-id="6e647-138">Name</span></span>          | <span data-ttu-id="6e647-139">説明</span><span class="sxs-lookup"><span data-stu-id="6e647-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="6e647-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e647-140">Authorization</span></span> | <span data-ttu-id="6e647-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6e647-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6e647-143">応答</span><span class="sxs-lookup"><span data-stu-id="6e647-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="6e647-144">CSV</span><span class="sxs-lookup"><span data-stu-id="6e647-144">CSV</span></span>

<span data-ttu-id="6e647-145">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="6e647-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6e647-146">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="6e647-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6e647-147">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="6e647-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6e647-148">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="6e647-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6e647-149">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="6e647-149">Report Refresh Date</span></span>
- <span data-ttu-id="6e647-150">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="6e647-150">User Principal Name</span></span>
- <span data-ttu-id="6e647-151">削除済み</span><span class="sxs-lookup"><span data-stu-id="6e647-151">Is Deleted</span></span>
- <span data-ttu-id="6e647-152">削除日</span><span class="sxs-lookup"><span data-stu-id="6e647-152">Deleted Date</span></span>
- <span data-ttu-id="6e647-153">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="6e647-153">Last Activity Date</span></span>
- <span data-ttu-id="6e647-154">ピア ツー ピア セッションの合計数</span><span class="sxs-lookup"><span data-stu-id="6e647-154">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="6e647-155">開催した会議の合計数</span><span class="sxs-lookup"><span data-stu-id="6e647-155">Total Organized Conference Count</span></span>
- <span data-ttu-id="6e647-156">参加した会議の合計数</span><span class="sxs-lookup"><span data-stu-id="6e647-156">Total Participated Conference Count</span></span>
- <span data-ttu-id="6e647-157">ピア ツー ピアの最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="6e647-157">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="6e647-158">開催した会議の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="6e647-158">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="6e647-159">参加した会議の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="6e647-159">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="6e647-160">ピア ツー ピアの IM の数</span><span class="sxs-lookup"><span data-stu-id="6e647-160">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="6e647-161">ピア ツー ピアのオーディオの数</span><span class="sxs-lookup"><span data-stu-id="6e647-161">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="6e647-162">ピア ツー ピアのオーディオの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="6e647-162">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="6e647-163">ピア ツー ピアのビデオの数</span><span class="sxs-lookup"><span data-stu-id="6e647-163">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="6e647-164">ピア ツー ピアのビデオの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="6e647-164">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="6e647-165">ピア ツー ピアのアプリ共有の数</span><span class="sxs-lookup"><span data-stu-id="6e647-165">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="6e647-166">ピア ツー ピアのファイル転送の数</span><span class="sxs-lookup"><span data-stu-id="6e647-166">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="6e647-167">開催した会議の IM の数</span><span class="sxs-lookup"><span data-stu-id="6e647-167">Organized Conference IM Count</span></span>
- <span data-ttu-id="6e647-168">開催した会議のオーディオ/ビデオの数</span><span class="sxs-lookup"><span data-stu-id="6e647-168">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="6e647-169">開催した会議のオーディオ/ビデオの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="6e647-169">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="6e647-170">開催した会議のアプリ共有の数</span><span class="sxs-lookup"><span data-stu-id="6e647-170">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="6e647-171">開催した会議の Web の数</span><span class="sxs-lookup"><span data-stu-id="6e647-171">Organized Conference Web Count</span></span>
- <span data-ttu-id="6e647-172">開催した会議のサード パーティのダイヤルイン/アウトの数</span><span class="sxs-lookup"><span data-stu-id="6e647-172">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="6e647-173">開催した会議の Microsoft のダイヤルイン/アウトの数</span><span class="sxs-lookup"><span data-stu-id="6e647-173">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="6e647-174">開催した会議の Microsoft のダイヤルインの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="6e647-174">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="6e647-175">開催した会議の Microsoft からのダイヤルアウトの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="6e647-175">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="6e647-176">参加した会議の IM の数</span><span class="sxs-lookup"><span data-stu-id="6e647-176">Participated Conference IM Count</span></span>
- <span data-ttu-id="6e647-177">参加した会議のオーディオ/ビデオの数</span><span class="sxs-lookup"><span data-stu-id="6e647-177">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="6e647-178">参加した会議のオーディオ/ビデオの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="6e647-178">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="6e647-179">参加した会議のアプリ共有の数</span><span class="sxs-lookup"><span data-stu-id="6e647-179">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="6e647-180">参加した会議の Web の数</span><span class="sxs-lookup"><span data-stu-id="6e647-180">Participated Conference Web Count</span></span>
- <span data-ttu-id="6e647-181">参加した会議のサード パーティのダイヤルイン/アウトの数</span><span class="sxs-lookup"><span data-stu-id="6e647-181">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="6e647-182">割り当て済み製品</span><span class="sxs-lookup"><span data-stu-id="6e647-182">Assigned Products</span></span>
- <span data-ttu-id="6e647-183">レポート期間</span><span class="sxs-lookup"><span data-stu-id="6e647-183">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="6e647-184">JSON</span><span class="sxs-lookup"><span data-stu-id="6e647-184">JSON</span></span>

<span data-ttu-id="6e647-185">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[Skypeforbusinessactivityuserdetail](../resources/skypeforbusinessactivityuserdetail.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6e647-185">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="6e647-186">この要求の既定のページサイズは200アイテムです。</span><span class="sxs-lookup"><span data-stu-id="6e647-186">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="6e647-187">例</span><span class="sxs-lookup"><span data-stu-id="6e647-187">Example</span></span>

### <a name="csv"></a><span data-ttu-id="6e647-188">CSV</span><span class="sxs-lookup"><span data-stu-id="6e647-188">CSV</span></span>

<span data-ttu-id="6e647-189">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6e647-189">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="6e647-190">要求</span><span class="sxs-lookup"><span data-stu-id="6e647-190">Request</span></span>

<span data-ttu-id="6e647-191">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6e647-191">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="6e647-192">応答</span><span class="sxs-lookup"><span data-stu-id="6e647-192">Response</span></span>

<span data-ttu-id="6e647-193">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6e647-193">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6e647-194">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="6e647-194">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6e647-195">Visual</span><span class="sxs-lookup"><span data-stu-id="6e647-195">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessactivityuserdetail_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6e647-196">Java</span><span class="sxs-lookup"><span data-stu-id="6e647-196">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessactivityuserdetail_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="6e647-197">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="6e647-197">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Total Peer-to-peer Session Count,Total Organized Conference Count,Total Participated Conference Count,Peer-to-peer Last Activity Date,Organized Conference Last Activity Date,Participated Conference Last Activity Date,Peer-to-peer IM Count,Peer-to-peer Audio Count,Peer-to-peer Audio Minutes,Peer-to-peer Video Count,Peer-to-peer Video Minutes,Peer-to-peer App Sharing Count,Peer-to-peer File Transfer Count,Organized Conference IM Count,Organized Conference Audio/Video Count,Organized Conference Audio/Video Minutes,Organized Conference App Sharing Count,Organized Conference Web Count,Organized Conference Dial-in/out 3rd Party Count,Organized Conference Dial-in/out Microsoft Count,Organized Conference Dial-in Microsoft Minutes,Organized Conference Dial-out Microsoft Minutes,Participated Conference IM Count,Participated Conference Audio/Video Count,Participated Conference Audio/Video Minutes,Participated Conference App Sharing Count,Participated Conference Web Count,Participated Conference Dial-in/out 3rd Party Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="6e647-198">JSON</span><span class="sxs-lookup"><span data-stu-id="6e647-198">JSON</span></span>

<span data-ttu-id="6e647-199">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="6e647-199">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="6e647-200">要求</span><span class="sxs-lookup"><span data-stu-id="6e647-200">Request</span></span>

<span data-ttu-id="6e647-201">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6e647-201">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="6e647-202">応答</span><span class="sxs-lookup"><span data-stu-id="6e647-202">Response</span></span>

<span data-ttu-id="6e647-203">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6e647-203">The following is an example of the response.</span></span>

> <span data-ttu-id="6e647-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6e647-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1419

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessActivityUserDetail)", 
  "value": [
    {
      "totalPeerToPeerSessionCount": 12, 
      "totalOrganizedConferenceCount": 0, 
      "totalParticipatedConferenceCount": 1, 
      "peerToPeerLastActivityDate": "2017-09-01", 
      "organizedConferenceLastActivityDate": null, 
      "participatedConferenceLastActivityDate": "2017-08-31", 
      "peerToPeerIMCount": 12, 
      "peerToPeerAudioCount": 0, 
      "peerToPeerAudioMinutes": 0, 
      "peerToPeerVideoCount": 0, 
      "peerToPeerVideoMinutes": 0, 
      "peerToPeerAppSharingCount": 0, 
      "peerToPeerFileTransferCount": 0, 
      "organizedConferenceIMCount": 0, 
      "organizedConferenceAudioVideoCount": 0, 
      "organizedConferenceAudioVideoMinutes": 0, 
      "organizedConferenceAppSharingCount": 0, 
      "organizedConferenceWebCount": 0, 
      "organizedConferenceDialInOut3rdPartyCount": 0, 
      "organizedConferenceCloudDialInOutMicrosoftCount": 0, 
      "organizedConferenceCloudDialInMicrosoftMinutes": 0, 
      "organizedConferenceCloudDialOutMicrosoftMinutes": 0, 
      "participatedConferenceIMCount": 0, 
      "participatedConferenceAudioVideoCount": 1, 
      "participatedConferenceAudioVideoMinutes": 69, 
      "participatedConferenceAppSharingCount": 0, 
      "participatedConferenceWebCount": 0, 
      "participatedConferenceDialInOut3rdPartyCount": 0, 
      "reportRefreshDate": "2017-09-06", 
      "userPrincipalName": "userPrincipalName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5", 
      ], 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6e647-206">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="6e647-206">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6e647-207">Visual</span><span class="sxs-lookup"><span data-stu-id="6e647-207">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessactivityuserdetail_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6e647-208">Java</span><span class="sxs-lookup"><span data-stu-id="6e647-208">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessactivityuserdetail_json-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
