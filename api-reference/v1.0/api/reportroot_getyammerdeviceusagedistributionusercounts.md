# <a name="reportroot-getyammerdeviceusagedistributionusercounts"></a><span data-ttu-id="6db36-101">reportRoot: getYammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="6db36-101">reportRoot: getYammerDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="6db36-102">デバイスの種類別にユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="6db36-102">Get the number of users by device type.</span></span>

> <span data-ttu-id="6db36-103">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer デバイスの使用状況](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6db36-103">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="6db36-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6db36-104">Permissions</span></span>

<span data-ttu-id="6db36-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6db36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="6db36-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6db36-107">Permission type</span></span>                        | <span data-ttu-id="6db36-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6db36-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6db36-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="6db36-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="6db36-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6db36-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6db36-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6db36-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6db36-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6db36-112">Not supported.</span></span>                           |
| <span data-ttu-id="6db36-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6db36-113">Application</span></span>                            | <span data-ttu-id="6db36-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6db36-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6db36-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6db36-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="6db36-116">要求パラメーター</span><span class="sxs-lookup"><span data-stu-id="6db36-116">Request parameters</span></span>

<span data-ttu-id="6db36-117">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="6db36-117">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="6db36-118">パラメーター</span><span class="sxs-lookup"><span data-stu-id="6db36-118">Parameter</span></span> | <span data-ttu-id="6db36-119">型</span><span class="sxs-lookup"><span data-stu-id="6db36-119">Type</span></span>   | <span data-ttu-id="6db36-120">説明</span><span class="sxs-lookup"><span data-stu-id="6db36-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6db36-121">period</span><span class="sxs-lookup"><span data-stu-id="6db36-121">period</span></span>    | <span data-ttu-id="6db36-122">文字列</span><span class="sxs-lookup"><span data-stu-id="6db36-122">string</span></span> | <span data-ttu-id="6db36-123">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="6db36-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6db36-124">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="6db36-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6db36-125">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="6db36-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="6db36-126">必須。</span><span class="sxs-lookup"><span data-stu-id="6db36-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="6db36-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6db36-127">Request headers</span></span>

| <span data-ttu-id="6db36-128">名前</span><span class="sxs-lookup"><span data-stu-id="6db36-128">Name</span></span>          | <span data-ttu-id="6db36-129">説明</span><span class="sxs-lookup"><span data-stu-id="6db36-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="6db36-130">承認</span><span class="sxs-lookup"><span data-stu-id="6db36-130">Authorization</span></span> | <span data-ttu-id="6db36-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6db36-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="6db36-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="6db36-133">If-None-Match</span></span> | <span data-ttu-id="6db36-134">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="6db36-134">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="6db36-135">省略可能。</span><span class="sxs-lookup"><span data-stu-id="6db36-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="6db36-136">応答</span><span class="sxs-lookup"><span data-stu-id="6db36-136">Response</span></span>

<span data-ttu-id="6db36-137">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="6db36-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6db36-138">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="6db36-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6db36-139">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="6db36-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6db36-140">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="6db36-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6db36-141">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="6db36-141">Report Refresh Date</span></span>
- <span data-ttu-id="6db36-142">Web</span><span class="sxs-lookup"><span data-stu-id="6db36-142">Web</span></span>
- <span data-ttu-id="6db36-143">Windows スマートフォン</span><span class="sxs-lookup"><span data-stu-id="6db36-143">Windows Phone</span></span>
- <span data-ttu-id="6db36-144">Android スマートフォン</span><span class="sxs-lookup"><span data-stu-id="6db36-144">Android Phone</span></span>
- <span data-ttu-id="6db36-145">iPhone</span><span class="sxs-lookup"><span data-stu-id="6db36-145">iPhone</span></span>
- <span data-ttu-id="6db36-146">iPad</span><span class="sxs-lookup"><span data-stu-id="6db36-146">iPad</span></span>
- <span data-ttu-id="6db36-147">その他</span><span class="sxs-lookup"><span data-stu-id="6db36-147">Other</span></span>
- <span data-ttu-id="6db36-148">レポート期間</span><span class="sxs-lookup"><span data-stu-id="6db36-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="6db36-149">例</span><span class="sxs-lookup"><span data-stu-id="6db36-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6db36-150">要求</span><span class="sxs-lookup"><span data-stu-id="6db36-150">Request</span></span>

<span data-ttu-id="6db36-151">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6db36-151">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusagedistributionusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="6db36-152">応答</span><span class="sxs-lookup"><span data-stu-id="6db36-152">Response</span></span>

<span data-ttu-id="6db36-153">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6db36-153">The following is an example of the response.</span></span>

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

<span data-ttu-id="6db36-154">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="6db36-154">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Period
```
