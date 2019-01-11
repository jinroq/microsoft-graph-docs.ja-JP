---
title: 'reportRoot: getSkypeForBusinessActivityUserDetail'
description: ユーザー別の Skype for Business アクティビティに関する詳細を取得します。
localization_priority: Normal
ms.openlocfilehash: 43bf2d7f08bc9a0033bd04f98687c7d03be5f2ea
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872633"
---
# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="a129c-103">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="a129c-103">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

> <span data-ttu-id="a129c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a129c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a129c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a129c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a129c-106">ユーザー別の Skype for Business アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="a129c-106">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="a129c-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business アクティビティ](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a129c-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="a129c-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a129c-108">Permissions</span></span>

<span data-ttu-id="a129c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a129c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a129c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a129c-111">Permission type</span></span>                        | <span data-ttu-id="a129c-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a129c-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a129c-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="a129c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="a129c-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a129c-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a129c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a129c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a129c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a129c-116">Not supported.</span></span>                           |
| <span data-ttu-id="a129c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a129c-117">Application</span></span>                            | <span data-ttu-id="a129c-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a129c-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a129c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a129c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="a129c-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="a129c-120">Function parameters</span></span>

<span data-ttu-id="a129c-121">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="a129c-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="a129c-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="a129c-122">Parameter</span></span> | <span data-ttu-id="a129c-123">Type</span><span class="sxs-lookup"><span data-stu-id="a129c-123">Type</span></span>   | <span data-ttu-id="a129c-124">説明</span><span class="sxs-lookup"><span data-stu-id="a129c-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a129c-125">period</span><span class="sxs-lookup"><span data-stu-id="a129c-125">period</span></span>    | <span data-ttu-id="a129c-126">文字列</span><span class="sxs-lookup"><span data-stu-id="a129c-126">string</span></span> | <span data-ttu-id="a129c-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="a129c-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a129c-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="a129c-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a129c-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="a129c-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="a129c-130">date</span><span class="sxs-lookup"><span data-stu-id="a129c-130">date</span></span>      | <span data-ttu-id="a129c-131">日付</span><span class="sxs-lookup"><span data-stu-id="a129c-131">Date</span></span>   | <span data-ttu-id="a129c-132">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="a129c-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="a129c-133">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="a129c-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="a129c-134">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="a129c-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="a129c-135">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a129c-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="a129c-136">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a129c-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a129c-137">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="a129c-137">The default output type is text/csv.</span></span> <span data-ttu-id="a129c-138">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="a129c-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a129c-139">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a129c-139">Request headers</span></span>

| <span data-ttu-id="a129c-140">名前</span><span class="sxs-lookup"><span data-stu-id="a129c-140">Name</span></span>          | <span data-ttu-id="a129c-141">説明</span><span class="sxs-lookup"><span data-stu-id="a129c-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a129c-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="a129c-142">Authorization</span></span> | <span data-ttu-id="a129c-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a129c-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a129c-145">応答</span><span class="sxs-lookup"><span data-stu-id="a129c-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a129c-146">CSV</span><span class="sxs-lookup"><span data-stu-id="a129c-146">CSV</span></span>

