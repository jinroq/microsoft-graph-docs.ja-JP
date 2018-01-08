# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="2c51a-101">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="2c51a-101">reportRoot: getOffice365ServicesUserCounts</span></span>

<span data-ttu-id="2c51a-102">アクティビティの種類とサービス別のユーザー数を取得します。</span><span class="sxs-lookup"><span data-stu-id="2c51a-102">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="2c51a-103">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: アクティブ ユーザー]((https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d))」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2c51a-103">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users]((https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)).</span></span>

## <a name="permissions"></a><span data-ttu-id="2c51a-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2c51a-104">Permissions</span></span>

<span data-ttu-id="2c51a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2c51a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="2c51a-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2c51a-107">Permission type</span></span>                        | <span data-ttu-id="2c51a-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2c51a-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2c51a-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2c51a-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="2c51a-110">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2c51a-110">Not supported.</span></span>                           |
| <span data-ttu-id="2c51a-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2c51a-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c51a-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2c51a-112">Not supported.</span></span>                           |
| <span data-ttu-id="2c51a-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2c51a-113">Application</span></span>                            | <span data-ttu-id="2c51a-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c51a-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2c51a-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2c51a-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="2c51a-116">要求パラメーター</span><span class="sxs-lookup"><span data-stu-id="2c51a-116">Request parameters</span></span>

<span data-ttu-id="2c51a-117">要求 URL に、次のクエリ パラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="2c51a-117">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="2c51a-118">パラメーター</span><span class="sxs-lookup"><span data-stu-id="2c51a-118">Parameter</span></span> | <span data-ttu-id="2c51a-119">型</span><span class="sxs-lookup"><span data-stu-id="2c51a-119">Type</span></span>   | <span data-ttu-id="2c51a-120">説明</span><span class="sxs-lookup"><span data-stu-id="2c51a-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2c51a-121">period</span><span class="sxs-lookup"><span data-stu-id="2c51a-121">period</span></span>    | <span data-ttu-id="2c51a-122">文字列</span><span class="sxs-lookup"><span data-stu-id="2c51a-122">string</span></span> | <span data-ttu-id="2c51a-123">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="2c51a-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2c51a-124">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="2c51a-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2c51a-125">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="2c51a-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="2c51a-126">必須。</span><span class="sxs-lookup"><span data-stu-id="2c51a-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="2c51a-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2c51a-127">Request headers</span></span>

| <span data-ttu-id="2c51a-128">名前</span><span class="sxs-lookup"><span data-stu-id="2c51a-128">Name</span></span>          | <span data-ttu-id="2c51a-129">説明</span><span class="sxs-lookup"><span data-stu-id="2c51a-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="2c51a-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c51a-130">Authorization</span></span> | <span data-ttu-id="2c51a-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2c51a-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="2c51a-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="2c51a-133">if-none-match</span></span> | <span data-ttu-id="2c51a-134">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="2c51a-134">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="2c51a-135">省略可能。</span><span class="sxs-lookup"><span data-stu-id="2c51a-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="2c51a-136">応答</span><span class="sxs-lookup"><span data-stu-id="2c51a-136">Response</span></span>

<span data-ttu-id="2c51a-137">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="2c51a-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2c51a-138">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="2c51a-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2c51a-139">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="2c51a-139">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="2c51a-140">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="2c51a-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2c51a-141">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="2c51a-141">Report Refresh Date</span></span>
- <span data-ttu-id="2c51a-142">Exchange アクティブ</span><span class="sxs-lookup"><span data-stu-id="2c51a-142">Exchange Active</span></span>
- <span data-ttu-id="2c51a-143">Exchange 非アクティブ</span><span class="sxs-lookup"><span data-stu-id="2c51a-143">Exchange Inactive</span></span>
- <span data-ttu-id="2c51a-144">OneDrive アクティブ</span><span class="sxs-lookup"><span data-stu-id="2c51a-144">OneDrive Active</span></span>
- <span data-ttu-id="2c51a-145">OneDrive 非アクティブ</span><span class="sxs-lookup"><span data-stu-id="2c51a-145">OneDrive Inactive</span></span>
- <span data-ttu-id="2c51a-146">SharePoint アクティブ</span><span class="sxs-lookup"><span data-stu-id="2c51a-146">SharePoint Online Active User*</span></span>
- <span data-ttu-id="2c51a-147">SharePoint 非アクティブ</span><span class="sxs-lookup"><span data-stu-id="2c51a-147">SharePoint Inactive</span></span>
- <span data-ttu-id="2c51a-148">Skype For Business アクティブ</span><span class="sxs-lookup"><span data-stu-id="2c51a-148">Skype For Business Active</span></span>
- <span data-ttu-id="2c51a-149">Skype For Business 非アクティブ</span><span class="sxs-lookup"><span data-stu-id="2c51a-149">Skype For Business Inactive</span></span>
- <span data-ttu-id="2c51a-150">Yammer アクティブ</span><span class="sxs-lookup"><span data-stu-id="2c51a-150">Yammer Active</span></span>
- <span data-ttu-id="2c51a-151">Yammer 非アクティブ</span><span class="sxs-lookup"><span data-stu-id="2c51a-151">Yammer Inactive</span></span>
- <span data-ttu-id="2c51a-152">Teams アクティブ</span><span class="sxs-lookup"><span data-stu-id="2c51a-152">Teams Active</span></span>
- <span data-ttu-id="2c51a-153">Teams 非アクティブ</span><span class="sxs-lookup"><span data-stu-id="2c51a-153">Teams Inactive</span></span>
- <span data-ttu-id="2c51a-154">レポート期間</span><span class="sxs-lookup"><span data-stu-id="2c51a-154">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="2c51a-155">例</span><span class="sxs-lookup"><span data-stu-id="2c51a-155">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2c51a-156">要求</span><span class="sxs-lookup"><span data-stu-id="2c51a-156">Request</span></span>

<span data-ttu-id="2c51a-157">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2c51a-157">The following is an example of the request body.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ServicesUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="2c51a-158">応答</span><span class="sxs-lookup"><span data-stu-id="2c51a-158">Response</span></span>

<span data-ttu-id="2c51a-159">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2c51a-159">The following is an example of a response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="2c51a-160">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="2c51a-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Active,Exchange Inactive,OneDrive Active,OneDrive Inactive,SharePoint Active,SharePoint Inactive,Skype For Business Active,Skype For Business Inactive,Yammer Active,Yammer Inactive,Teams Active,Teams Inactive,Report Period
```
