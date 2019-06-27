---
title: 'reportRoot: getSkypeForBusinessActivityUserDetail'
description: ユーザー別の Skype for Business アクティビティに関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 6b80e72b903c73f4893a81369bec33d43c4cd275
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276252"
---
# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="bb3d3-103">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="bb3d3-103">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

<span data-ttu-id="bb3d3-104">ユーザー別の Skype for Business アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="bb3d3-104">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="bb3d3-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business アクティビティ](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb3d3-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="bb3d3-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bb3d3-106">Permissions</span></span>

<span data-ttu-id="bb3d3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb3d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bb3d3-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bb3d3-109">Permission type</span></span>                        | <span data-ttu-id="bb3d3-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bb3d3-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="bb3d3-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="bb3d3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bb3d3-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb3d3-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="bb3d3-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bb3d3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb3d3-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb3d3-114">Not supported.</span></span>                           |
| <span data-ttu-id="bb3d3-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bb3d3-115">Application</span></span>                            | <span data-ttu-id="bb3d3-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb3d3-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bb3d3-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bb3d3-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="bb3d3-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="bb3d3-118">Function parameters</span></span>

<span data-ttu-id="bb3d3-119">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="bb3d3-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="bb3d3-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="bb3d3-120">Parameter</span></span> | <span data-ttu-id="bb3d3-121">型</span><span class="sxs-lookup"><span data-stu-id="bb3d3-121">Type</span></span>   | <span data-ttu-id="bb3d3-122">説明</span><span class="sxs-lookup"><span data-stu-id="bb3d3-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="bb3d3-123">period</span><span class="sxs-lookup"><span data-stu-id="bb3d3-123">period</span></span>    | <span data-ttu-id="bb3d3-124">文字列</span><span class="sxs-lookup"><span data-stu-id="bb3d3-124">string</span></span> | <span data-ttu-id="bb3d3-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="bb3d3-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="bb3d3-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="bb3d3-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="bb3d3-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="bb3d3-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="bb3d3-128">date</span><span class="sxs-lookup"><span data-stu-id="bb3d3-128">date</span></span>      | <span data-ttu-id="bb3d3-129">日付</span><span class="sxs-lookup"><span data-stu-id="bb3d3-129">Date</span></span>   | <span data-ttu-id="bb3d3-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="bb3d3-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="bb3d3-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="bb3d3-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="bb3d3-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="bb3d3-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="bb3d3-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="bb3d3-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb3d3-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bb3d3-134">Request headers</span></span>

| <span data-ttu-id="bb3d3-135">名前</span><span class="sxs-lookup"><span data-stu-id="bb3d3-135">Name</span></span>          | <span data-ttu-id="bb3d3-136">説明</span><span class="sxs-lookup"><span data-stu-id="bb3d3-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="bb3d3-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb3d3-137">Authorization</span></span> | <span data-ttu-id="bb3d3-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bb3d3-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="bb3d3-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="bb3d3-140">If-None-Match</span></span> | <span data-ttu-id="bb3d3-141">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="bb3d3-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="bb3d3-142">省略可能。</span><span class="sxs-lookup"><span data-stu-id="bb3d3-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="bb3d3-143">応答</span><span class="sxs-lookup"><span data-stu-id="bb3d3-143">Response</span></span>

