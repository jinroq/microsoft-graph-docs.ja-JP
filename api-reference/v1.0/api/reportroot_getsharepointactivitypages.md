# <a name="reportroot-getsharepointactivitypages"></a><span data-ttu-id="261b7-101">reportRoot: getSharePointActivityPages</span><span class="sxs-lookup"><span data-stu-id="261b7-101">reportRoot: getSharePointActivityPages</span></span>

<span data-ttu-id="261b7-102">ユーザーがアクセスしたそれぞれ別個のページ数を取得します。</span><span class="sxs-lookup"><span data-stu-id="261b7-102">Get the number of unique pages visited by users.</span></span>

> <span data-ttu-id="261b7-103">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint アクティビティ](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="261b7-103">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="261b7-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="261b7-104">Permissions</span></span>

<span data-ttu-id="261b7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="261b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="261b7-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="261b7-107">Permission type</span></span>                        | <span data-ttu-id="261b7-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="261b7-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="261b7-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="261b7-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="261b7-110">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="261b7-110">Not supported.</span></span>                           |
| <span data-ttu-id="261b7-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="261b7-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="261b7-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="261b7-112">Not supported.</span></span>                           |
| <span data-ttu-id="261b7-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="261b7-113">Application</span></span>                            | <span data-ttu-id="261b7-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="261b7-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="261b7-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="261b7-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityPages(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="261b7-116">要求パラメーター</span><span class="sxs-lookup"><span data-stu-id="261b7-116">Request parameters</span></span>

<span data-ttu-id="261b7-117">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="261b7-117">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="261b7-118">パラメーター</span><span class="sxs-lookup"><span data-stu-id="261b7-118">Parameter</span></span> | <span data-ttu-id="261b7-119">型</span><span class="sxs-lookup"><span data-stu-id="261b7-119">Type</span></span>   | <span data-ttu-id="261b7-120">説明</span><span class="sxs-lookup"><span data-stu-id="261b7-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="261b7-121">period</span><span class="sxs-lookup"><span data-stu-id="261b7-121">period</span></span>    | <span data-ttu-id="261b7-122">文字列</span><span class="sxs-lookup"><span data-stu-id="261b7-122">string</span></span> | <span data-ttu-id="261b7-123">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="261b7-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="261b7-124">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="261b7-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="261b7-125">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="261b7-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="261b7-126">必須。</span><span class="sxs-lookup"><span data-stu-id="261b7-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="261b7-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="261b7-127">Request headers</span></span>

| <span data-ttu-id="261b7-128">名前</span><span class="sxs-lookup"><span data-stu-id="261b7-128">Name</span></span>          | <span data-ttu-id="261b7-129">説明</span><span class="sxs-lookup"><span data-stu-id="261b7-129">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="261b7-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="261b7-130">Authorization</span></span> | <span data-ttu-id="261b7-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="261b7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="261b7-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="261b7-133">If-None-Match</span></span> | <span data-ttu-id="261b7-134">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="261b7-134">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="261b7-135">省略可能。</span><span class="sxs-lookup"><span data-stu-id="261b7-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="261b7-136">応答</span><span class="sxs-lookup"><span data-stu-id="261b7-136">Response</span></span>

<span data-ttu-id="261b7-137">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="261b7-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="261b7-138">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="261b7-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="261b7-139">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="261b7-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="261b7-140">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="261b7-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="261b7-141">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="261b7-141">Report Refresh Date</span></span>
- <span data-ttu-id="261b7-142">アクセスしたページ数</span><span class="sxs-lookup"><span data-stu-id="261b7-142">Visited Page Count</span></span>
- <span data-ttu-id="261b7-143">レポート日付</span><span class="sxs-lookup"><span data-stu-id="261b7-143">Report Date</span></span>
- <span data-ttu-id="261b7-144">レポート期間</span><span class="sxs-lookup"><span data-stu-id="261b7-144">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="261b7-145">例</span><span class="sxs-lookup"><span data-stu-id="261b7-145">Example</span></span>

#### <a name="request"></a><span data-ttu-id="261b7-146">要求</span><span class="sxs-lookup"><span data-stu-id="261b7-146">Request</span></span>

<span data-ttu-id="261b7-147">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="261b7-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivitypages"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityPages(period='D7')
```

#### <a name="response"></a><span data-ttu-id="261b7-148">応答</span><span class="sxs-lookup"><span data-stu-id="261b7-148">Response</span></span>

<span data-ttu-id="261b7-149">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="261b7-149">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="261b7-150">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="261b7-150">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page Count,Report Date,Report Period
```