<span data-ttu-id="a129c-147">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="a129c-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a129c-148">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="a129c-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a129c-149">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="a129c-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a129c-150">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="a129c-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a129c-151">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="a129c-151">Report Refresh Date</span></span>
- <span data-ttu-id="a129c-152">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="a129c-152">User Principal Name</span></span>
- <span data-ttu-id="a129c-153">削除済み</span><span class="sxs-lookup"><span data-stu-id="a129c-153">Is Deleted</span></span>
- <span data-ttu-id="a129c-154">削除日</span><span class="sxs-lookup"><span data-stu-id="a129c-154">Deleted Date</span></span>
- <span data-ttu-id="a129c-155">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="a129c-155">Last Activity Date</span></span>
- <span data-ttu-id="a129c-156">ピア ツー ピア セッションの合計数</span><span class="sxs-lookup"><span data-stu-id="a129c-156">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="a129c-157">開催した会議の合計数</span><span class="sxs-lookup"><span data-stu-id="a129c-157">Total Organized Conference Count</span></span>
- <span data-ttu-id="a129c-158">参加した会議の合計数</span><span class="sxs-lookup"><span data-stu-id="a129c-158">Total Participated Conference Count</span></span>
- <span data-ttu-id="a129c-159">ピア ツー ピアの最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="a129c-159">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="a129c-160">開催した会議の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="a129c-160">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="a129c-161">参加した会議の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="a129c-161">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="a129c-162">ピア ツー ピアの IM の数</span><span class="sxs-lookup"><span data-stu-id="a129c-162">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="a129c-163">ピア ツー ピアのオーディオの数</span><span class="sxs-lookup"><span data-stu-id="a129c-163">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="a129c-164">ピア ツー ピアのオーディオの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="a129c-164">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="a129c-165">ピア ツー ピアのビデオの数</span><span class="sxs-lookup"><span data-stu-id="a129c-165">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="a129c-166">ピア ツー ピアのビデオの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="a129c-166">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="a129c-167">ピア ツー ピアのアプリ共有の数</span><span class="sxs-lookup"><span data-stu-id="a129c-167">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="a129c-168">ピア ツー ピアのファイル転送の数</span><span class="sxs-lookup"><span data-stu-id="a129c-168">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="a129c-169">開催した会議の IM の数</span><span class="sxs-lookup"><span data-stu-id="a129c-169">Organized Conference IM Count</span></span>
- <span data-ttu-id="a129c-170">開催した会議のオーディオ/ビデオの数</span><span class="sxs-lookup"><span data-stu-id="a129c-170">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="a129c-171">開催した会議のオーディオ/ビデオの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="a129c-171">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="a129c-172">開催した会議のアプリ共有の数</span><span class="sxs-lookup"><span data-stu-id="a129c-172">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="a129c-173">開催した会議の Web の数</span><span class="sxs-lookup"><span data-stu-id="a129c-173">Organized Conference Web Count</span></span>
- <span data-ttu-id="a129c-174">開催した会議のサード パーティのダイヤルイン/アウトの数</span><span class="sxs-lookup"><span data-stu-id="a129c-174">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="a129c-175">開催した会議の Microsoft のダイヤルイン/アウトの数</span><span class="sxs-lookup"><span data-stu-id="a129c-175">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="a129c-176">開催した会議の Microsoft のダイヤルインの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="a129c-176">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="a129c-177">開催した会議の Microsoft からのダイヤルアウトの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="a129c-177">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="a129c-178">会議の参加した IM の数</span><span class="sxs-lookup"><span data-stu-id="a129c-178">Participated Conference IM Count</span></span>
- <span data-ttu-id="a129c-179">参加した会議のオーディオ/ビデオの数</span><span class="sxs-lookup"><span data-stu-id="a129c-179">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="a129c-180">参加した会議のオーディオ/ビデオの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="a129c-180">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="a129c-181">参加した会議のアプリ共有の数</span><span class="sxs-lookup"><span data-stu-id="a129c-181">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="a129c-182">参加した会議の Web の数</span><span class="sxs-lookup"><span data-stu-id="a129c-182">Participated Conference Web Count</span></span>
- <span data-ttu-id="a129c-183">参加した会議のサード パーティのダイヤルイン/アウトの数</span><span class="sxs-lookup"><span data-stu-id="a129c-183">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="a129c-184">割り当て済み製品</span><span class="sxs-lookup"><span data-stu-id="a129c-184">Assigned Products</span></span>
- <span data-ttu-id="a129c-185">レポート期間</span><span class="sxs-lookup"><span data-stu-id="a129c-185">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="a129c-186">JSON</span><span class="sxs-lookup"><span data-stu-id="a129c-186">JSON</span></span>

<span data-ttu-id="a129c-187">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a129c-187">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="a129c-188">この要求の既定のページ サイズは、アイテムは 200 個です。</span><span class="sxs-lookup"><span data-stu-id="a129c-188">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="a129c-189">例</span><span class="sxs-lookup"><span data-stu-id="a129c-189">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a129c-190">CSV</span><span class="sxs-lookup"><span data-stu-id="a129c-190">CSV</span></span>

<span data-ttu-id="a129c-191">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="a129c-191">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a129c-192">要求</span><span class="sxs-lookup"><span data-stu-id="a129c-192">Request</span></span>

<span data-ttu-id="a129c-193">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a129c-193">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="a129c-194">応答</span><span class="sxs-lookup"><span data-stu-id="a129c-194">Response</span></span>

<span data-ttu-id="a129c-195">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a129c-195">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a129c-196">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="a129c-196">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="a129c-197">JSON</span><span class="sxs-lookup"><span data-stu-id="a129c-197">JSON</span></span>

<span data-ttu-id="a129c-198">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="a129c-198">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a129c-199">要求</span><span class="sxs-lookup"><span data-stu-id="a129c-199">Request</span></span>

<span data-ttu-id="a129c-200">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a129c-200">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="a129c-201">応答</span><span class="sxs-lookup"><span data-stu-id="a129c-201">Response</span></span>

<span data-ttu-id="a129c-202">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a129c-202">The following is an example of the response.</span></span>

> <span data-ttu-id="a129c-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a129c-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
