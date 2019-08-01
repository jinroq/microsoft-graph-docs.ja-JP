---
title: 'reportRoot: getSkypeForBusinessActivityUserDetail'
description: ユーザー別の Skype for Business アクティビティに関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: ade165db5242e6cb3962f025ccdab8854c5edb6d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021754"
---
# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="a6fe6-103">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="a6fe6-103">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

<span data-ttu-id="a6fe6-104">ユーザー別の Skype for Business アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="a6fe6-104">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="a6fe6-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business アクティビティ](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6fe6-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="a6fe6-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a6fe6-106">Permissions</span></span>

<span data-ttu-id="a6fe6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6fe6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a6fe6-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a6fe6-109">Permission type</span></span>                        | <span data-ttu-id="a6fe6-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a6fe6-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a6fe6-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="a6fe6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a6fe6-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6fe6-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a6fe6-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a6fe6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6fe6-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6fe6-114">Not supported.</span></span>                           |
| <span data-ttu-id="a6fe6-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a6fe6-115">Application</span></span>                            | <span data-ttu-id="a6fe6-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6fe6-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a6fe6-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a6fe6-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a6fe6-118">プロトコル</span><span class="sxs-lookup"><span data-stu-id="a6fe6-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="a6fe6-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="a6fe6-119">Function parameters</span></span>

<span data-ttu-id="a6fe6-120">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="a6fe6-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="a6fe6-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="a6fe6-121">Parameter</span></span> | <span data-ttu-id="a6fe6-122">型</span><span class="sxs-lookup"><span data-stu-id="a6fe6-122">Type</span></span>   | <span data-ttu-id="a6fe6-123">説明</span><span class="sxs-lookup"><span data-stu-id="a6fe6-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a6fe6-124">period</span><span class="sxs-lookup"><span data-stu-id="a6fe6-124">period</span></span>    | <span data-ttu-id="a6fe6-125">文字列</span><span class="sxs-lookup"><span data-stu-id="a6fe6-125">string</span></span> | <span data-ttu-id="a6fe6-126">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="a6fe6-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a6fe6-127">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="a6fe6-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a6fe6-128">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="a6fe6-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="a6fe6-129">date</span><span class="sxs-lookup"><span data-stu-id="a6fe6-129">date</span></span>      | <span data-ttu-id="a6fe6-130">日付</span><span class="sxs-lookup"><span data-stu-id="a6fe6-130">Date</span></span>   | <span data-ttu-id="a6fe6-131">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="a6fe6-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="a6fe6-132">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="a6fe6-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="a6fe6-133">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="a6fe6-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="a6fe6-134">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a6fe6-134">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6fe6-135">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a6fe6-135">Request headers</span></span>

| <span data-ttu-id="a6fe6-136">名前</span><span class="sxs-lookup"><span data-stu-id="a6fe6-136">Name</span></span>          | <span data-ttu-id="a6fe6-137">説明</span><span class="sxs-lookup"><span data-stu-id="a6fe6-137">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="a6fe6-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6fe6-138">Authorization</span></span> | <span data-ttu-id="a6fe6-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a6fe6-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="a6fe6-141">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="a6fe6-141">If-None-Match</span></span> | <span data-ttu-id="a6fe6-142">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="a6fe6-142">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="a6fe6-143">省略可能。</span><span class="sxs-lookup"><span data-stu-id="a6fe6-143">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="a6fe6-144">応答</span><span class="sxs-lookup"><span data-stu-id="a6fe6-144">Response</span></span>

