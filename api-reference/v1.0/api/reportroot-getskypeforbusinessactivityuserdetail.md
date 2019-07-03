---
title: 'reportRoot: getSkypeForBusinessActivityUserDetail'
description: ユーザー別の Skype for Business アクティビティに関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: ba15c78416f9155487c479470bcd284701dc8ede
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35446102"
---
# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="08d56-103">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="08d56-103">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

<span data-ttu-id="08d56-104">ユーザー別の Skype for Business アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="08d56-104">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="08d56-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business アクティビティ](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="08d56-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="08d56-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="08d56-106">Permissions</span></span>

<span data-ttu-id="08d56-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="08d56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="08d56-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="08d56-109">Permission type</span></span>                        | <span data-ttu-id="08d56-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="08d56-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="08d56-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="08d56-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="08d56-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="08d56-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="08d56-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="08d56-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08d56-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="08d56-114">Not supported.</span></span>                           |
| <span data-ttu-id="08d56-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="08d56-115">Application</span></span>                            | <span data-ttu-id="08d56-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="08d56-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="08d56-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="08d56-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="08d56-118">プロトコル</span><span class="sxs-lookup"><span data-stu-id="08d56-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="08d56-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="08d56-119">Function parameters</span></span>

<span data-ttu-id="08d56-120">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="08d56-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="08d56-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="08d56-121">Parameter</span></span> | <span data-ttu-id="08d56-122">型</span><span class="sxs-lookup"><span data-stu-id="08d56-122">Type</span></span>   | <span data-ttu-id="08d56-123">説明</span><span class="sxs-lookup"><span data-stu-id="08d56-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="08d56-124">period</span><span class="sxs-lookup"><span data-stu-id="08d56-124">period</span></span>    | <span data-ttu-id="08d56-125">文字列</span><span class="sxs-lookup"><span data-stu-id="08d56-125">string</span></span> | <span data-ttu-id="08d56-126">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="08d56-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="08d56-127">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="08d56-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="08d56-128">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="08d56-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="08d56-129">date</span><span class="sxs-lookup"><span data-stu-id="08d56-129">date</span></span>      | <span data-ttu-id="08d56-130">日付</span><span class="sxs-lookup"><span data-stu-id="08d56-130">Date</span></span>   | <span data-ttu-id="08d56-131">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="08d56-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="08d56-132">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="08d56-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="08d56-133">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="08d56-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="08d56-134">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="08d56-134">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="08d56-135">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="08d56-135">Request headers</span></span>

| <span data-ttu-id="08d56-136">名前</span><span class="sxs-lookup"><span data-stu-id="08d56-136">Name</span></span>          | <span data-ttu-id="08d56-137">説明</span><span class="sxs-lookup"><span data-stu-id="08d56-137">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="08d56-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="08d56-138">Authorization</span></span> | <span data-ttu-id="08d56-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="08d56-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="08d56-141">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="08d56-141">If-None-Match</span></span> | <span data-ttu-id="08d56-142">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="08d56-142">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="08d56-143">省略可能。</span><span class="sxs-lookup"><span data-stu-id="08d56-143">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="08d56-144">応答</span><span class="sxs-lookup"><span data-stu-id="08d56-144">Response</span></span>