<span data-ttu-id="bb3d3-144">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="bb3d3-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="bb3d3-145">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="bb3d3-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="bb3d3-146">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="bb3d3-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="bb3d3-147">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="bb3d3-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="bb3d3-148">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="bb3d3-148">Report Refresh Date</span></span>
- <span data-ttu-id="bb3d3-149">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="bb3d3-149">User Principal Name</span></span>
- <span data-ttu-id="bb3d3-150">削除済み</span><span class="sxs-lookup"><span data-stu-id="bb3d3-150">Is Deleted</span></span>
- <span data-ttu-id="bb3d3-151">削除日</span><span class="sxs-lookup"><span data-stu-id="bb3d3-151">Deleted Date</span></span>
- <span data-ttu-id="bb3d3-152">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="bb3d3-152">Last Activity Date</span></span>
- <span data-ttu-id="bb3d3-153">ピア ツー ピア セッションの合計数</span><span class="sxs-lookup"><span data-stu-id="bb3d3-153">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="bb3d3-154">開催した会議の合計数</span><span class="sxs-lookup"><span data-stu-id="bb3d3-154">Total Organized Conference Count</span></span>
- <span data-ttu-id="bb3d3-155">参加した会議の合計数</span><span class="sxs-lookup"><span data-stu-id="bb3d3-155">Total Participated Conference Count</span></span>
- <span data-ttu-id="bb3d3-156">ピア ツー ピアの最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="bb3d3-156">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="bb3d3-157">開催した会議の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="bb3d3-157">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="bb3d3-158">参加した会議の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="bb3d3-158">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="bb3d3-159">ピア ツー ピアの IM の数</span><span class="sxs-lookup"><span data-stu-id="bb3d3-159">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="bb3d3-160">ピア ツー ピアのオーディオの数</span><span class="sxs-lookup"><span data-stu-id="bb3d3-160">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="bb3d3-161">ピア ツー ピアのオーディオの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="bb3d3-161">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="bb3d3-162">ピア ツー ピアのビデオの数</span><span class="sxs-lookup"><span data-stu-id="bb3d3-162">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="bb3d3-163">ピア ツー ピアのビデオの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="bb3d3-163">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="bb3d3-164">ピア ツー ピアのアプリ共有の数</span><span class="sxs-lookup"><span data-stu-id="bb3d3-164">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="bb3d3-165">ピア ツー ピアのファイル転送の数</span><span class="sxs-lookup"><span data-stu-id="bb3d3-165">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="bb3d3-166">開催した会議の IM の数</span><span class="sxs-lookup"><span data-stu-id="bb3d3-166">Organized Conference IM Count</span></span>
- <span data-ttu-id="bb3d3-167">開催した会議のオーディオ/ビデオの数</span><span class="sxs-lookup"><span data-stu-id="bb3d3-167">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="bb3d3-168">開催した会議のオーディオ/ビデオの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="bb3d3-168">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="bb3d3-169">開催した会議のアプリ共有の数</span><span class="sxs-lookup"><span data-stu-id="bb3d3-169">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="bb3d3-170">開催した会議の Web の数</span><span class="sxs-lookup"><span data-stu-id="bb3d3-170">Organized Conference Web Count</span></span>
- <span data-ttu-id="bb3d3-171">開催した会議のサード パーティのダイヤルイン/アウトの数</span><span class="sxs-lookup"><span data-stu-id="bb3d3-171">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="bb3d3-172">開催した会議の Microsoft のダイヤルイン/アウトの数</span><span class="sxs-lookup"><span data-stu-id="bb3d3-172">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="bb3d3-173">開催した会議の Microsoft のダイヤルインの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="bb3d3-173">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="bb3d3-174">開催した会議の Microsoft からのダイヤルアウトの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="bb3d3-174">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="bb3d3-175">参加した会議の IM の数</span><span class="sxs-lookup"><span data-stu-id="bb3d3-175">Paricipated Conference IM Count</span></span>
- <span data-ttu-id="bb3d3-176">参加した会議のオーディオ/ビデオの数</span><span class="sxs-lookup"><span data-stu-id="bb3d3-176">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="bb3d3-177">参加した会議のオーディオ/ビデオの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="bb3d3-177">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="bb3d3-178">参加した会議のアプリ共有の数</span><span class="sxs-lookup"><span data-stu-id="bb3d3-178">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="bb3d3-179">参加した会議の Web の数</span><span class="sxs-lookup"><span data-stu-id="bb3d3-179">Participated Conference Web Count</span></span>
- <span data-ttu-id="bb3d3-180">参加した会議のサード パーティのダイヤルイン/アウトの数</span><span class="sxs-lookup"><span data-stu-id="bb3d3-180">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="bb3d3-181">割り当て済み製品</span><span class="sxs-lookup"><span data-stu-id="bb3d3-181">Assigned Products</span></span>
- <span data-ttu-id="bb3d3-182">レポート期間</span><span class="sxs-lookup"><span data-stu-id="bb3d3-182">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="bb3d3-183">例</span><span class="sxs-lookup"><span data-stu-id="bb3d3-183">Example</span></span>

#### <a name="request"></a><span data-ttu-id="bb3d3-184">要求</span><span class="sxs-lookup"><span data-stu-id="bb3d3-184">Request</span></span>

<span data-ttu-id="bb3d3-185">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bb3d3-185">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="bb3d3-186">応答</span><span class="sxs-lookup"><span data-stu-id="bb3d3-186">Response</span></span>

<span data-ttu-id="bb3d3-187">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bb3d3-187">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="bb3d3-188">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="bb3d3-188">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bb3d3-189">C#</span><span class="sxs-lookup"><span data-stu-id="bb3d3-189">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessactivityuserdetail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bb3d3-190">Javascript</span><span class="sxs-lookup"><span data-stu-id="bb3d3-190">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessactivityuserdetail-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="bb3d3-191">目的-C</span><span class="sxs-lookup"><span data-stu-id="bb3d3-191">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessactivityuserdetail-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="bb3d3-192">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="bb3d3-192">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
    "Error: /api-reference/v1.0/api/reportroot-getskypeforbusinessactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getskypeforbusinessactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getskypeforbusinessactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
