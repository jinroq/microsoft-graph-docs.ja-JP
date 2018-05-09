# <a name="reportroot-getmailboxusagemailboxcounts"></a><span data-ttu-id="e91db-101">reportRoot: getMailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="e91db-101">reportRoot: getMailboxUsageMailboxCounts</span></span>

<span data-ttu-id="e91db-102">組織内のユーザー メールボックスの合計数と、レポート期間中の各日にアクティブなメールボックス数を取得します。</span><span class="sxs-lookup"><span data-stu-id="e91db-102">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="e91db-103">メールボックスは、ユーザーが何らかの電子メールを送信するか、読んだ場合にアクティブとみなされます。</span><span class="sxs-lookup"><span data-stu-id="e91db-103">A mailbox is considered active if the user sent or read any email.</span></span>

> <span data-ttu-id="e91db-104">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メールボックスの使用状況](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e91db-104">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="e91db-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e91db-105">Permissions</span></span>

<span data-ttu-id="e91db-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e91db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="e91db-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e91db-108">Permission type</span></span>                        | <span data-ttu-id="e91db-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e91db-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e91db-110">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="e91db-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e91db-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e91db-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e91db-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e91db-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e91db-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e91db-113">Not supported.</span></span>                           |
| <span data-ttu-id="e91db-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e91db-114">Application</span></span>                            | <span data-ttu-id="e91db-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e91db-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e91db-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e91db-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageMailboxCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="e91db-117">要求パラメーター</span><span class="sxs-lookup"><span data-stu-id="e91db-117">Request parameters</span></span>

<span data-ttu-id="e91db-118">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="e91db-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e91db-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e91db-119">Parameter</span></span> | <span data-ttu-id="e91db-120">型</span><span class="sxs-lookup"><span data-stu-id="e91db-120">Type</span></span>   | <span data-ttu-id="e91db-121">説明</span><span class="sxs-lookup"><span data-stu-id="e91db-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e91db-122">period</span><span class="sxs-lookup"><span data-stu-id="e91db-122">period</span></span>    | <span data-ttu-id="e91db-123">文字列</span><span class="sxs-lookup"><span data-stu-id="e91db-123">string</span></span> | <span data-ttu-id="e91db-124">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="e91db-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e91db-125">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="e91db-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e91db-126">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="e91db-126">These values follow the format D   where    represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e91db-127">必須。</span><span class="sxs-lookup"><span data-stu-id="e91db-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="e91db-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e91db-128">Request headers</span></span>

| <span data-ttu-id="e91db-129">名前</span><span class="sxs-lookup"><span data-stu-id="e91db-129">Name</span></span>          | <span data-ttu-id="e91db-130">説明</span><span class="sxs-lookup"><span data-stu-id="e91db-130">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="e91db-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="e91db-131">Authorization</span></span> | <span data-ttu-id="e91db-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e91db-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="e91db-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="e91db-134">If-None-Match</span></span> | <span data-ttu-id="e91db-135">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="e91db-135">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="e91db-136">省略可能。</span><span class="sxs-lookup"><span data-stu-id="e91db-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="e91db-137">応答</span><span class="sxs-lookup"><span data-stu-id="e91db-137">Response</span></span>

<span data-ttu-id="e91db-138">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="e91db-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e91db-139">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="e91db-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e91db-140">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="e91db-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e91db-141">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="e91db-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e91db-142">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="e91db-142">Report Refresh Date</span></span>
- <span data-ttu-id="e91db-143">合計</span><span class="sxs-lookup"><span data-stu-id="e91db-143">Total</span></span>
- <span data-ttu-id="e91db-144">アクティブ</span><span class="sxs-lookup"><span data-stu-id="e91db-144">Active</span></span>
- <span data-ttu-id="e91db-145">レポート日付</span><span class="sxs-lookup"><span data-stu-id="e91db-145">Report Date</span></span>
- <span data-ttu-id="e91db-146">レポート期間</span><span class="sxs-lookup"><span data-stu-id="e91db-146">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="e91db-147">例</span><span class="sxs-lookup"><span data-stu-id="e91db-147">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e91db-148">要求</span><span class="sxs-lookup"><span data-stu-id="e91db-148">Request</span></span>

<span data-ttu-id="e91db-149">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e91db-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagemailboxcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageMailboxCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="e91db-150">応答</span><span class="sxs-lookup"><span data-stu-id="e91db-150">Response</span></span>

<span data-ttu-id="e91db-151">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e91db-151">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="e91db-152">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="e91db-152">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
```
