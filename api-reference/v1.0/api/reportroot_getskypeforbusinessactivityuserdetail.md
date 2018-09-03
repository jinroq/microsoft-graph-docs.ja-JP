# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="ca065-101">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="ca065-101">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

<span data-ttu-id="ca065-102">ユーザー別の Skype for Business アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="ca065-102">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="ca065-103">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business アクティビティ](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ca065-103">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="ca065-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ca065-104">Permissions</span></span>

<span data-ttu-id="ca065-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ca065-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="ca065-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ca065-107">Permission type</span></span>                        | <span data-ttu-id="ca065-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ca065-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ca065-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="ca065-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="ca065-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca065-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ca065-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ca065-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca065-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca065-112">Not supported.</span></span>                           |
| <span data-ttu-id="ca065-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ca065-113">Application</span></span>                            | <span data-ttu-id="ca065-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca065-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ca065-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ca065-115">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="ca065-116">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="ca065-116">Function parameters</span></span>

<span data-ttu-id="ca065-117">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="ca065-117">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="ca065-118">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ca065-118">Parameter</span></span> | <span data-ttu-id="ca065-119">型</span><span class="sxs-lookup"><span data-stu-id="ca065-119">Type</span></span>   | <span data-ttu-id="ca065-120">説明</span><span class="sxs-lookup"><span data-stu-id="ca065-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ca065-121">期間</span><span class="sxs-lookup"><span data-stu-id="ca065-121">period</span></span>    | <span data-ttu-id="ca065-122">文字列</span><span class="sxs-lookup"><span data-stu-id="ca065-122">string</span></span> | <span data-ttu-id="ca065-123">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="ca065-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ca065-124">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="ca065-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ca065-125">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="ca065-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="ca065-126">日付</span><span class="sxs-lookup"><span data-stu-id="ca065-126">date</span></span>      | <span data-ttu-id="ca065-127">日付</span><span class="sxs-lookup"><span data-stu-id="ca065-127">Date</span></span>   | <span data-ttu-id="ca065-128">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="ca065-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="ca065-129">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="ca065-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="ca065-130">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="ca065-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="ca065-131">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ca065-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ca065-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ca065-132">Request headers</span></span>

| <span data-ttu-id="ca065-133">名前</span><span class="sxs-lookup"><span data-stu-id="ca065-133">Name</span></span>          | <span data-ttu-id="ca065-134">説明</span><span class="sxs-lookup"><span data-stu-id="ca065-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="ca065-135">承認</span><span class="sxs-lookup"><span data-stu-id="ca065-135">Authorization</span></span> | <span data-ttu-id="ca065-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ca065-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="ca065-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="ca065-138">If-None-Match</span></span> | <span data-ttu-id="ca065-139">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="ca065-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="ca065-140">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ca065-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="ca065-141">応答</span><span class="sxs-lookup"><span data-stu-id="ca065-141">Response</span></span>

<span data-ttu-id="ca065-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="ca065-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ca065-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="ca065-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ca065-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="ca065-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ca065-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="ca065-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ca065-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="ca065-146">Report Refresh Date</span></span>
- <span data-ttu-id="ca065-147">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="ca065-147">User Principal Name</span></span>
- <span data-ttu-id="ca065-148">削除済み</span><span class="sxs-lookup"><span data-stu-id="ca065-148">Is Deleted</span></span>
- <span data-ttu-id="ca065-149">削除日</span><span class="sxs-lookup"><span data-stu-id="ca065-149">Deleted Date</span></span>
- <span data-ttu-id="ca065-150">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="ca065-150">Last Activity Date</span></span>
- <span data-ttu-id="ca065-151">ピア ツー ピア セッションの合計数</span><span class="sxs-lookup"><span data-stu-id="ca065-151">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="ca065-152">開催した会議の合計数</span><span class="sxs-lookup"><span data-stu-id="ca065-152">Total Organized Conference Count</span></span>
- <span data-ttu-id="ca065-153">参加した会議の合計数</span><span class="sxs-lookup"><span data-stu-id="ca065-153">Total Participated Conference Count</span></span>
- <span data-ttu-id="ca065-154">ピア ツー ピアの最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="ca065-154">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="ca065-155">開催した会議の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="ca065-155">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="ca065-156">参加した会議の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="ca065-156">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="ca065-157">ピア ツー ピアの IM の数</span><span class="sxs-lookup"><span data-stu-id="ca065-157">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="ca065-158">ピア ツー ピアのオーディオの数</span><span class="sxs-lookup"><span data-stu-id="ca065-158">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="ca065-159">ピア ツー ピアのオーディオの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="ca065-159">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="ca065-160">ピア ツー ピアのビデオの数</span><span class="sxs-lookup"><span data-stu-id="ca065-160">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="ca065-161">ピア ツー ピアのビデオの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="ca065-161">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="ca065-162">ピア ツー ピアのアプリ共有の数</span><span class="sxs-lookup"><span data-stu-id="ca065-162">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="ca065-163">ピア ツー ピアのファイル転送の数</span><span class="sxs-lookup"><span data-stu-id="ca065-163">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="ca065-164">開催した会議の IM の数</span><span class="sxs-lookup"><span data-stu-id="ca065-164">Organized Conference IM Count</span></span>
- <span data-ttu-id="ca065-165">開催した会議のオーディオ/ビデオの数</span><span class="sxs-lookup"><span data-stu-id="ca065-165">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="ca065-166">開催した会議のオーディオ/ビデオの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="ca065-166">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="ca065-167">開催した会議のアプリ共有の数</span><span class="sxs-lookup"><span data-stu-id="ca065-167">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="ca065-168">開催した会議の Web の数</span><span class="sxs-lookup"><span data-stu-id="ca065-168">Organized Conference Web Count</span></span>
- <span data-ttu-id="ca065-169">開催した会議のサード パーティのダイヤルイン/アウトの数</span><span class="sxs-lookup"><span data-stu-id="ca065-169">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="ca065-170">開催した会議の Microsoft のダイヤルイン/アウトの数</span><span class="sxs-lookup"><span data-stu-id="ca065-170">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="ca065-171">開催した会議の Microsoft のダイヤルインの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="ca065-171">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="ca065-172">開催した会議の Microsoft からのダイヤルアウトの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="ca065-172">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="ca065-173">参加した会議の IM の数</span><span class="sxs-lookup"><span data-stu-id="ca065-173">Paricipated Conference IM Count</span></span>
- <span data-ttu-id="ca065-174">参加した会議のオーディオ/ビデオの数</span><span class="sxs-lookup"><span data-stu-id="ca065-174">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="ca065-175">参加した会議のオーディオ/ビデオの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="ca065-175">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="ca065-176">参加した会議のアプリ共有の数</span><span class="sxs-lookup"><span data-stu-id="ca065-176">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="ca065-177">参加した会議の Web の数</span><span class="sxs-lookup"><span data-stu-id="ca065-177">Participated Conference Web Count</span></span>
- <span data-ttu-id="ca065-178">参加した会議のサード パーティのダイヤルイン/アウトの数</span><span class="sxs-lookup"><span data-stu-id="ca065-178">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="ca065-179">割り当て済み製品</span><span class="sxs-lookup"><span data-stu-id="ca065-179">Assigned Products</span></span>
- <span data-ttu-id="ca065-180">レポート期間</span><span class="sxs-lookup"><span data-stu-id="ca065-180">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="ca065-181">例</span><span class="sxs-lookup"><span data-stu-id="ca065-181">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ca065-182">要求</span><span class="sxs-lookup"><span data-stu-id="ca065-182">Request</span></span>

<span data-ttu-id="ca065-183">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ca065-183">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="ca065-184">応答</span><span class="sxs-lookup"><span data-stu-id="ca065-184">Response</span></span>

<span data-ttu-id="ca065-185">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ca065-185">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="ca065-186">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="ca065-186">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Total Peer-to-peer Session Count,Total Organized Conference Count,Total Participated Conference Count,Peer-to-peer Last Activity Date,Organized Conference Last Activity Date,Participated Conference Last Activity Date,Peer-to-peer IM Count,Peer-to-peer Audio Count,Peer-to-peer Audio Minutes,Peer-to-peer Video Count,Peer-to-peer Video Minutes,Peer-to-peer App Sharing Count,Peer-to-peer File Transfer Count,Organized Conference IM Count,Organized Conference Audio/Video Count,Organized Conference Audio/Video Minutes,Organized Conference App Sharing Count,Organized Conference Web Count,Organized Conference Dial-in/out 3rd Party Count,Organized Conference Dial-in/out Microsoft Count,Organized Conference Dial-in Microsoft Minutes,Organized Conference Dial-out Microsoft Minutes,Paricipated Conference IM Count,Participated Conference Audio/Video Count,Participated Conference Audio/Video Minutes,Participated Conference App Sharing Count,Participated Conference Web Count,Participated Conference Dial-in/out 3rd Party Count,Assigned Products,Report Period
```
