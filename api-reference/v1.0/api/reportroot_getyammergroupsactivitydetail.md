# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="e677f-101">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="e677f-101">reportRoot: getYammerGroupsActivityDetail</span></span>

<span data-ttu-id="e677f-102">グループ別の Yammer グループ アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="e677f-102">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="e677f-103">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer グループ アクティビティ](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e677f-103">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="e677f-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e677f-104">Permissions</span></span>

<span data-ttu-id="e677f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e677f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="e677f-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e677f-107">Permission type</span></span>                        | <span data-ttu-id="e677f-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e677f-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e677f-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="e677f-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="e677f-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e677f-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e677f-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e677f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e677f-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e677f-112">Not supported.</span></span>                           |
| <span data-ttu-id="e677f-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e677f-113">Application</span></span>                            | <span data-ttu-id="e677f-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e677f-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e677f-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e677f-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="e677f-116">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="e677f-116">Function parameters</span></span>

<span data-ttu-id="e677f-117">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="e677f-117">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="e677f-118">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e677f-118">Parameter</span></span> | <span data-ttu-id="e677f-119">型</span><span class="sxs-lookup"><span data-stu-id="e677f-119">Type</span></span>   | <span data-ttu-id="e677f-120">説明</span><span class="sxs-lookup"><span data-stu-id="e677f-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e677f-121">期間</span><span class="sxs-lookup"><span data-stu-id="e677f-121">period</span></span>    | <span data-ttu-id="e677f-122">文字列</span><span class="sxs-lookup"><span data-stu-id="e677f-122">string</span></span> | <span data-ttu-id="e677f-123">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="e677f-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e677f-124">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="e677f-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e677f-125">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="e677f-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="e677f-126">日付</span><span class="sxs-lookup"><span data-stu-id="e677f-126">date</span></span>      | <span data-ttu-id="e677f-127">日付</span><span class="sxs-lookup"><span data-stu-id="e677f-127">Date</span></span>   | <span data-ttu-id="e677f-128">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="e677f-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="e677f-129">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="e677f-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="e677f-130">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="e677f-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="e677f-131">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e677f-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e677f-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e677f-132">Request headers</span></span>

| <span data-ttu-id="e677f-133">名前</span><span class="sxs-lookup"><span data-stu-id="e677f-133">Name</span></span>          | <span data-ttu-id="e677f-134">説明</span><span class="sxs-lookup"><span data-stu-id="e677f-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="e677f-135">承認</span><span class="sxs-lookup"><span data-stu-id="e677f-135">Authorization</span></span> | <span data-ttu-id="e677f-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e677f-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="e677f-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="e677f-138">If-None-Match</span></span> | <span data-ttu-id="e677f-139">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="e677f-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="e677f-140">省略可能。</span><span class="sxs-lookup"><span data-stu-id="e677f-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="e677f-141">応答</span><span class="sxs-lookup"><span data-stu-id="e677f-141">Response</span></span>

<span data-ttu-id="e677f-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="e677f-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e677f-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="e677f-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e677f-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="e677f-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e677f-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="e677f-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e677f-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="e677f-146">Report Refresh Date</span></span>
- <span data-ttu-id="e677f-147">グループ表示名</span><span class="sxs-lookup"><span data-stu-id="e677f-147">Group Display Name</span></span>
- <span data-ttu-id="e677f-148">削除済み</span><span class="sxs-lookup"><span data-stu-id="e677f-148">Is Deleted</span></span>
- <span data-ttu-id="e677f-149">所有者のプリンシパル名</span><span class="sxs-lookup"><span data-stu-id="e677f-149">Owner Principal Name</span></span>
- <span data-ttu-id="e677f-150">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="e677f-150">Last Activity Date</span></span>
- <span data-ttu-id="e677f-151">グループの種類</span><span class="sxs-lookup"><span data-stu-id="e677f-151">Group Type</span></span>
- <span data-ttu-id="e677f-152">Office 365 接続</span><span class="sxs-lookup"><span data-stu-id="e677f-152">Office 365 Connected</span></span>
- <span data-ttu-id="e677f-153">メンバー数</span><span class="sxs-lookup"><span data-stu-id="e677f-153">Member Count</span></span>
- <span data-ttu-id="e677f-154">投稿数</span><span class="sxs-lookup"><span data-stu-id="e677f-154">Posted Count</span></span>
- <span data-ttu-id="e677f-155">読み取り数</span><span class="sxs-lookup"><span data-stu-id="e677f-155">Read Count</span></span>
- <span data-ttu-id="e677f-156">「いいね!」の数</span><span class="sxs-lookup"><span data-stu-id="e677f-156">Liked Count</span></span>
- <span data-ttu-id="e677f-157">レポート期間</span><span class="sxs-lookup"><span data-stu-id="e677f-157">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="e677f-158">例</span><span class="sxs-lookup"><span data-stu-id="e677f-158">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e677f-159">要求</span><span class="sxs-lookup"><span data-stu-id="e677f-159">Request</span></span>

<span data-ttu-id="e677f-160">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e677f-160">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="e677f-161">応答</span><span class="sxs-lookup"><span data-stu-id="e677f-161">Response</span></span>

<span data-ttu-id="e677f-162">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e677f-162">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="e677f-163">要求</span><span class="sxs-lookup"><span data-stu-id="e677f-163">Request</span></span>
<span data-ttu-id="e677f-164">で呼び出した場合、レポートは指定した日のアクティビティに制限されます。`date`</span><span class="sxs-lookup"><span data-stu-id="e677f-164">If called with a `date`, the report is scoped to activity on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivityuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="e677f-165">応答</span><span class="sxs-lookup"><span data-stu-id="e677f-165">Response</span></span>

<span data-ttu-id="e677f-166">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e677f-166">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="e677f-167">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="e677f-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "ignored"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Office 365 Connected,Member Count,Posted Count,Read Count,Liked Count,Report Period
```
