# <a name="reportroot-getskypeforbusinessdeviceusageuserdetail"></a><span data-ttu-id="c5f67-101">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="c5f67-101">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span></span>

<span data-ttu-id="c5f67-102">ユーザー別の Skype for Business デバイス使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="c5f67-102">Get details about Skype for Business device usage by user.</span></span>

> <span data-ttu-id="c5f67-103">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: 使用している Skype for Business クライアント](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c5f67-103">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="c5f67-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c5f67-104">Permissions</span></span>

<span data-ttu-id="c5f67-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c5f67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="c5f67-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c5f67-107">Permission type</span></span>                        | <span data-ttu-id="c5f67-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c5f67-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c5f67-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="c5f67-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="c5f67-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5f67-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c5f67-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c5f67-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5f67-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c5f67-112">Not supported.</span></span>                           |
| <span data-ttu-id="c5f67-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c5f67-113">Application</span></span>                            | <span data-ttu-id="c5f67-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5f67-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c5f67-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c5f67-115">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="c5f67-116">要求パラメーター</span><span class="sxs-lookup"><span data-stu-id="c5f67-116">Request parameters</span></span>

<span data-ttu-id="c5f67-117">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="c5f67-117">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="c5f67-118">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c5f67-118">Parameter</span></span> | <span data-ttu-id="c5f67-119">型</span><span class="sxs-lookup"><span data-stu-id="c5f67-119">Type</span></span>   | <span data-ttu-id="c5f67-120">説明</span><span class="sxs-lookup"><span data-stu-id="c5f67-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c5f67-121">period</span><span class="sxs-lookup"><span data-stu-id="c5f67-121">period</span></span>    | <span data-ttu-id="c5f67-122">文字列</span><span class="sxs-lookup"><span data-stu-id="c5f67-122">string</span></span> | <span data-ttu-id="c5f67-123">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="c5f67-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c5f67-124">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="c5f67-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c5f67-125">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="c5f67-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="c5f67-126">date</span><span class="sxs-lookup"><span data-stu-id="c5f67-126">date</span></span>      | <span data-ttu-id="c5f67-127">日付</span><span class="sxs-lookup"><span data-stu-id="c5f67-127">Date</span></span>   | <span data-ttu-id="c5f67-128">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="c5f67-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="c5f67-129">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="c5f67-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="c5f67-130">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="c5f67-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="c5f67-131">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c5f67-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5f67-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c5f67-132">Request headers</span></span>

| <span data-ttu-id="c5f67-133">名前</span><span class="sxs-lookup"><span data-stu-id="c5f67-133">Name</span></span>          | <span data-ttu-id="c5f67-134">説明</span><span class="sxs-lookup"><span data-stu-id="c5f67-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="c5f67-135">承認</span><span class="sxs-lookup"><span data-stu-id="c5f67-135">Authorization</span></span> | <span data-ttu-id="c5f67-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c5f67-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="c5f67-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="c5f67-138">If-None-Match</span></span> | <span data-ttu-id="c5f67-139">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="c5f67-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="c5f67-140">省略可能。</span><span class="sxs-lookup"><span data-stu-id="c5f67-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="c5f67-141">応答</span><span class="sxs-lookup"><span data-stu-id="c5f67-141">Response</span></span>

<span data-ttu-id="c5f67-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="c5f67-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c5f67-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="c5f67-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c5f67-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="c5f67-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c5f67-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="c5f67-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c5f67-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="c5f67-146">Report Refresh Date</span></span>
- <span data-ttu-id="c5f67-147">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="c5f67-147">User Principal Name</span></span>
- <span data-ttu-id="c5f67-148">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="c5f67-148">Last Activity Date</span></span>
- <span data-ttu-id="c5f67-149">Windows の使用</span><span class="sxs-lookup"><span data-stu-id="c5f67-149">Used Windows</span></span>
- <span data-ttu-id="c5f67-150">Windows スマートフォンの使用</span><span class="sxs-lookup"><span data-stu-id="c5f67-150">Used Windows Phone</span></span>
- <span data-ttu-id="c5f67-151">Android スマートフォンの使用</span><span class="sxs-lookup"><span data-stu-id="c5f67-151">Used Android Phone</span></span>
- <span data-ttu-id="c5f67-152">iPhone の使用</span><span class="sxs-lookup"><span data-stu-id="c5f67-152">Used iPhone</span></span>
- <span data-ttu-id="c5f67-153">IPad の使用</span><span class="sxs-lookup"><span data-stu-id="c5f67-153">Used iPad</span></span>
- <span data-ttu-id="c5f67-154">レポート期間</span><span class="sxs-lookup"><span data-stu-id="c5f67-154">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="c5f67-155">例</span><span class="sxs-lookup"><span data-stu-id="c5f67-155">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c5f67-156">要求</span><span class="sxs-lookup"><span data-stu-id="c5f67-156">Request</span></span>

<span data-ttu-id="c5f67-157">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c5f67-157">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="c5f67-158">応答</span><span class="sxs-lookup"><span data-stu-id="c5f67-158">Response</span></span>

<span data-ttu-id="c5f67-159">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c5f67-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="c5f67-160">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="c5f67-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Used Windows,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Report Period
```
