# <a name="reportroot-getskypeforbusinessorganizeractivityusercounts"></a><span data-ttu-id="457f4-101">reportRoot: getSkypeForBusinessOrganizerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="457f4-101">reportRoot: getSkypeForBusinessOrganizerActivityUserCounts</span></span>

<span data-ttu-id="457f4-102">一意のユーザー数と組織内のユーザーが開催、企画した電話会議セッションの数と種類に関する使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="457f4-102">Get usage trends on the number of unique users and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="457f4-103">会議セッションの種類には、IM、オーディオ/ビデオ、アプリケーション共有、Web、サード パーティへのダイヤルイン/ダイヤルアウト、Microsoft へのダイヤルイン/ダイヤルアウトなどがあります。</span><span class="sxs-lookup"><span data-stu-id="457f4-103">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and dial-in/out Microsoft.</span></span>

> <span data-ttu-id="457f4-104">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business 電話会議の開催者のアクティビティ](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="457f4-104">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="457f4-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="457f4-105">Permissions</span></span>

<span data-ttu-id="457f4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="457f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="457f4-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="457f4-108">Permission type</span></span>                        | <span data-ttu-id="457f4-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="457f4-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="457f4-110">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="457f4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="457f4-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="457f4-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="457f4-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="457f4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="457f4-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="457f4-113">Not supported.</span></span>                           |
| <span data-ttu-id="457f4-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="457f4-114">Application</span></span>                            | <span data-ttu-id="457f4-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="457f4-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="457f4-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="457f4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="457f4-117">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="457f4-117">Function parameters</span></span>

<span data-ttu-id="457f4-118">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="457f4-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="457f4-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="457f4-119">Parameter</span></span> | <span data-ttu-id="457f4-120">型</span><span class="sxs-lookup"><span data-stu-id="457f4-120">Type</span></span>   | <span data-ttu-id="457f4-121">説明</span><span class="sxs-lookup"><span data-stu-id="457f4-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="457f4-122">期間</span><span class="sxs-lookup"><span data-stu-id="457f4-122">period</span></span>    | <span data-ttu-id="457f4-123">文字列</span><span class="sxs-lookup"><span data-stu-id="457f4-123">string</span></span> | <span data-ttu-id="457f4-124">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="457f4-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="457f4-125">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="457f4-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="457f4-126">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="457f4-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="457f4-127">必須。</span><span class="sxs-lookup"><span data-stu-id="457f4-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="457f4-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="457f4-128">Request headers</span></span>

| <span data-ttu-id="457f4-129">名前</span><span class="sxs-lookup"><span data-stu-id="457f4-129">Name</span></span>          | <span data-ttu-id="457f4-130">説明</span><span class="sxs-lookup"><span data-stu-id="457f4-130">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="457f4-131">承認</span><span class="sxs-lookup"><span data-stu-id="457f4-131">Authorization</span></span> | <span data-ttu-id="457f4-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="457f4-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="457f4-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="457f4-134">If-None-Match</span></span> | <span data-ttu-id="457f4-135">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="457f4-135">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="457f4-136">省略可能。</span><span class="sxs-lookup"><span data-stu-id="457f4-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="457f4-137">応答</span><span class="sxs-lookup"><span data-stu-id="457f4-137">Response</span></span>

<span data-ttu-id="457f4-138">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="457f4-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="457f4-139">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="457f4-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="457f4-140">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="457f4-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="457f4-141">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="457f4-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="457f4-142">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="457f4-142">Report Refresh Date</span></span>
- <span data-ttu-id="457f4-143">レポート日付</span><span class="sxs-lookup"><span data-stu-id="457f4-143">Report Date</span></span>
- <span data-ttu-id="457f4-144">レポート期間</span><span class="sxs-lookup"><span data-stu-id="457f4-144">Report Period</span></span>
- <span data-ttu-id="457f4-145">IM</span><span class="sxs-lookup"><span data-stu-id="457f4-145">IM</span></span>
- <span data-ttu-id="457f4-146">オーディオ/ビデオ</span><span class="sxs-lookup"><span data-stu-id="457f4-146">Audio/Video</span></span>
- <span data-ttu-id="457f4-147">アプリ共有</span><span class="sxs-lookup"><span data-stu-id="457f4-147">App Sharing</span></span>
- <span data-ttu-id="457f4-148">Web</span><span class="sxs-lookup"><span data-stu-id="457f4-148">Web</span></span>
- <span data-ttu-id="457f4-149">サード パーティのダイヤルイン/アウト</span><span class="sxs-lookup"><span data-stu-id="457f4-149">Dial-in/out 3rd Party</span></span>
- <span data-ttu-id="457f4-150">Microsoft へのダイヤルイン/アウト</span><span class="sxs-lookup"><span data-stu-id="457f4-150">Dial-in/out Microsoft</span></span>

## <a name="example"></a><span data-ttu-id="457f4-151">例</span><span class="sxs-lookup"><span data-stu-id="457f4-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="457f4-152">要求</span><span class="sxs-lookup"><span data-stu-id="457f4-152">Request</span></span>

<span data-ttu-id="457f4-153">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="457f4-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessorganizeractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessOrganizerActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="457f4-154">応答</span><span class="sxs-lookup"><span data-stu-id="457f4-154">Response</span></span>

<span data-ttu-id="457f4-155">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="457f4-155">The following is an example of the response.</span></span>

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

<span data-ttu-id="457f4-156">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="457f4-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party,Dial-in/out Microsoft
```
