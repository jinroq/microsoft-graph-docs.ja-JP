# <a name="reportroot-getskypeforbusinessorganizeractivityminutecounts"></a><span data-ttu-id="7001e-101">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="7001e-101">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span></span>

<span data-ttu-id="7001e-102">組織内のユーザーが開催、企画した電話会議セッションの長さ (分数) と種類に関する使用状況の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="7001e-102">Get usage trends on the length in minutes and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="7001e-103">電話会議セッションの種類には、オーディオ/ビデオ、および Microsoft へのダイヤルインとダイヤルアウトがあります。</span><span class="sxs-lookup"><span data-stu-id="7001e-103">Types of conference sessions include audio/video, and dial-in and dial-out - Microsoft.</span></span>

> <span data-ttu-id="7001e-104">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business 電話会議の開催者のアクティビティ]((https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254))」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7001e-104">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity]((https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254)).</span></span>

## <a name="permissions"></a><span data-ttu-id="7001e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7001e-105">Permissions</span></span>

<span data-ttu-id="7001e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7001e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="7001e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7001e-108">Permission type</span></span>                        | <span data-ttu-id="7001e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7001e-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7001e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7001e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7001e-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7001e-111">Not supported.</span></span>                           |
| <span data-ttu-id="7001e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7001e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7001e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7001e-113">Not supported.</span></span>                           |
| <span data-ttu-id="7001e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7001e-114">Application</span></span>                            | <span data-ttu-id="7001e-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7001e-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7001e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7001e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="7001e-117">要求パラメーター</span><span class="sxs-lookup"><span data-stu-id="7001e-117">Request parameters</span></span>

<span data-ttu-id="7001e-118">要求 URL に、次のクエリ パラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="7001e-118">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="7001e-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="7001e-119">Parameter</span></span> | <span data-ttu-id="7001e-120">型</span><span class="sxs-lookup"><span data-stu-id="7001e-120">Type</span></span>   | <span data-ttu-id="7001e-121">説明</span><span class="sxs-lookup"><span data-stu-id="7001e-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7001e-122">period</span><span class="sxs-lookup"><span data-stu-id="7001e-122">period</span></span>    | <span data-ttu-id="7001e-123">文字列</span><span class="sxs-lookup"><span data-stu-id="7001e-123">string</span></span> | <span data-ttu-id="7001e-124">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="7001e-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7001e-125">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="7001e-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7001e-126">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="7001e-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="7001e-127">必須。</span><span class="sxs-lookup"><span data-stu-id="7001e-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="7001e-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7001e-128">Request headers</span></span>

| <span data-ttu-id="7001e-129">名前</span><span class="sxs-lookup"><span data-stu-id="7001e-129">Name</span></span>          | <span data-ttu-id="7001e-130">説明</span><span class="sxs-lookup"><span data-stu-id="7001e-130">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7001e-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="7001e-131">Authorization</span></span> | <span data-ttu-id="7001e-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7001e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7001e-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="7001e-134">if-none-match</span></span> | <span data-ttu-id="7001e-135">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="7001e-135">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="7001e-136">省略可能。</span><span class="sxs-lookup"><span data-stu-id="7001e-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="7001e-137">応答</span><span class="sxs-lookup"><span data-stu-id="7001e-137">Response</span></span>

<span data-ttu-id="7001e-138">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="7001e-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7001e-139">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="7001e-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7001e-140">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="7001e-140">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="7001e-141">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="7001e-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7001e-142">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="7001e-142">Report Refresh Date</span></span>
- <span data-ttu-id="7001e-143">レポート日付</span><span class="sxs-lookup"><span data-stu-id="7001e-143">Schedule Report Date</span></span>
- <span data-ttu-id="7001e-144">レポート期間</span><span class="sxs-lookup"><span data-stu-id="7001e-144">Report Period</span></span>
- <span data-ttu-id="7001e-145">オーディオ/ビデオ</span><span class="sxs-lookup"><span data-stu-id="7001e-145">Audio/Video</span></span>
- <span data-ttu-id="7001e-146">Microsoft へのダイヤルイン</span><span class="sxs-lookup"><span data-stu-id="7001e-146">Dial-in Microsoft</span></span>
- <span data-ttu-id="7001e-147">Microsoft からダイヤルアウト</span><span class="sxs-lookup"><span data-stu-id="7001e-147">Dial-out Microsoft</span></span>

## <a name="example"></a><span data-ttu-id="7001e-148">例</span><span class="sxs-lookup"><span data-stu-id="7001e-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7001e-149">要求</span><span class="sxs-lookup"><span data-stu-id="7001e-149">Request</span></span>

<span data-ttu-id="7001e-150">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7001e-150">The following is an example of the request body.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivityminutecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="7001e-151">応答</span><span class="sxs-lookup"><span data-stu-id="7001e-151">Response</span></span>

<span data-ttu-id="7001e-152">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7001e-152">The following is an example of a response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7001e-153">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="7001e-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video,Dial-in Microsoft,Dial-out Microsoft
```
