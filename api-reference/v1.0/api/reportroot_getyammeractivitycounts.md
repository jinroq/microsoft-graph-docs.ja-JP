# <a name="reportroot-getyammeractivitycounts"></a><span data-ttu-id="551cb-101">reportRoot: getYammerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="551cb-101">reportRoot: getYammerActivityCounts</span></span>

<span data-ttu-id="551cb-102">投稿、読み取り、および " いいね!" を付けられたメッセージの数によって、組織内での Yammer アクティビティの量の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="551cb-102">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span>

> <span data-ttu-id="551cb-103">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer アクティビティ](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="551cb-103">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="551cb-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="551cb-104">Permissions</span></span>

<span data-ttu-id="551cb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="551cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="551cb-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="551cb-107">Permission type</span></span>                        | <span data-ttu-id="551cb-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="551cb-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="551cb-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="551cb-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="551cb-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="551cb-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="551cb-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="551cb-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="551cb-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="551cb-112">Not supported.</span></span>                           |
| <span data-ttu-id="551cb-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="551cb-113">Application</span></span>                            | <span data-ttu-id="551cb-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="551cb-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="551cb-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="551cb-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="551cb-116">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="551cb-116">Function parameters</span></span>

<span data-ttu-id="551cb-117">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="551cb-117">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="551cb-118">パラメーター</span><span class="sxs-lookup"><span data-stu-id="551cb-118">Parameter</span></span> | <span data-ttu-id="551cb-119">型</span><span class="sxs-lookup"><span data-stu-id="551cb-119">Type</span></span>   | <span data-ttu-id="551cb-120">説明</span><span class="sxs-lookup"><span data-stu-id="551cb-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="551cb-121">期間</span><span class="sxs-lookup"><span data-stu-id="551cb-121">period</span></span>    | <span data-ttu-id="551cb-122">文字列</span><span class="sxs-lookup"><span data-stu-id="551cb-122">string</span></span> | <span data-ttu-id="551cb-123">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="551cb-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="551cb-124">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="551cb-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="551cb-125">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="551cb-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="551cb-126">必須。</span><span class="sxs-lookup"><span data-stu-id="551cb-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="551cb-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="551cb-127">Request headers</span></span>

| <span data-ttu-id="551cb-128">名前</span><span class="sxs-lookup"><span data-stu-id="551cb-128">Name</span></span>          | <span data-ttu-id="551cb-129">説明</span><span class="sxs-lookup"><span data-stu-id="551cb-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="551cb-130">承認</span><span class="sxs-lookup"><span data-stu-id="551cb-130">Authorization</span></span> | <span data-ttu-id="551cb-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="551cb-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="551cb-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="551cb-133">If-None-Match</span></span> | <span data-ttu-id="551cb-134">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="551cb-134">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="551cb-135">省略可能。</span><span class="sxs-lookup"><span data-stu-id="551cb-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="551cb-136">応答</span><span class="sxs-lookup"><span data-stu-id="551cb-136">Response</span></span>

<span data-ttu-id="551cb-137">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="551cb-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="551cb-138">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="551cb-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="551cb-139">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="551cb-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="551cb-140">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="551cb-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="551cb-141">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="551cb-141">Report Refresh Date</span></span>
- <span data-ttu-id="551cb-142">いいね!</span><span class="sxs-lookup"><span data-stu-id="551cb-142">Liked</span></span>
- <span data-ttu-id="551cb-143">投稿</span><span class="sxs-lookup"><span data-stu-id="551cb-143">Posted</span></span>
- <span data-ttu-id="551cb-144">読み取り</span><span class="sxs-lookup"><span data-stu-id="551cb-144">Read</span></span>
- <span data-ttu-id="551cb-145">レポート日付</span><span class="sxs-lookup"><span data-stu-id="551cb-145">Report Date</span></span>
- <span data-ttu-id="551cb-146">レポート期間</span><span class="sxs-lookup"><span data-stu-id="551cb-146">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="551cb-147">例</span><span class="sxs-lookup"><span data-stu-id="551cb-147">Example</span></span>

#### <a name="request"></a><span data-ttu-id="551cb-148">要求</span><span class="sxs-lookup"><span data-stu-id="551cb-148">Request</span></span>

<span data-ttu-id="551cb-149">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="551cb-149">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammeractivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="551cb-150">応答</span><span class="sxs-lookup"><span data-stu-id="551cb-150">Response</span></span>

<span data-ttu-id="551cb-151">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="551cb-151">The following is an example of the response.</span></span>

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

<span data-ttu-id="551cb-152">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="551cb-152">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
```
