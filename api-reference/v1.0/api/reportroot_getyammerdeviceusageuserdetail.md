# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="66b39-101">reportRoot: getYammerDeviceUsageUserDetail function</span><span class="sxs-lookup"><span data-stu-id="66b39-101">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

<span data-ttu-id="66b39-102">ユーザー別の Yammer デバイス使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="66b39-102">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="66b39-103">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer デバイスの使用状況]((https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38))」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="66b39-103">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage]((https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)).</span></span>

## <a name="permissions"></a><span data-ttu-id="66b39-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="66b39-104">Permissions</span></span>

<span data-ttu-id="66b39-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="66b39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="66b39-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="66b39-107">Permission type</span></span>                        | <span data-ttu-id="66b39-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="66b39-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="66b39-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="66b39-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="66b39-110">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66b39-110">Not supported.</span></span>                           |
| <span data-ttu-id="66b39-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="66b39-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66b39-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66b39-112">Not supported.</span></span>                           |
| <span data-ttu-id="66b39-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="66b39-113">Application</span></span>                            | <span data-ttu-id="66b39-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="66b39-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="66b39-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="66b39-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="66b39-116">要求パラメーター</span><span class="sxs-lookup"><span data-stu-id="66b39-116">Request parameters</span></span>

<span data-ttu-id="66b39-117">要求 URL に、選択したクエリ パラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="66b39-117">In the request URL, provide the chosen query parameter with a valid value.</span></span>

| <span data-ttu-id="66b39-118">パラメーター</span><span class="sxs-lookup"><span data-stu-id="66b39-118">Parameter</span></span> | <span data-ttu-id="66b39-119">型</span><span class="sxs-lookup"><span data-stu-id="66b39-119">Type</span></span>   | <span data-ttu-id="66b39-120">説明</span><span class="sxs-lookup"><span data-stu-id="66b39-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="66b39-121">period</span><span class="sxs-lookup"><span data-stu-id="66b39-121">period</span></span>    | <span data-ttu-id="66b39-122">文字列</span><span class="sxs-lookup"><span data-stu-id="66b39-122">string</span></span> | <span data-ttu-id="66b39-123">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="66b39-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="66b39-124">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="66b39-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="66b39-125">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="66b39-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="66b39-126">date</span><span class="sxs-lookup"><span data-stu-id="66b39-126">date</span></span>      | <span data-ttu-id="66b39-127">日付</span><span class="sxs-lookup"><span data-stu-id="66b39-127">Date</span></span>   | <span data-ttu-id="66b39-128">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="66b39-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="66b39-129">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="66b39-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="66b39-130">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="66b39-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="66b39-131">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="66b39-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="66b39-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="66b39-132">Request headers</span></span>

| <span data-ttu-id="66b39-133">名前</span><span class="sxs-lookup"><span data-stu-id="66b39-133">Name</span></span>          | <span data-ttu-id="66b39-134">説明</span><span class="sxs-lookup"><span data-stu-id="66b39-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="66b39-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="66b39-135">Authorization</span></span> | <span data-ttu-id="66b39-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="66b39-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="66b39-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="66b39-138">if-none-match</span></span> | <span data-ttu-id="66b39-139">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="66b39-139">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="66b39-140">省略可能。</span><span class="sxs-lookup"><span data-stu-id="66b39-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="66b39-141">応答</span><span class="sxs-lookup"><span data-stu-id="66b39-141">Response</span></span>

<span data-ttu-id="66b39-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="66b39-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="66b39-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="66b39-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="66b39-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="66b39-144">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="66b39-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="66b39-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="66b39-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="66b39-146">Report Refresh Date</span></span>
- <span data-ttu-id="66b39-147">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="66b39-147">User Principal Name</span></span>
- <span data-ttu-id="66b39-148">表示名</span><span class="sxs-lookup"><span data-stu-id="66b39-148">Display Name</span></span>
- <span data-ttu-id="66b39-149">ユーザーの状態</span><span class="sxs-lookup"><span data-stu-id="66b39-149">Migrating User State</span></span>
- <span data-ttu-id="66b39-150">状態変更日付</span><span class="sxs-lookup"><span data-stu-id="66b39-150">State Change Date</span></span>
- <span data-ttu-id="66b39-151">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="66b39-151">Last Activity Date</span></span>
- <span data-ttu-id="66b39-152">Web の使用</span><span class="sxs-lookup"><span data-stu-id="66b39-152">Used Web</span></span>
- <span data-ttu-id="66b39-153">Windows スマートフォンの使用</span><span class="sxs-lookup"><span data-stu-id="66b39-153">Used Windows Phone</span></span>
- <span data-ttu-id="66b39-154">Android スマートフォンの使用</span><span class="sxs-lookup"><span data-stu-id="66b39-154">Used Android Phone</span></span>
- <span data-ttu-id="66b39-155">iPhone の使用</span><span class="sxs-lookup"><span data-stu-id="66b39-155">Used iPhone</span></span>
- <span data-ttu-id="66b39-156">IPad の使用</span><span class="sxs-lookup"><span data-stu-id="66b39-156">Used iPad</span></span>
- <span data-ttu-id="66b39-157">その他の使用</span><span class="sxs-lookup"><span data-stu-id="66b39-157">Used Others</span></span>
- <span data-ttu-id="66b39-158">レポート期間</span><span class="sxs-lookup"><span data-stu-id="66b39-158">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="66b39-159">例</span><span class="sxs-lookup"><span data-stu-id="66b39-159">Example</span></span>

#### <a name="request"></a><span data-ttu-id="66b39-160">要求</span><span class="sxs-lookup"><span data-stu-id="66b39-160">Request</span></span>

<span data-ttu-id="66b39-161">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="66b39-161">The following is an example of the request body.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="66b39-162">応答</span><span class="sxs-lookup"><span data-stu-id="66b39-162">Response</span></span>

<span data-ttu-id="66b39-163">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="66b39-163">The following is an example of a response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="66b39-164">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="66b39-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