<span data-ttu-id="a6fe6-145">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="a6fe6-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a6fe6-146">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="a6fe6-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a6fe6-147">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="a6fe6-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a6fe6-148">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="a6fe6-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a6fe6-149">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="a6fe6-149">Report Refresh Date</span></span>
- <span data-ttu-id="a6fe6-150">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="a6fe6-150">User Principal Name</span></span>
- <span data-ttu-id="a6fe6-151">削除済み</span><span class="sxs-lookup"><span data-stu-id="a6fe6-151">Is Deleted</span></span>
- <span data-ttu-id="a6fe6-152">削除日</span><span class="sxs-lookup"><span data-stu-id="a6fe6-152">Deleted Date</span></span>
- <span data-ttu-id="a6fe6-153">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="a6fe6-153">Last Activity Date</span></span>
- <span data-ttu-id="a6fe6-154">ピア ツー ピア セッションの合計数</span><span class="sxs-lookup"><span data-stu-id="a6fe6-154">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="a6fe6-155">開催した会議の合計数</span><span class="sxs-lookup"><span data-stu-id="a6fe6-155">Total Organized Conference Count</span></span>
- <span data-ttu-id="a6fe6-156">参加した会議の合計数</span><span class="sxs-lookup"><span data-stu-id="a6fe6-156">Total Participated Conference Count</span></span>
- <span data-ttu-id="a6fe6-157">ピア ツー ピアの最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="a6fe6-157">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="a6fe6-158">開催した会議の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="a6fe6-158">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="a6fe6-159">参加した会議の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="a6fe6-159">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="a6fe6-160">ピア ツー ピアの IM の数</span><span class="sxs-lookup"><span data-stu-id="a6fe6-160">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="a6fe6-161">ピア ツー ピアのオーディオの数</span><span class="sxs-lookup"><span data-stu-id="a6fe6-161">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="a6fe6-162">ピア ツー ピアのオーディオの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="a6fe6-162">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="a6fe6-163">ピア ツー ピアのビデオの数</span><span class="sxs-lookup"><span data-stu-id="a6fe6-163">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="a6fe6-164">ピア ツー ピアのビデオの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="a6fe6-164">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="a6fe6-165">ピア ツー ピアのアプリ共有の数</span><span class="sxs-lookup"><span data-stu-id="a6fe6-165">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="a6fe6-166">ピア ツー ピアのファイル転送の数</span><span class="sxs-lookup"><span data-stu-id="a6fe6-166">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="a6fe6-167">開催した会議の IM の数</span><span class="sxs-lookup"><span data-stu-id="a6fe6-167">Organized Conference IM Count</span></span>
- <span data-ttu-id="a6fe6-168">開催した会議のオーディオ/ビデオの数</span><span class="sxs-lookup"><span data-stu-id="a6fe6-168">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="a6fe6-169">開催した会議のオーディオ/ビデオの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="a6fe6-169">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="a6fe6-170">開催した会議のアプリ共有の数</span><span class="sxs-lookup"><span data-stu-id="a6fe6-170">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="a6fe6-171">開催した会議の Web の数</span><span class="sxs-lookup"><span data-stu-id="a6fe6-171">Organized Conference Web Count</span></span>
- <span data-ttu-id="a6fe6-172">開催した会議のサード パーティのダイヤルイン/アウトの数</span><span class="sxs-lookup"><span data-stu-id="a6fe6-172">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="a6fe6-173">開催した会議の Microsoft のダイヤルイン/アウトの数</span><span class="sxs-lookup"><span data-stu-id="a6fe6-173">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="a6fe6-174">開催した会議の Microsoft のダイヤルインの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="a6fe6-174">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="a6fe6-175">開催した会議の Microsoft からのダイヤルアウトの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="a6fe6-175">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="a6fe6-176">参加した会議の IM の数</span><span class="sxs-lookup"><span data-stu-id="a6fe6-176">Paricipated Conference IM Count</span></span>
- <span data-ttu-id="a6fe6-177">参加した会議のオーディオ/ビデオの数</span><span class="sxs-lookup"><span data-stu-id="a6fe6-177">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="a6fe6-178">参加した会議のオーディオ/ビデオの時間 (分)</span><span class="sxs-lookup"><span data-stu-id="a6fe6-178">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="a6fe6-179">参加した会議のアプリ共有の数</span><span class="sxs-lookup"><span data-stu-id="a6fe6-179">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="a6fe6-180">参加した会議の Web の数</span><span class="sxs-lookup"><span data-stu-id="a6fe6-180">Participated Conference Web Count</span></span>
- <span data-ttu-id="a6fe6-181">参加した会議のサード パーティのダイヤルイン/アウトの数</span><span class="sxs-lookup"><span data-stu-id="a6fe6-181">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="a6fe6-182">割り当て済み製品</span><span class="sxs-lookup"><span data-stu-id="a6fe6-182">Assigned Products</span></span>
- <span data-ttu-id="a6fe6-183">レポート期間</span><span class="sxs-lookup"><span data-stu-id="a6fe6-183">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="a6fe6-184">例</span><span class="sxs-lookup"><span data-stu-id="a6fe6-184">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a6fe6-185">要求</span><span class="sxs-lookup"><span data-stu-id="a6fe6-185">Request</span></span>

<span data-ttu-id="a6fe6-186">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a6fe6-186">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessActivityUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a6fe6-187">C#</span><span class="sxs-lookup"><span data-stu-id="a6fe6-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessactivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a6fe6-188">Javascript</span><span class="sxs-lookup"><span data-stu-id="a6fe6-188">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessactivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a6fe6-189">目的-C</span><span class="sxs-lookup"><span data-stu-id="a6fe6-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessactivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a6fe6-190">Java</span><span class="sxs-lookup"><span data-stu-id="a6fe6-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessactivityuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a6fe6-191">応答</span><span class="sxs-lookup"><span data-stu-id="a6fe6-191">Response</span></span>

<span data-ttu-id="a6fe6-192">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a6fe6-192">The following is an example of the response.</span></span>

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

<span data-ttu-id="a6fe6-193">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="a6fe6-193">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
