# <a name="reportroot-getsharepointsiteusagesitecounts"></a><span data-ttu-id="1312d-101">reportRoot: getSharePointSiteUsageSiteCounts</span><span class="sxs-lookup"><span data-stu-id="1312d-101">reportRoot: getSharePointSiteUsageSiteCounts</span></span>

<span data-ttu-id="1312d-102">すべてのサイトのファイルの合計数と、アクティブ ファイルの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="1312d-102">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="1312d-103">ファイル (ユーザーまたはシステム) は、一定期間中に保存、同期、変更、共有されるとアクティブとみなされます。</span><span class="sxs-lookup"><span data-stu-id="1312d-103">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="1312d-104">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint サイトの使用状況](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1312d-104">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="1312d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1312d-105">Permissions</span></span>

<span data-ttu-id="1312d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1312d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="1312d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1312d-108">Permission type</span></span>                        | <span data-ttu-id="1312d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1312d-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1312d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1312d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1312d-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1312d-111">Not supported.</span></span>                           |
| <span data-ttu-id="1312d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1312d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1312d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1312d-113">Not supported.</span></span>                           |
| <span data-ttu-id="1312d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1312d-114">Application</span></span>                            | <span data-ttu-id="1312d-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1312d-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1312d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1312d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageSiteCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="1312d-117">要求パラメーター</span><span class="sxs-lookup"><span data-stu-id="1312d-117">Request parameters</span></span>

<span data-ttu-id="1312d-118">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="1312d-118">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="1312d-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="1312d-119">Parameter</span></span> | <span data-ttu-id="1312d-120">型</span><span class="sxs-lookup"><span data-stu-id="1312d-120">Type</span></span>   | <span data-ttu-id="1312d-121">説明</span><span class="sxs-lookup"><span data-stu-id="1312d-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1312d-122">period</span><span class="sxs-lookup"><span data-stu-id="1312d-122">period</span></span>    | <span data-ttu-id="1312d-123">文字列</span><span class="sxs-lookup"><span data-stu-id="1312d-123">string</span></span> | <span data-ttu-id="1312d-124">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="1312d-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1312d-125">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="1312d-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1312d-126">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="1312d-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="1312d-127">必須。</span><span class="sxs-lookup"><span data-stu-id="1312d-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="1312d-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1312d-128">Request headers</span></span>

| <span data-ttu-id="1312d-129">名前</span><span class="sxs-lookup"><span data-stu-id="1312d-129">Name</span></span>          | <span data-ttu-id="1312d-130">説明</span><span class="sxs-lookup"><span data-stu-id="1312d-130">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1312d-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="1312d-131">Authorization</span></span> | <span data-ttu-id="1312d-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1312d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1312d-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="1312d-134">If-None-Match</span></span> | <span data-ttu-id="1312d-135">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="1312d-135">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="1312d-136">省略可能。</span><span class="sxs-lookup"><span data-stu-id="1312d-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="1312d-137">応答</span><span class="sxs-lookup"><span data-stu-id="1312d-137">Response</span></span>

<span data-ttu-id="1312d-138">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="1312d-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1312d-139">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="1312d-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1312d-140">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="1312d-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1312d-141">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="1312d-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1312d-142">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="1312d-142">Report Refresh Date</span></span>
- <span data-ttu-id="1312d-143">サイトの種類</span><span class="sxs-lookup"><span data-stu-id="1312d-143">Site Type</span></span>
- <span data-ttu-id="1312d-144">合計</span><span class="sxs-lookup"><span data-stu-id="1312d-144">Total</span></span>
- <span data-ttu-id="1312d-145">アクティブ</span><span class="sxs-lookup"><span data-stu-id="1312d-145">Active</span></span>
- <span data-ttu-id="1312d-146">レポート日付</span><span class="sxs-lookup"><span data-stu-id="1312d-146">Report Date</span></span>
- <span data-ttu-id="1312d-147">レポート期間</span><span class="sxs-lookup"><span data-stu-id="1312d-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="1312d-148">例</span><span class="sxs-lookup"><span data-stu-id="1312d-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1312d-149">要求</span><span class="sxs-lookup"><span data-stu-id="1312d-149">Request</span></span>

<span data-ttu-id="1312d-150">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1312d-150">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagesitecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageSiteCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="1312d-151">応答</span><span class="sxs-lookup"><span data-stu-id="1312d-151">Response</span></span>

<span data-ttu-id="1312d-152">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1312d-152">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="1312d-153">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="1312d-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```
