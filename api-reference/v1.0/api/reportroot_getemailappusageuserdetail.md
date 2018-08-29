# <a name="reportroot-getemailappusageuserdetail"></a><span data-ttu-id="334c6-101">reportRoot: getEmailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="334c6-101">reportRoot: getEmailAppUsageUserDetail</span></span>

<span data-ttu-id="334c6-102">メール アプリの各バージョンでユーザーが実行したアクティビティの詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="334c6-102">Get details about which activities users performed on the various email apps.</span></span>

> <span data-ttu-id="334c6-103">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メール アプリの使用状況](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="334c6-103">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="334c6-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="334c6-104">Permissions</span></span>

<span data-ttu-id="334c6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="334c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="334c6-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="334c6-107">Permission type</span></span>                        | <span data-ttu-id="334c6-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="334c6-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="334c6-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="334c6-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="334c6-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="334c6-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="334c6-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="334c6-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="334c6-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="334c6-112">Not supported.</span></span>                           |
| <span data-ttu-id="334c6-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="334c6-113">Application</span></span>                            | <span data-ttu-id="334c6-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="334c6-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="334c6-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="334c6-115">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getEmailAppUsageUserDetail(period='{period_value}')
GET /reports/getEmailAppUsageUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="334c6-116">要求パラメーター</span><span class="sxs-lookup"><span data-stu-id="334c6-116">Request parameters</span></span>

<span data-ttu-id="334c6-117">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="334c6-117">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="334c6-118">パラメーター</span><span class="sxs-lookup"><span data-stu-id="334c6-118">Parameter</span></span> | <span data-ttu-id="334c6-119">型</span><span class="sxs-lookup"><span data-stu-id="334c6-119">Type</span></span>   | <span data-ttu-id="334c6-120">説明</span><span class="sxs-lookup"><span data-stu-id="334c6-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="334c6-121">period</span><span class="sxs-lookup"><span data-stu-id="334c6-121">period</span></span>    | <span data-ttu-id="334c6-122">文字列</span><span class="sxs-lookup"><span data-stu-id="334c6-122">string</span></span> | <span data-ttu-id="334c6-123">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="334c6-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="334c6-124">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="334c6-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="334c6-125">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="334c6-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="334c6-126">date</span><span class="sxs-lookup"><span data-stu-id="334c6-126">date</span></span>      | <span data-ttu-id="334c6-127">日付</span><span class="sxs-lookup"><span data-stu-id="334c6-127">Date</span></span>   | <span data-ttu-id="334c6-128">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="334c6-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="334c6-129">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="334c6-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="334c6-130">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="334c6-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="334c6-131">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="334c6-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="334c6-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="334c6-132">Request headers</span></span>

| <span data-ttu-id="334c6-133">名前</span><span class="sxs-lookup"><span data-stu-id="334c6-133">Name</span></span>          | <span data-ttu-id="334c6-134">説明</span><span class="sxs-lookup"><span data-stu-id="334c6-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="334c6-135">承認</span><span class="sxs-lookup"><span data-stu-id="334c6-135">Authorization</span></span> | <span data-ttu-id="334c6-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="334c6-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="334c6-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="334c6-138">If-None-Match</span></span> | <span data-ttu-id="334c6-139">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="334c6-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="334c6-140">省略可能。</span><span class="sxs-lookup"><span data-stu-id="334c6-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="334c6-141">応答</span><span class="sxs-lookup"><span data-stu-id="334c6-141">Response</span></span>

<span data-ttu-id="334c6-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="334c6-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="334c6-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="334c6-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="334c6-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="334c6-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="334c6-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="334c6-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="334c6-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="334c6-146">Report Refresh Date</span></span>
- <span data-ttu-id="334c6-147">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="334c6-147">User Principal Name</span></span>
- <span data-ttu-id="334c6-148">表示名</span><span class="sxs-lookup"><span data-stu-id="334c6-148">Display Name</span></span>
- <span data-ttu-id="334c6-149">削除済み</span><span class="sxs-lookup"><span data-stu-id="334c6-149">Is Deleted</span></span>
- <span data-ttu-id="334c6-150">削除日</span><span class="sxs-lookup"><span data-stu-id="334c6-150">Deleted Date</span></span>
- <span data-ttu-id="334c6-151">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="334c6-151">Last Activity Date</span></span>
- <span data-ttu-id="334c6-152">Mail For Mac</span><span class="sxs-lookup"><span data-stu-id="334c6-152">Mail For Mac</span></span>
- <span data-ttu-id="334c6-153">Outlook For Mac</span><span class="sxs-lookup"><span data-stu-id="334c6-153">Outlook For Mac</span></span>
- <span data-ttu-id="334c6-154">Outlook For Windows</span><span class="sxs-lookup"><span data-stu-id="334c6-154">Outlook For Windows</span></span>
- <span data-ttu-id="334c6-155">Outlook For Mobile</span><span class="sxs-lookup"><span data-stu-id="334c6-155">Outlook For Mobile</span></span>
- <span data-ttu-id="334c6-156">Other For Mobile</span><span class="sxs-lookup"><span data-stu-id="334c6-156">Other For Mobile</span></span>
- <span data-ttu-id="334c6-157">Outlook For Web</span><span class="sxs-lookup"><span data-stu-id="334c6-157">Outlook For Web</span></span>
- <span data-ttu-id="334c6-158">POP3 アプリ</span><span class="sxs-lookup"><span data-stu-id="334c6-158">POP3 App</span></span>
- <span data-ttu-id="334c6-159">IMAP4 アプリ</span><span class="sxs-lookup"><span data-stu-id="334c6-159">IMAP4 App</span></span>
- <span data-ttu-id="334c6-160">SMTP アプリ</span><span class="sxs-lookup"><span data-stu-id="334c6-160">SMTP App</span></span>
- <span data-ttu-id="334c6-161">レポート期間</span><span class="sxs-lookup"><span data-stu-id="334c6-161">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="334c6-162">例</span><span class="sxs-lookup"><span data-stu-id="334c6-162">Example</span></span>

#### <a name="request"></a><span data-ttu-id="334c6-163">要求</span><span class="sxs-lookup"><span data-stu-id="334c6-163">Request</span></span>

<span data-ttu-id="334c6-164">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="334c6-164">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailappusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="334c6-165">応答</span><span class="sxs-lookup"><span data-stu-id="334c6-165">Response</span></span>

<span data-ttu-id="334c6-166">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="334c6-166">The following is an example of the response.</span></span>

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

<span data-ttu-id="334c6-167">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="334c6-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Period
```
