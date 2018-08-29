# <a name="reportroot-getonedriveusageaccountdetail"></a><span data-ttu-id="e38ea-101">reportRoot: getOneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="e38ea-101">reportRoot: getOneDriveUsageAccountDetail</span></span>

<span data-ttu-id="e38ea-102">アカウント別の OneDrive の使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="e38ea-102">Get details about OneDrive usage by account.</span></span>

> <span data-ttu-id="e38ea-103">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business の使用状況](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e38ea-103">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="e38ea-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e38ea-104">Permissions</span></span>

<span data-ttu-id="e38ea-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e38ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="e38ea-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e38ea-107">Permission type</span></span>                        | <span data-ttu-id="e38ea-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e38ea-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e38ea-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="e38ea-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="e38ea-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e38ea-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e38ea-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e38ea-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e38ea-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e38ea-112">Not supported.</span></span>                           |
| <span data-ttu-id="e38ea-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e38ea-113">Application</span></span>                            | <span data-ttu-id="e38ea-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e38ea-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e38ea-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e38ea-115">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOneDriveUsageAccountDetail(period='{period_value}')
GET /reports/getOneDriveUsageAccountDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="e38ea-116">要求パラメーター</span><span class="sxs-lookup"><span data-stu-id="e38ea-116">Request parameters</span></span>

<span data-ttu-id="e38ea-117">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="e38ea-117">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="e38ea-118">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e38ea-118">Parameter</span></span> | <span data-ttu-id="e38ea-119">型</span><span class="sxs-lookup"><span data-stu-id="e38ea-119">Type</span></span>   | <span data-ttu-id="e38ea-120">説明</span><span class="sxs-lookup"><span data-stu-id="e38ea-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e38ea-121">period</span><span class="sxs-lookup"><span data-stu-id="e38ea-121">period</span></span>    | <span data-ttu-id="e38ea-122">文字列</span><span class="sxs-lookup"><span data-stu-id="e38ea-122">string</span></span> | <span data-ttu-id="e38ea-123">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="e38ea-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e38ea-124">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="e38ea-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e38ea-125">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="e38ea-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="e38ea-126">date</span><span class="sxs-lookup"><span data-stu-id="e38ea-126">date</span></span>      | <span data-ttu-id="e38ea-127">日付</span><span class="sxs-lookup"><span data-stu-id="e38ea-127">Date</span></span>   | <span data-ttu-id="e38ea-128">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="e38ea-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="e38ea-129">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="e38ea-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="e38ea-130">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="e38ea-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="e38ea-131">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e38ea-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e38ea-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e38ea-132">Request headers</span></span>

| <span data-ttu-id="e38ea-133">名前</span><span class="sxs-lookup"><span data-stu-id="e38ea-133">Name</span></span>          | <span data-ttu-id="e38ea-134">説明</span><span class="sxs-lookup"><span data-stu-id="e38ea-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="e38ea-135">承認</span><span class="sxs-lookup"><span data-stu-id="e38ea-135">Authorization</span></span> | <span data-ttu-id="e38ea-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e38ea-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="e38ea-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="e38ea-138">If-None-Match</span></span> | <span data-ttu-id="e38ea-139">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="e38ea-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="e38ea-140">省略可能。</span><span class="sxs-lookup"><span data-stu-id="e38ea-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="e38ea-141">応答</span><span class="sxs-lookup"><span data-stu-id="e38ea-141">Response</span></span>

<span data-ttu-id="e38ea-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="e38ea-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e38ea-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="e38ea-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e38ea-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="e38ea-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e38ea-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="e38ea-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e38ea-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="e38ea-146">Report Refresh Date</span></span>
- <span data-ttu-id="e38ea-147">サイトの URL</span><span class="sxs-lookup"><span data-stu-id="e38ea-147">Site URL</span></span>
- <span data-ttu-id="e38ea-148">所有者の表示名</span><span class="sxs-lookup"><span data-stu-id="e38ea-148">Owner Display Name</span></span>
- <span data-ttu-id="e38ea-149">削除済み</span><span class="sxs-lookup"><span data-stu-id="e38ea-149">Is Deleted</span></span>
- <span data-ttu-id="e38ea-150">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="e38ea-150">Last Activity Date</span></span>
- <span data-ttu-id="e38ea-151">ファイル数</span><span class="sxs-lookup"><span data-stu-id="e38ea-151">File Count</span></span>
- <span data-ttu-id="e38ea-152">アクティブなファイル数</span><span class="sxs-lookup"><span data-stu-id="e38ea-152">Active File Count</span></span>
- <span data-ttu-id="e38ea-153">使用済みストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="e38ea-153">Storage Used (Byte)</span></span>
- <span data-ttu-id="e38ea-154">割り当て済みストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="e38ea-154">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="e38ea-155">レポート期間</span><span class="sxs-lookup"><span data-stu-id="e38ea-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="e38ea-156">例</span><span class="sxs-lookup"><span data-stu-id="e38ea-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e38ea-157">要求</span><span class="sxs-lookup"><span data-stu-id="e38ea-157">Request</span></span>

<span data-ttu-id="e38ea-158">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e38ea-158">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageAccountDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="e38ea-159">応答</span><span class="sxs-lookup"><span data-stu-id="e38ea-159">Response</span></span>

<span data-ttu-id="e38ea-160">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e38ea-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="e38ea-161">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="e38ea-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Storage Used (Byte),Storage Allocated (Byte),Report Period
```
