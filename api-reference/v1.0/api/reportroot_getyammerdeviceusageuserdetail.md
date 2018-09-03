# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="43f0d-101">reportRoot: getYammerDeviceUsageUserDetail 関数</span><span class="sxs-lookup"><span data-stu-id="43f0d-101">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

<span data-ttu-id="43f0d-102">ユーザー別の Yammer デバイス使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="43f0d-102">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="43f0d-103">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer デバイスの使用状況](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="43f0d-103">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="43f0d-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="43f0d-104">Permissions</span></span>

<span data-ttu-id="43f0d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="43f0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="43f0d-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="43f0d-107">Permission type</span></span>                        | <span data-ttu-id="43f0d-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="43f0d-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="43f0d-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="43f0d-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="43f0d-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="43f0d-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="43f0d-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="43f0d-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43f0d-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43f0d-112">Not supported.</span></span>                           |
| <span data-ttu-id="43f0d-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="43f0d-113">Application</span></span>                            | <span data-ttu-id="43f0d-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="43f0d-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="43f0d-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="43f0d-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="43f0d-116">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="43f0d-116">Function parameters</span></span>

<span data-ttu-id="43f0d-117">要求 URL に、クエリ パラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="43f0d-117">In the request URL, provide the query parameter with a valid value.</span></span>

| <span data-ttu-id="43f0d-118">パラメーター</span><span class="sxs-lookup"><span data-stu-id="43f0d-118">Parameter</span></span> | <span data-ttu-id="43f0d-119">型</span><span class="sxs-lookup"><span data-stu-id="43f0d-119">Type</span></span>   | <span data-ttu-id="43f0d-120">説明</span><span class="sxs-lookup"><span data-stu-id="43f0d-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="43f0d-121">期間</span><span class="sxs-lookup"><span data-stu-id="43f0d-121">period</span></span>    | <span data-ttu-id="43f0d-122">文字列</span><span class="sxs-lookup"><span data-stu-id="43f0d-122">string</span></span> | <span data-ttu-id="43f0d-123">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="43f0d-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="43f0d-124">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="43f0d-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="43f0d-125">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="43f0d-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="43f0d-126">日付</span><span class="sxs-lookup"><span data-stu-id="43f0d-126">date</span></span>      | <span data-ttu-id="43f0d-127">日付</span><span class="sxs-lookup"><span data-stu-id="43f0d-127">Date</span></span>   | <span data-ttu-id="43f0d-128">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="43f0d-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="43f0d-129">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="43f0d-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="43f0d-130">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="43f0d-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="43f0d-131">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="43f0d-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="43f0d-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="43f0d-132">Request headers</span></span>

| <span data-ttu-id="43f0d-133">名前</span><span class="sxs-lookup"><span data-stu-id="43f0d-133">Name</span></span>          | <span data-ttu-id="43f0d-134">説明</span><span class="sxs-lookup"><span data-stu-id="43f0d-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="43f0d-135">承認</span><span class="sxs-lookup"><span data-stu-id="43f0d-135">Authorization</span></span> | <span data-ttu-id="43f0d-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="43f0d-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="43f0d-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="43f0d-138">If-None-Match</span></span> | <span data-ttu-id="43f0d-139">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="43f0d-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="43f0d-140">省略可能。</span><span class="sxs-lookup"><span data-stu-id="43f0d-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="43f0d-141">応答</span><span class="sxs-lookup"><span data-stu-id="43f0d-141">Response</span></span>

<span data-ttu-id="43f0d-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="43f0d-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="43f0d-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="43f0d-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="43f0d-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="43f0d-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="43f0d-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="43f0d-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="43f0d-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="43f0d-146">Report Refresh Date</span></span>
- <span data-ttu-id="43f0d-147">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="43f0d-147">User Principal Name</span></span>
- <span data-ttu-id="43f0d-148">表示名</span><span class="sxs-lookup"><span data-stu-id="43f0d-148">Display Name</span></span>
- <span data-ttu-id="43f0d-149">ユーザーの状態</span><span class="sxs-lookup"><span data-stu-id="43f0d-149">User State</span></span>
- <span data-ttu-id="43f0d-150">状態変更日付</span><span class="sxs-lookup"><span data-stu-id="43f0d-150">State Change Date</span></span>
- <span data-ttu-id="43f0d-151">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="43f0d-151">Last Activity Date</span></span>
- <span data-ttu-id="43f0d-152">Web の使用</span><span class="sxs-lookup"><span data-stu-id="43f0d-152">Used Web</span></span>
- <span data-ttu-id="43f0d-153">Windows スマートフォンの使用</span><span class="sxs-lookup"><span data-stu-id="43f0d-153">Used Windows Phone</span></span>
- <span data-ttu-id="43f0d-154">Android スマートフォンの使用</span><span class="sxs-lookup"><span data-stu-id="43f0d-154">Used Android Phone</span></span>
- <span data-ttu-id="43f0d-155">iPhone の使用</span><span class="sxs-lookup"><span data-stu-id="43f0d-155">Used iPhone</span></span>
- <span data-ttu-id="43f0d-156">IPad の使用</span><span class="sxs-lookup"><span data-stu-id="43f0d-156">Used iPad</span></span>
- <span data-ttu-id="43f0d-157">その他の使用</span><span class="sxs-lookup"><span data-stu-id="43f0d-157">Used Others</span></span>
- <span data-ttu-id="43f0d-158">レポート期間</span><span class="sxs-lookup"><span data-stu-id="43f0d-158">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="43f0d-159">例</span><span class="sxs-lookup"><span data-stu-id="43f0d-159">Example</span></span>

#### <a name="request"></a><span data-ttu-id="43f0d-160">要求</span><span class="sxs-lookup"><span data-stu-id="43f0d-160">Request</span></span>

<span data-ttu-id="43f0d-161">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="43f0d-161">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="43f0d-162">応答</span><span class="sxs-lookup"><span data-stu-id="43f0d-162">Response</span></span>

<span data-ttu-id="43f0d-163">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="43f0d-163">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="43f0d-164">要求</span><span class="sxs-lookup"><span data-stu-id="43f0d-164">Request</span></span>

<span data-ttu-id="43f0d-165">パラメーターで呼び出した場合、レポートの使用は特定の日に制限されます。`date`</span><span class="sxs-lookup"><span data-stu-id="43f0d-165">If called with the `date` parameter, the report is scoped to usage on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="43f0d-166">応答</span><span class="sxs-lookup"><span data-stu-id="43f0d-166">Response</span></span>

<span data-ttu-id="43f0d-167">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="43f0d-167">The following is an example of the response.</span></span>

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

<span data-ttu-id="43f0d-168">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="43f0d-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Used Web,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Used Others,Report Period
```
