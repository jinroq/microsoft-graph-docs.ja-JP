---
title: 'reportRoot: getSkypeForBusinessActivityUserDetail'
description: ユーザー別の Skype for Business アクティビティに関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 015a876a49d8c404c82dd392062ed77777bb8020
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872496"
---
# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="44ab5-103">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="44ab5-103">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44ab5-104">ユーザー別の Skype for Business アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="44ab5-104">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="44ab5-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business アクティビティ](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44ab5-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="44ab5-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="44ab5-106">Permissions</span></span>

<span data-ttu-id="44ab5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44ab5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="44ab5-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="44ab5-109">Permission type</span></span>                        | <span data-ttu-id="44ab5-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="44ab5-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="44ab5-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="44ab5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="44ab5-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="44ab5-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="44ab5-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="44ab5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44ab5-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44ab5-114">Not supported.</span></span>                           |
| <span data-ttu-id="44ab5-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="44ab5-115">Application</span></span>                            | <span data-ttu-id="44ab5-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="44ab5-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="44ab5-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="44ab5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="44ab5-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="44ab5-118">Function parameters</span></span>

<span data-ttu-id="44ab5-119">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="44ab5-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="44ab5-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="44ab5-120">Parameter</span></span> | <span data-ttu-id="44ab5-121">型</span><span class="sxs-lookup"><span data-stu-id="44ab5-121">Type</span></span>   | <span data-ttu-id="44ab5-122">説明</span><span class="sxs-lookup"><span data-stu-id="44ab5-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="44ab5-123">period</span><span class="sxs-lookup"><span data-stu-id="44ab5-123">period</span></span>    | <span data-ttu-id="44ab5-124">文字列</span><span class="sxs-lookup"><span data-stu-id="44ab5-124">string</span></span> | <span data-ttu-id="44ab5-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="44ab5-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="44ab5-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="44ab5-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="44ab5-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="44ab5-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="44ab5-128">date</span><span class="sxs-lookup"><span data-stu-id="44ab5-128">date</span></span>      | <span data-ttu-id="44ab5-129">日付</span><span class="sxs-lookup"><span data-stu-id="44ab5-129">Date</span></span>   | <span data-ttu-id="44ab5-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="44ab5-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="44ab5-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="44ab5-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="44ab5-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="44ab5-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="44ab5-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="44ab5-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="44ab5-134">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="44ab5-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="44ab5-135">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="44ab5-135">The default output type is text/csv.</span></span> <span data-ttu-id="44ab5-136">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="44ab5-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="44ab5-137">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="44ab5-137">Request headers</span></span>

| <span data-ttu-id="44ab5-138">名前</span><span class="sxs-lookup"><span data-stu-id="44ab5-138">Name</span></span>          | <span data-ttu-id="44ab5-139">説明</span><span class="sxs-lookup"><span data-stu-id="44ab5-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="44ab5-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="44ab5-140">Authorization</span></span> | <span data-ttu-id="44ab5-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="44ab5-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="44ab5-143">応答</span><span class="sxs-lookup"><span data-stu-id="44ab5-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="44ab5-144">CSV</span><span class="sxs-lookup"><span data-stu-id="44ab5-144">CSV</span></span>

