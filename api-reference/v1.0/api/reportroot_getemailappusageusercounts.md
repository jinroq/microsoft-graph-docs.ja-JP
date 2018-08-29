# <a name="reportroot-getemailappusageusercounts"></a><span data-ttu-id="69478-101">reportRoot: getEmailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="69478-101">reportRoot: getEmailAppUsageUserCounts</span></span>

<span data-ttu-id="69478-102">任意のメール アプリを使用して Exchange Online に接続されている、それぞれ別個のユーザー数を取得します。</span><span class="sxs-lookup"><span data-stu-id="69478-102">Get the count of unique users that connected to Exchange Online using any email app.</span></span>

> <span data-ttu-id="69478-103">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メール アプリの使用状況](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="69478-103">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="69478-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="69478-104">Permissions</span></span>

<span data-ttu-id="69478-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="69478-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="69478-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="69478-107">Permission type</span></span>                        | <span data-ttu-id="69478-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="69478-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="69478-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="69478-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="69478-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="69478-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="69478-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="69478-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69478-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69478-112">Not supported.</span></span>                           |
| <span data-ttu-id="69478-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="69478-113">Application</span></span>                            | <span data-ttu-id="69478-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="69478-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="69478-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="69478-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="69478-116">要求パラメーター</span><span class="sxs-lookup"><span data-stu-id="69478-116">Request parameters</span></span>

<span data-ttu-id="69478-117">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="69478-117">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="69478-118">パラメーター</span><span class="sxs-lookup"><span data-stu-id="69478-118">Parameter</span></span> | <span data-ttu-id="69478-119">型</span><span class="sxs-lookup"><span data-stu-id="69478-119">Type</span></span>   | <span data-ttu-id="69478-120">説明</span><span class="sxs-lookup"><span data-stu-id="69478-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="69478-121">period</span><span class="sxs-lookup"><span data-stu-id="69478-121">period</span></span>    | <span data-ttu-id="69478-122">文字列</span><span class="sxs-lookup"><span data-stu-id="69478-122">string</span></span> | <span data-ttu-id="69478-123">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="69478-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="69478-124">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="69478-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="69478-125">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="69478-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="69478-126">必須。</span><span class="sxs-lookup"><span data-stu-id="69478-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="69478-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="69478-127">Request headers</span></span>

| <span data-ttu-id="69478-128">名前</span><span class="sxs-lookup"><span data-stu-id="69478-128">Name</span></span>          | <span data-ttu-id="69478-129">説明</span><span class="sxs-lookup"><span data-stu-id="69478-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="69478-130">承認</span><span class="sxs-lookup"><span data-stu-id="69478-130">Authorization</span></span> | <span data-ttu-id="69478-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="69478-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="69478-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="69478-133">If-None-Match</span></span> | <span data-ttu-id="69478-134">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="69478-134">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="69478-135">省略可能。</span><span class="sxs-lookup"><span data-stu-id="69478-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="69478-136">応答</span><span class="sxs-lookup"><span data-stu-id="69478-136">Response</span></span>

<span data-ttu-id="69478-137">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="69478-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="69478-138">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="69478-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="69478-139">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="69478-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="69478-140">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="69478-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="69478-141">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="69478-141">Report Refresh Date</span></span>
- <span data-ttu-id="69478-142">Mail For Mac</span><span class="sxs-lookup"><span data-stu-id="69478-142">Mail For Mac</span></span>
- <span data-ttu-id="69478-143">Outlook For Mac</span><span class="sxs-lookup"><span data-stu-id="69478-143">Outlook For Mac</span></span>
- <span data-ttu-id="69478-144">Outlook For Windows</span><span class="sxs-lookup"><span data-stu-id="69478-144">Outlook For Windows</span></span>
- <span data-ttu-id="69478-145">Outlook For Mobile</span><span class="sxs-lookup"><span data-stu-id="69478-145">Outlook For Mobile</span></span>
- <span data-ttu-id="69478-146">Other For Mobile</span><span class="sxs-lookup"><span data-stu-id="69478-146">Other For Mobile</span></span>
- <span data-ttu-id="69478-147">Outlook For Web</span><span class="sxs-lookup"><span data-stu-id="69478-147">Outlook For Web</span></span>
- <span data-ttu-id="69478-148">POP3 アプリ</span><span class="sxs-lookup"><span data-stu-id="69478-148">POP3 App</span></span>
- <span data-ttu-id="69478-149">IMAP4 アプリ</span><span class="sxs-lookup"><span data-stu-id="69478-149">IMAP4 App</span></span>
- <span data-ttu-id="69478-150">SMTP アプリ</span><span class="sxs-lookup"><span data-stu-id="69478-150">SMTP App</span></span>
- <span data-ttu-id="69478-151">レポート日付</span><span class="sxs-lookup"><span data-stu-id="69478-151">Report Date</span></span>
- <span data-ttu-id="69478-152">レポート期間</span><span class="sxs-lookup"><span data-stu-id="69478-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="69478-153">例</span><span class="sxs-lookup"><span data-stu-id="69478-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="69478-154">要求</span><span class="sxs-lookup"><span data-stu-id="69478-154">Request</span></span>

<span data-ttu-id="69478-155">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="69478-155">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailappusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="69478-156">応答</span><span class="sxs-lookup"><span data-stu-id="69478-156">Response</span></span>

<span data-ttu-id="69478-157">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="69478-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="69478-158">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="69478-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Date,Report Period
```
