# <a name="reportroot-getonedriveactivityusercounts"></a><span data-ttu-id="9a149-101">reportRoot: getOneDriveActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="9a149-101">reportRoot: getOneDriveActivityUserCounts</span></span>

<span data-ttu-id="9a149-102">アクティブな OneDrive ユーザーの数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="9a149-102">Get the trend in the number of active OneDrive users.</span></span>

> <span data-ttu-id="9a149-103">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business のアクティビティ](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a149-103">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="9a149-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9a149-104">Permissions</span></span>

<span data-ttu-id="9a149-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a149-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="9a149-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9a149-107">Permission type</span></span>                        | <span data-ttu-id="9a149-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9a149-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9a149-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9a149-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="9a149-110">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a149-110">Not supported.</span></span>                           |
| <span data-ttu-id="9a149-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9a149-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a149-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a149-112">Not supported.</span></span>                           |
| <span data-ttu-id="9a149-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9a149-113">Application</span></span>                            | <span data-ttu-id="9a149-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a149-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="9a149-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9a149-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="9a149-116">要求パラメーター</span><span class="sxs-lookup"><span data-stu-id="9a149-116">Request parameters</span></span>

<span data-ttu-id="9a149-117">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="9a149-117">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="9a149-118">パラメーター</span><span class="sxs-lookup"><span data-stu-id="9a149-118">Parameter</span></span> | <span data-ttu-id="9a149-119">型</span><span class="sxs-lookup"><span data-stu-id="9a149-119">Type</span></span>   | <span data-ttu-id="9a149-120">説明</span><span class="sxs-lookup"><span data-stu-id="9a149-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9a149-121">period</span><span class="sxs-lookup"><span data-stu-id="9a149-121">period</span></span>    | <span data-ttu-id="9a149-122">文字列</span><span class="sxs-lookup"><span data-stu-id="9a149-122">string</span></span> | <span data-ttu-id="9a149-123">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="9a149-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9a149-124">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="9a149-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9a149-125">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="9a149-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="9a149-126">必須。</span><span class="sxs-lookup"><span data-stu-id="9a149-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="9a149-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a149-127">Request headers</span></span>

| <span data-ttu-id="9a149-128">名前</span><span class="sxs-lookup"><span data-stu-id="9a149-128">Name</span></span>          | <span data-ttu-id="9a149-129">説明</span><span class="sxs-lookup"><span data-stu-id="9a149-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="9a149-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a149-130">Authorization</span></span> | <span data-ttu-id="9a149-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9a149-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="9a149-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="9a149-133">If-None-Match</span></span> | <span data-ttu-id="9a149-134">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="9a149-134">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="9a149-135">省略可能。</span><span class="sxs-lookup"><span data-stu-id="9a149-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="9a149-136">応答</span><span class="sxs-lookup"><span data-stu-id="9a149-136">Response</span></span>

<span data-ttu-id="9a149-137">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="9a149-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9a149-138">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="9a149-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9a149-139">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="9a149-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9a149-140">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="9a149-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9a149-141">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="9a149-141">Report Refresh Date</span></span>
- <span data-ttu-id="9a149-142">表示済みまたは編集済み</span><span class="sxs-lookup"><span data-stu-id="9a149-142">Viewed Or Edited</span></span>
- <span data-ttu-id="9a149-143">同期済み</span><span class="sxs-lookup"><span data-stu-id="9a149-143">Synced</span></span>
- <span data-ttu-id="9a149-144">社内で共有済み</span><span class="sxs-lookup"><span data-stu-id="9a149-144">Shared Internally</span></span>
- <span data-ttu-id="9a149-145">外部で共有済み</span><span class="sxs-lookup"><span data-stu-id="9a149-145">Shared Externally</span></span>
- <span data-ttu-id="9a149-146">レポート日付</span><span class="sxs-lookup"><span data-stu-id="9a149-146">Report Date</span></span>
- <span data-ttu-id="9a149-147">レポート期間</span><span class="sxs-lookup"><span data-stu-id="9a149-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="9a149-148">例</span><span class="sxs-lookup"><span data-stu-id="9a149-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9a149-149">要求</span><span class="sxs-lookup"><span data-stu-id="9a149-149">Request</span></span>

<span data-ttu-id="9a149-150">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9a149-150">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="9a149-151">応答</span><span class="sxs-lookup"><span data-stu-id="9a149-151">Response</span></span>

<span data-ttu-id="9a149-152">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9a149-152">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="9a149-153">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="9a149-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```