<span data-ttu-id="08d56-145">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="08d56-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="08d56-146">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="08d56-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="08d56-147">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="08d56-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="08d56-148">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="08d56-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="08d56-149">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="08d56-149">Report Refresh Date</span></span>
- <span data-ttu-id="08d56-150">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="08d56-150">User Principal Name</span></span>
- <span data-ttu-id="08d56-151">削除済み</span><span class="sxs-lookup"><span data-stu-id="08d56-151">Is Deleted</span></span>
- <span data-ttu-id="08d56-152">削除日</span><span class="sxs-lookup"><span data-stu-id="08d56-152">Deleted Date</span></span>
- <span data-ttu-id="08d56-153">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="08d56-153">Last Activity Date</span></span>
- <span data-ttu-id="08d56-154">ピア ツー ピア セッションの合計数</span><span class="sxs-lookup"><span data-stu-id="08d56-154">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="08d56-155">開催した会議の合計数</span><span class="sxs-lookup"><span data-stu-id="08d56-155">Total Organized Conference Count</span></span>
- <span data-ttu-id="08d56-156">参加した会議の合計数</span><span class="sxs-lookup"><span data-stu-id="08d56-156">Total Participated Conference Count</span></span>
- <span data-ttu-id="08d56-157">ピア ツー ピアの最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="08d56-157">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="08d56-158">開催した会議の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="08d56-158">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="08d56-159">参加した会議の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="08d56-159">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="08d56-160">ピア ツー ピアの IM の数</span><span class="sxs-lookup"><span data-stu-id="08d56-160">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="08d56-161">ピア ツー ピアのオーディオの数</span><span class="sxs-lookup"><span data-stu-id="08d56-161">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="08d56-162">ピア ツー ピアのオーディオの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="08d56-162">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="08d56-163">ピア ツー ピアのビデオの数</span><span class="sxs-lookup"><span data-stu-id="08d56-163">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="08d56-164">ピア ツー ピアのビデオの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="08d56-164">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="08d56-165">ピア ツー ピアのアプリ共有の数</span><span class="sxs-lookup"><span data-stu-id="08d56-165">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="08d56-166">ピア ツー ピアのファイル転送の数</span><span class="sxs-lookup"><span data-stu-id="08d56-166">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="08d56-167">開催した会議の IM の数</span><span class="sxs-lookup"><span data-stu-id="08d56-167">Organized Conference IM Count</span></span>
- <span data-ttu-id="08d56-168">開催した会議のオーディオ/ビデオの数</span><span class="sxs-lookup"><span data-stu-id="08d56-168">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="08d56-169">開催した会議のオーディオ/ビデオの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="08d56-169">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="08d56-170">開催した会議のアプリ共有の数</span><span class="sxs-lookup"><span data-stu-id="08d56-170">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="08d56-171">開催した会議の Web の数</span><span class="sxs-lookup"><span data-stu-id="08d56-171">Organized Conference Web Count</span></span>
- <span data-ttu-id="08d56-172">開催した会議のサード パーティのダイヤルイン/アウトの数</span><span class="sxs-lookup"><span data-stu-id="08d56-172">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="08d56-173">開催した会議の Microsoft のダイヤルイン/アウトの数</span><span class="sxs-lookup"><span data-stu-id="08d56-173">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="08d56-174">開催した会議の Microsoft のダイヤルインの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="08d56-174">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="08d56-175">開催した会議の Microsoft からのダイヤルアウトの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="08d56-175">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="08d56-176">参加した会議の IM の数</span><span class="sxs-lookup"><span data-stu-id="08d56-176">Paricipated Conference IM Count</span></span>
- <span data-ttu-id="08d56-177">参加した会議のオーディオ/ビデオの数</span><span class="sxs-lookup"><span data-stu-id="08d56-177">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="08d56-178">参加した会議のオーディオ/ビデオの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="08d56-178">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="08d56-179">参加した会議のアプリ共有の数</span><span class="sxs-lookup"><span data-stu-id="08d56-179">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="08d56-180">参加した会議の Web の数</span><span class="sxs-lookup"><span data-stu-id="08d56-180">Participated Conference Web Count</span></span>
- <span data-ttu-id="08d56-181">参加した会議のサード パーティのダイヤルイン/アウトの数</span><span class="sxs-lookup"><span data-stu-id="08d56-181">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="08d56-182">割り当て済み製品</span><span class="sxs-lookup"><span data-stu-id="08d56-182">Assigned Products</span></span>
- <span data-ttu-id="08d56-183">レポート期間</span><span class="sxs-lookup"><span data-stu-id="08d56-183">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="08d56-184">例</span><span class="sxs-lookup"><span data-stu-id="08d56-184">Example</span></span>

#### <a name="request"></a><span data-ttu-id="08d56-185">要求</span><span class="sxs-lookup"><span data-stu-id="08d56-185">Request</span></span>

<span data-ttu-id="08d56-186">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="08d56-186">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessActivityUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="08d56-187">C#</span><span class="sxs-lookup"><span data-stu-id="08d56-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessactivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="08d56-188">Javascript</span><span class="sxs-lookup"><span data-stu-id="08d56-188">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessactivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="08d56-189">目的-C</span><span class="sxs-lookup"><span data-stu-id="08d56-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessactivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="08d56-190">応答</span><span class="sxs-lookup"><span data-stu-id="08d56-190">Response</span></span>

<span data-ttu-id="08d56-191">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="08d56-191">The following is an example of the response.</span></span>

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

<span data-ttu-id="08d56-192">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="08d56-192">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Total Peer-to-peer Session Count,Total Organized Conference Count,Total Participated Conference Count,Peer-to-peer Last Activity Date,Organized Conference Last Activity Date,Participated Conference Last Activity Date,Peer-to-peer IM Count,Peer-to-peer Audio Count,Peer-to-peer Audio Minutes,Peer-to-peer Video Count,Peer-to-peer Video Minutes,Peer-to-peer App Sharing Count,Peer-to-peer File Transfer Count,Organized Conference IM Count,Organized Conference Audio/Video Count,Organized Conference Audio/Video Minutes,Organized Conference App Sharing Count,Organized Conference Web Count,Organized Conference Dial-in/out 3rd Party Count,Organized Conference Dial-in/out Microsoft Count,Organized Conference Dial-in Microsoft Minutes,Organized Conference Dial-out Microsoft Minutes,Paricipated Conference IM Count,Participated Conference Audio/Video Count,Participated Conference Audio/Video Minutes,Participated Conference App Sharing Count,Participated Conference Web Count,Participated Conference Dial-in/out 3rd Party Count,Assigned Products,Report Period
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
