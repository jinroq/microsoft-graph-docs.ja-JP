# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="a08cf-101">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="a08cf-101">reportRoot: getOffice365ActiveUserCounts</span></span>

<span data-ttu-id="a08cf-102">レポート期間中の日ごとのアクティブ ユーザー数を製品別に取得します。</span><span class="sxs-lookup"><span data-stu-id="a08cf-102">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="a08cf-103">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: アクティブ ユーザー](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a08cf-103">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="a08cf-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a08cf-104">Permissions</span></span>

<span data-ttu-id="a08cf-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a08cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="a08cf-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a08cf-107">Permission type</span></span>                        | <span data-ttu-id="a08cf-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a08cf-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a08cf-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="a08cf-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="a08cf-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a08cf-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a08cf-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a08cf-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a08cf-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a08cf-112">Not supported.</span></span>                           |
| <span data-ttu-id="a08cf-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a08cf-113">Application</span></span>                            | <span data-ttu-id="a08cf-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a08cf-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a08cf-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a08cf-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a08cf-116">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="a08cf-116">Function parameters</span></span>

<span data-ttu-id="a08cf-117">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="a08cf-117">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a08cf-118">パラメーター</span><span class="sxs-lookup"><span data-stu-id="a08cf-118">Parameter</span></span> | <span data-ttu-id="a08cf-119">型</span><span class="sxs-lookup"><span data-stu-id="a08cf-119">Type</span></span>   | <span data-ttu-id="a08cf-120">説明</span><span class="sxs-lookup"><span data-stu-id="a08cf-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a08cf-121">期間</span><span class="sxs-lookup"><span data-stu-id="a08cf-121">period</span></span>    | <span data-ttu-id="a08cf-122">文字列</span><span class="sxs-lookup"><span data-stu-id="a08cf-122">string</span></span> | <span data-ttu-id="a08cf-123">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="a08cf-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a08cf-124">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="a08cf-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a08cf-125">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="a08cf-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a08cf-126">必須。</span><span class="sxs-lookup"><span data-stu-id="a08cf-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="a08cf-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a08cf-127">Request headers</span></span>

| <span data-ttu-id="a08cf-128">名前</span><span class="sxs-lookup"><span data-stu-id="a08cf-128">Name</span></span>          | <span data-ttu-id="a08cf-129">説明</span><span class="sxs-lookup"><span data-stu-id="a08cf-129">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a08cf-130">承認</span><span class="sxs-lookup"><span data-stu-id="a08cf-130">Authorization</span></span> | <span data-ttu-id="a08cf-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a08cf-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a08cf-133">応答</span><span class="sxs-lookup"><span data-stu-id="a08cf-133">Response</span></span>

<span data-ttu-id="a08cf-134">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="a08cf-134">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a08cf-135">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="a08cf-135">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a08cf-136">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="a08cf-136">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a08cf-137">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="a08cf-137">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a08cf-138">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="a08cf-138">Report Refresh Date</span></span>
- <span data-ttu-id="a08cf-139">Office 365</span><span class="sxs-lookup"><span data-stu-id="a08cf-139">Office 365</span></span>
- <span data-ttu-id="a08cf-140">Exchange</span><span class="sxs-lookup"><span data-stu-id="a08cf-140">Exchange</span></span>
- <span data-ttu-id="a08cf-141">OneDrive</span><span class="sxs-lookup"><span data-stu-id="a08cf-141">OneDrive</span></span>
- <span data-ttu-id="a08cf-142">SharePoint</span><span class="sxs-lookup"><span data-stu-id="a08cf-142">SharePoint</span></span>
- <span data-ttu-id="a08cf-143">Skype For Business</span><span class="sxs-lookup"><span data-stu-id="a08cf-143">Skype For Business</span></span> 
- <span data-ttu-id="a08cf-144">Yammer</span><span class="sxs-lookup"><span data-stu-id="a08cf-144">Yammer</span></span>
- <span data-ttu-id="a08cf-145">Teams</span><span class="sxs-lookup"><span data-stu-id="a08cf-145">Teams</span></span>
- <span data-ttu-id="a08cf-146">レポート日付</span><span class="sxs-lookup"><span data-stu-id="a08cf-146">Report Date</span></span>
- <span data-ttu-id="a08cf-147">レポート期間</span><span class="sxs-lookup"><span data-stu-id="a08cf-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="a08cf-148">例</span><span class="sxs-lookup"><span data-stu-id="a08cf-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a08cf-149">要求</span><span class="sxs-lookup"><span data-stu-id="a08cf-149">Request</span></span>

<span data-ttu-id="a08cf-150">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a08cf-150">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="a08cf-151">応答</span><span class="sxs-lookup"><span data-stu-id="a08cf-151">Response</span></span>

<span data-ttu-id="a08cf-152">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a08cf-152">The following is an example of the response.</span></span>

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

<span data-ttu-id="a08cf-153">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="a08cf-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Office 365,Exchange,OneDrive,SharePoint,Skype For Business,Yammer,Teams,Report Date,Report Period
```