<span data-ttu-id="44ab5-145">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="44ab5-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="44ab5-146">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="44ab5-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="44ab5-147">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="44ab5-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="44ab5-148">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="44ab5-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="44ab5-149">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="44ab5-149">Report Refresh Date</span></span>
- <span data-ttu-id="44ab5-150">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="44ab5-150">User Principal Name</span></span>
- <span data-ttu-id="44ab5-151">削除済み</span><span class="sxs-lookup"><span data-stu-id="44ab5-151">Is Deleted</span></span>
- <span data-ttu-id="44ab5-152">削除日</span><span class="sxs-lookup"><span data-stu-id="44ab5-152">Deleted Date</span></span>
- <span data-ttu-id="44ab5-153">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="44ab5-153">Last Activity Date</span></span>
- <span data-ttu-id="44ab5-154">ピア ツー ピア セッションの合計数</span><span class="sxs-lookup"><span data-stu-id="44ab5-154">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="44ab5-155">開催した会議の合計数</span><span class="sxs-lookup"><span data-stu-id="44ab5-155">Total Organized Conference Count</span></span>
- <span data-ttu-id="44ab5-156">参加した会議の合計数</span><span class="sxs-lookup"><span data-stu-id="44ab5-156">Total Participated Conference Count</span></span>
- <span data-ttu-id="44ab5-157">ピア ツー ピアの最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="44ab5-157">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="44ab5-158">開催した会議の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="44ab5-158">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="44ab5-159">参加した会議の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="44ab5-159">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="44ab5-160">ピア ツー ピアの IM の数</span><span class="sxs-lookup"><span data-stu-id="44ab5-160">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="44ab5-161">ピア ツー ピアのオーディオの数</span><span class="sxs-lookup"><span data-stu-id="44ab5-161">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="44ab5-162">ピア ツー ピアのオーディオの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="44ab5-162">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="44ab5-163">ピア ツー ピアのビデオの数</span><span class="sxs-lookup"><span data-stu-id="44ab5-163">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="44ab5-164">ピア ツー ピアのビデオの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="44ab5-164">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="44ab5-165">ピア ツー ピアのアプリ共有の数</span><span class="sxs-lookup"><span data-stu-id="44ab5-165">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="44ab5-166">ピア ツー ピアのファイル転送の数</span><span class="sxs-lookup"><span data-stu-id="44ab5-166">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="44ab5-167">開催した会議の IM の数</span><span class="sxs-lookup"><span data-stu-id="44ab5-167">Organized Conference IM Count</span></span>
- <span data-ttu-id="44ab5-168">開催した会議のオーディオ/ビデオの数</span><span class="sxs-lookup"><span data-stu-id="44ab5-168">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="44ab5-169">開催した会議のオーディオ/ビデオの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="44ab5-169">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="44ab5-170">開催した会議のアプリ共有の数</span><span class="sxs-lookup"><span data-stu-id="44ab5-170">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="44ab5-171">開催した会議の Web の数</span><span class="sxs-lookup"><span data-stu-id="44ab5-171">Organized Conference Web Count</span></span>
- <span data-ttu-id="44ab5-172">開催した会議のサード パーティのダイヤルイン/アウトの数</span><span class="sxs-lookup"><span data-stu-id="44ab5-172">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="44ab5-173">開催した会議の Microsoft のダイヤルイン/アウトの数</span><span class="sxs-lookup"><span data-stu-id="44ab5-173">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="44ab5-174">開催した会議の Microsoft のダイヤルインの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="44ab5-174">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="44ab5-175">開催した会議の Microsoft からのダイヤルアウトの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="44ab5-175">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="44ab5-176">参加した会議の IM の数</span><span class="sxs-lookup"><span data-stu-id="44ab5-176">Participated Conference IM Count</span></span>
- <span data-ttu-id="44ab5-177">参加した会議のオーディオ/ビデオの数</span><span class="sxs-lookup"><span data-stu-id="44ab5-177">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="44ab5-178">参加した会議のオーディオ/ビデオの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="44ab5-178">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="44ab5-179">参加した会議のアプリ共有の数</span><span class="sxs-lookup"><span data-stu-id="44ab5-179">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="44ab5-180">参加した会議の Web の数</span><span class="sxs-lookup"><span data-stu-id="44ab5-180">Participated Conference Web Count</span></span>
- <span data-ttu-id="44ab5-181">参加した会議のサード パーティのダイヤルイン/アウトの数</span><span class="sxs-lookup"><span data-stu-id="44ab5-181">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="44ab5-182">割り当て済み製品</span><span class="sxs-lookup"><span data-stu-id="44ab5-182">Assigned Products</span></span>
- <span data-ttu-id="44ab5-183">レポート期間</span><span class="sxs-lookup"><span data-stu-id="44ab5-183">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="44ab5-184">JSON</span><span class="sxs-lookup"><span data-stu-id="44ab5-184">JSON</span></span>

<span data-ttu-id="44ab5-185">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[Skypeforbusinessactivityuserdetail](../resources/skypeforbusinessactivityuserdetail.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="44ab5-185">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="44ab5-186">この要求の既定のページサイズは200アイテムです。</span><span class="sxs-lookup"><span data-stu-id="44ab5-186">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="44ab5-187">例</span><span class="sxs-lookup"><span data-stu-id="44ab5-187">Example</span></span>

### <a name="csv"></a><span data-ttu-id="44ab5-188">CSV</span><span class="sxs-lookup"><span data-stu-id="44ab5-188">CSV</span></span>

<span data-ttu-id="44ab5-189">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="44ab5-189">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="44ab5-190">要求</span><span class="sxs-lookup"><span data-stu-id="44ab5-190">Request</span></span>

<span data-ttu-id="44ab5-191">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="44ab5-191">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="44ab5-192">プロトコル</span><span class="sxs-lookup"><span data-stu-id="44ab5-192">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="44ab5-193">C#</span><span class="sxs-lookup"><span data-stu-id="44ab5-193">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessactivityuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="44ab5-194">Javascript</span><span class="sxs-lookup"><span data-stu-id="44ab5-194">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessactivityuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="44ab5-195">目的-C</span><span class="sxs-lookup"><span data-stu-id="44ab5-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessactivityuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="44ab5-196">Java</span><span class="sxs-lookup"><span data-stu-id="44ab5-196">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessactivityuserdetail-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="44ab5-197">応答</span><span class="sxs-lookup"><span data-stu-id="44ab5-197">Response</span></span>

<span data-ttu-id="44ab5-198">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="44ab5-198">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="44ab5-199">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="44ab5-199">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="44ab5-200">JSON</span><span class="sxs-lookup"><span data-stu-id="44ab5-200">JSON</span></span>

<span data-ttu-id="44ab5-201">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="44ab5-201">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="44ab5-202">要求</span><span class="sxs-lookup"><span data-stu-id="44ab5-202">Request</span></span>

<span data-ttu-id="44ab5-203">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="44ab5-203">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="44ab5-204">プロトコル</span><span class="sxs-lookup"><span data-stu-id="44ab5-204">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="44ab5-205">C#</span><span class="sxs-lookup"><span data-stu-id="44ab5-205">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessactivityuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="44ab5-206">Javascript</span><span class="sxs-lookup"><span data-stu-id="44ab5-206">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessactivityuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="44ab5-207">目的-C</span><span class="sxs-lookup"><span data-stu-id="44ab5-207">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessactivityuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="44ab5-208">Java</span><span class="sxs-lookup"><span data-stu-id="44ab5-208">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessactivityuserdetail-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="44ab5-209">応答</span><span class="sxs-lookup"><span data-stu-id="44ab5-209">Response</span></span>

<span data-ttu-id="44ab5-210">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="44ab5-210">The following is an example of the response.</span></span>

> <span data-ttu-id="44ab5-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="44ab5-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
