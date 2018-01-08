# <a name="reportroot-getemailappusageappsusercounts"></a><span data-ttu-id="c8852-101">reportRoot: getEmailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="c8852-101">reportRoot: getEmailAppUsageAppsUserCounts</span></span>

<span data-ttu-id="c8852-102">メール アプリごとの、それぞれ別個のユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="c8852-102">Get the count of unique users per email app.</span></span>

> <span data-ttu-id="c8852-103">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メール アプリの使用状況]((https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d))」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8852-103">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage]((https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)).</span></span>

## <a name="permissions"></a><span data-ttu-id="c8852-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c8852-104">Permissions</span></span>

<span data-ttu-id="c8852-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8852-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="c8852-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c8852-107">Permission type</span></span>                        | <span data-ttu-id="c8852-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c8852-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c8852-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c8852-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="c8852-110">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8852-110">Not supported.</span></span>                           |
| <span data-ttu-id="c8852-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c8852-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8852-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8852-112">Not supported.</span></span>                           |
| <span data-ttu-id="c8852-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c8852-113">Application</span></span>                            | <span data-ttu-id="c8852-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8852-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c8852-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c8852-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageAppsUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="c8852-116">要求パラメーター</span><span class="sxs-lookup"><span data-stu-id="c8852-116">Request parameters</span></span>

<span data-ttu-id="c8852-117">要求 URL に、次のクエリ パラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="c8852-117">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="c8852-118">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c8852-118">Parameter</span></span> | <span data-ttu-id="c8852-119">型</span><span class="sxs-lookup"><span data-stu-id="c8852-119">Type</span></span>   | <span data-ttu-id="c8852-120">説明</span><span class="sxs-lookup"><span data-stu-id="c8852-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c8852-121">period</span><span class="sxs-lookup"><span data-stu-id="c8852-121">period</span></span>    | <span data-ttu-id="c8852-122">文字列</span><span class="sxs-lookup"><span data-stu-id="c8852-122">string</span></span> | <span data-ttu-id="c8852-123">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="c8852-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c8852-124">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="c8852-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c8852-125">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="c8852-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c8852-126">必須。</span><span class="sxs-lookup"><span data-stu-id="c8852-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="c8852-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8852-127">Request headers</span></span>

| <span data-ttu-id="c8852-128">名前</span><span class="sxs-lookup"><span data-stu-id="c8852-128">Name</span></span>          | <span data-ttu-id="c8852-129">説明</span><span class="sxs-lookup"><span data-stu-id="c8852-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="c8852-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8852-130">Authorization</span></span> | <span data-ttu-id="c8852-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c8852-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="c8852-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="c8852-133">if-none-match</span></span> | <span data-ttu-id="c8852-134">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="c8852-134">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="c8852-135">省略可能。</span><span class="sxs-lookup"><span data-stu-id="c8852-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="c8852-136">応答</span><span class="sxs-lookup"><span data-stu-id="c8852-136">Response</span></span>

<span data-ttu-id="c8852-137">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="c8852-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c8852-138">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="c8852-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c8852-139">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="c8852-139">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="c8852-140">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="c8852-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c8852-141">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="c8852-141">Report Refresh Date</span></span>
- <span data-ttu-id="c8852-142">Mail For Mac</span><span class="sxs-lookup"><span data-stu-id="c8852-142">Mail For Mac</span></span>
- <span data-ttu-id="c8852-143">Outlook For Mac</span><span class="sxs-lookup"><span data-stu-id="c8852-143">Outlook for Mac</span></span>
- <span data-ttu-id="c8852-144">Outlook For Windows</span><span class="sxs-lookup"><span data-stu-id="c8852-144">Outlook for Windows</span></span>
- <span data-ttu-id="c8852-145">Outlook For Mobile</span><span class="sxs-lookup"><span data-stu-id="c8852-145">Outlook For Mobile</span></span>
- <span data-ttu-id="c8852-146">Other For Mobile</span><span class="sxs-lookup"><span data-stu-id="c8852-146">Other For Mobile</span></span>
- <span data-ttu-id="c8852-147">Outlook For Web</span><span class="sxs-lookup"><span data-stu-id="c8852-147">Outlook for web</span></span>
- <span data-ttu-id="c8852-148">POP3 アプリ</span><span class="sxs-lookup"><span data-stu-id="c8852-148">POP3 App</span></span>
- <span data-ttu-id="c8852-149">IMAP4 アプリ</span><span class="sxs-lookup"><span data-stu-id="c8852-149">IMAP4 App</span></span>
- <span data-ttu-id="c8852-150">SMTP アプリ</span><span class="sxs-lookup"><span data-stu-id="c8852-150">SMTP App</span></span>
- <span data-ttu-id="c8852-151">レポート期間</span><span class="sxs-lookup"><span data-stu-id="c8852-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="c8852-152">例</span><span class="sxs-lookup"><span data-stu-id="c8852-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c8852-153">要求</span><span class="sxs-lookup"><span data-stu-id="c8852-153">Request</span></span>

<span data-ttu-id="c8852-154">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c8852-154">The following is an example of the request body.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageappsusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageAppsUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="c8852-155">応答</span><span class="sxs-lookup"><span data-stu-id="c8852-155">Response</span></span>

<span data-ttu-id="c8852-156">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c8852-156">The following is an example of a response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="c8852-157">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="c8852-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Period
```
