# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="0fbca-101">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="0fbca-101">reportRoot: getSharePointActivityUserCounts</span></span>

<span data-ttu-id="0fbca-102">アクティブ ユーザーの数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="0fbca-102">Get the trend in the number of active users.</span></span> <span data-ttu-id="0fbca-103">ユーザーが一定期間中にファイル アクティビティ (保存、同期、変更、共有) を実行するか、またはページにアクセスすると、そのユーザーはアクティブとみなされます。</span><span class="sxs-lookup"><span data-stu-id="0fbca-103">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="0fbca-104">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint アクティビティ](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0fbca-104">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="0fbca-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0fbca-105">Permissions</span></span>

<span data-ttu-id="0fbca-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0fbca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="0fbca-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0fbca-108">Permission type</span></span>                        | <span data-ttu-id="0fbca-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0fbca-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0fbca-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0fbca-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0fbca-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0fbca-111">Not supported.</span></span>                           |
| <span data-ttu-id="0fbca-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0fbca-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fbca-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0fbca-113">Not supported.</span></span>                           |
| <span data-ttu-id="0fbca-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0fbca-114">Application</span></span>                            | <span data-ttu-id="0fbca-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0fbca-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0fbca-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0fbca-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="0fbca-117">要求パラメーター</span><span class="sxs-lookup"><span data-stu-id="0fbca-117">Request parameters</span></span>

<span data-ttu-id="0fbca-118">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="0fbca-118">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="0fbca-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="0fbca-119">Parameter</span></span> | <span data-ttu-id="0fbca-120">型</span><span class="sxs-lookup"><span data-stu-id="0fbca-120">Type</span></span>   | <span data-ttu-id="0fbca-121">説明</span><span class="sxs-lookup"><span data-stu-id="0fbca-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0fbca-122">period</span><span class="sxs-lookup"><span data-stu-id="0fbca-122">period</span></span>    | <span data-ttu-id="0fbca-123">文字列</span><span class="sxs-lookup"><span data-stu-id="0fbca-123">string</span></span> | <span data-ttu-id="0fbca-124">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="0fbca-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0fbca-125">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="0fbca-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0fbca-126">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="0fbca-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="0fbca-127">必須。</span><span class="sxs-lookup"><span data-stu-id="0fbca-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="0fbca-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0fbca-128">Request headers</span></span>

| <span data-ttu-id="0fbca-129">名前</span><span class="sxs-lookup"><span data-stu-id="0fbca-129">Name</span></span>          | <span data-ttu-id="0fbca-130">説明</span><span class="sxs-lookup"><span data-stu-id="0fbca-130">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0fbca-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fbca-131">Authorization</span></span> | <span data-ttu-id="0fbca-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0fbca-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0fbca-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="0fbca-134">If-None-Match</span></span> | <span data-ttu-id="0fbca-135">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="0fbca-135">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="0fbca-136">省略可能。</span><span class="sxs-lookup"><span data-stu-id="0fbca-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="0fbca-137">応答</span><span class="sxs-lookup"><span data-stu-id="0fbca-137">Response</span></span>

<span data-ttu-id="0fbca-138">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="0fbca-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0fbca-139">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="0fbca-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0fbca-140">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="0fbca-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0fbca-141">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="0fbca-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0fbca-142">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="0fbca-142">Report Refresh Date</span></span>
- <span data-ttu-id="0fbca-143">アクセスしたページ</span><span class="sxs-lookup"><span data-stu-id="0fbca-143">Visited Page</span></span>
- <span data-ttu-id="0fbca-144">表示済みまたは編集済み</span><span class="sxs-lookup"><span data-stu-id="0fbca-144">Viewed Or Edited</span></span>
- <span data-ttu-id="0fbca-145">同期済み</span><span class="sxs-lookup"><span data-stu-id="0fbca-145">Synced</span></span>
- <span data-ttu-id="0fbca-146">社内で共有済み</span><span class="sxs-lookup"><span data-stu-id="0fbca-146">Shared Internally</span></span>
- <span data-ttu-id="0fbca-147">外部で共有済み</span><span class="sxs-lookup"><span data-stu-id="0fbca-147">Shared Externally</span></span>
- <span data-ttu-id="0fbca-148">レポート日付</span><span class="sxs-lookup"><span data-stu-id="0fbca-148">Report Date</span></span>
- <span data-ttu-id="0fbca-149">レポート期間</span><span class="sxs-lookup"><span data-stu-id="0fbca-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="0fbca-150">例</span><span class="sxs-lookup"><span data-stu-id="0fbca-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0fbca-151">要求</span><span class="sxs-lookup"><span data-stu-id="0fbca-151">Request</span></span>

<span data-ttu-id="0fbca-152">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0fbca-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="0fbca-153">応答</span><span class="sxs-lookup"><span data-stu-id="0fbca-153">Response</span></span>

<span data-ttu-id="0fbca-154">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0fbca-154">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="0fbca-155">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="0fbca-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```
