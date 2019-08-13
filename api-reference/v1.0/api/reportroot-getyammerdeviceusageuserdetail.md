---
title: 'reportRoot: getYammerDeviceUsageUserDetail function'
description: ユーザー別の Yammer デバイス使用状況に関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 0111cb3510187801fd2dea5905a91ee3225cf616
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320270"
---
# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="74dc3-103">reportRoot: getYammerDeviceUsageUserDetail function</span><span class="sxs-lookup"><span data-stu-id="74dc3-103">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

<span data-ttu-id="74dc3-104">ユーザー別の Yammer デバイス使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="74dc3-104">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="74dc3-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer デバイスの使用状況](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="74dc3-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="74dc3-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="74dc3-106">Permissions</span></span>

<span data-ttu-id="74dc3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="74dc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="74dc3-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="74dc3-109">Permission type</span></span>                        | <span data-ttu-id="74dc3-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="74dc3-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="74dc3-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="74dc3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="74dc3-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="74dc3-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="74dc3-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="74dc3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74dc3-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74dc3-114">Not supported.</span></span>                           |
| <span data-ttu-id="74dc3-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="74dc3-115">Application</span></span>                            | <span data-ttu-id="74dc3-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="74dc3-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="74dc3-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="74dc3-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="74dc3-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="74dc3-118">Function parameters</span></span>

<span data-ttu-id="74dc3-119">要求 URL に、クエリ パラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="74dc3-119">In the request URL, provide the query parameter with a valid value.</span></span>

| <span data-ttu-id="74dc3-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="74dc3-120">Parameter</span></span> | <span data-ttu-id="74dc3-121">型</span><span class="sxs-lookup"><span data-stu-id="74dc3-121">Type</span></span>   | <span data-ttu-id="74dc3-122">説明</span><span class="sxs-lookup"><span data-stu-id="74dc3-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="74dc3-123">period</span><span class="sxs-lookup"><span data-stu-id="74dc3-123">period</span></span>    | <span data-ttu-id="74dc3-124">文字列</span><span class="sxs-lookup"><span data-stu-id="74dc3-124">string</span></span> | <span data-ttu-id="74dc3-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="74dc3-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="74dc3-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="74dc3-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="74dc3-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="74dc3-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="74dc3-128">date</span><span class="sxs-lookup"><span data-stu-id="74dc3-128">date</span></span>      | <span data-ttu-id="74dc3-129">日付</span><span class="sxs-lookup"><span data-stu-id="74dc3-129">Date</span></span>   | <span data-ttu-id="74dc3-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="74dc3-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="74dc3-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="74dc3-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="74dc3-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="74dc3-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="74dc3-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="74dc3-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="74dc3-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="74dc3-134">Request headers</span></span>

| <span data-ttu-id="74dc3-135">名前</span><span class="sxs-lookup"><span data-stu-id="74dc3-135">Name</span></span>          | <span data-ttu-id="74dc3-136">説明</span><span class="sxs-lookup"><span data-stu-id="74dc3-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="74dc3-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="74dc3-137">Authorization</span></span> | <span data-ttu-id="74dc3-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="74dc3-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="74dc3-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="74dc3-140">If-None-Match</span></span> | <span data-ttu-id="74dc3-141">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="74dc3-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="74dc3-142">省略可能。</span><span class="sxs-lookup"><span data-stu-id="74dc3-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="74dc3-143">応答</span><span class="sxs-lookup"><span data-stu-id="74dc3-143">Response</span></span>

<span data-ttu-id="74dc3-144">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="74dc3-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="74dc3-145">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="74dc3-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="74dc3-146">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="74dc3-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="74dc3-147">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="74dc3-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="74dc3-148">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="74dc3-148">Report Refresh Date</span></span>
- <span data-ttu-id="74dc3-149">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="74dc3-149">User Principal Name</span></span>
- <span data-ttu-id="74dc3-150">表示名</span><span class="sxs-lookup"><span data-stu-id="74dc3-150">Display Name</span></span>
- <span data-ttu-id="74dc3-151">ユーザーの状態</span><span class="sxs-lookup"><span data-stu-id="74dc3-151">User State</span></span>
- <span data-ttu-id="74dc3-152">状態変更日付</span><span class="sxs-lookup"><span data-stu-id="74dc3-152">State Change Date</span></span>
- <span data-ttu-id="74dc3-153">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="74dc3-153">Last Activity Date</span></span>
- <span data-ttu-id="74dc3-154">Web の使用</span><span class="sxs-lookup"><span data-stu-id="74dc3-154">Used Web</span></span>
- <span data-ttu-id="74dc3-155">Windows スマートフォンの使用</span><span class="sxs-lookup"><span data-stu-id="74dc3-155">Used Windows Phone</span></span>
- <span data-ttu-id="74dc3-156">Android スマートフォンの使用</span><span class="sxs-lookup"><span data-stu-id="74dc3-156">Used Android Phone</span></span>
- <span data-ttu-id="74dc3-157">iPhone の使用</span><span class="sxs-lookup"><span data-stu-id="74dc3-157">Used iPhone</span></span>
- <span data-ttu-id="74dc3-158">IPad の使用</span><span class="sxs-lookup"><span data-stu-id="74dc3-158">Used iPad</span></span>
- <span data-ttu-id="74dc3-159">その他の使用</span><span class="sxs-lookup"><span data-stu-id="74dc3-159">Used Others</span></span>
- <span data-ttu-id="74dc3-160">レポート期間</span><span class="sxs-lookup"><span data-stu-id="74dc3-160">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="74dc3-161">例</span><span class="sxs-lookup"><span data-stu-id="74dc3-161">Example</span></span>

#### <a name="request"></a><span data-ttu-id="74dc3-162">要求</span><span class="sxs-lookup"><span data-stu-id="74dc3-162">Request</span></span>

<span data-ttu-id="74dc3-163">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="74dc3-163">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="74dc3-164">プロトコル</span><span class="sxs-lookup"><span data-stu-id="74dc3-164">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="74dc3-165">C#</span><span class="sxs-lookup"><span data-stu-id="74dc3-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammerdeviceusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="74dc3-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74dc3-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammerdeviceusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="74dc3-167">目的-C</span><span class="sxs-lookup"><span data-stu-id="74dc3-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammerdeviceusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="74dc3-168">Java</span><span class="sxs-lookup"><span data-stu-id="74dc3-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammerdeviceusageuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="74dc3-169">応答</span><span class="sxs-lookup"><span data-stu-id="74dc3-169">Response</span></span>

<span data-ttu-id="74dc3-170">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="74dc3-170">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="74dc3-171">要求</span><span class="sxs-lookup"><span data-stu-id="74dc3-171">Request</span></span>

<span data-ttu-id="74dc3-172">`date`パラメーターを指定して呼び出された場合、レポートのスコープは、指定された日付の使用に設定されます。</span><span class="sxs-lookup"><span data-stu-id="74dc3-172">If called with the `date` parameter, the report is scoped to usage on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="74dc3-173">応答</span><span class="sxs-lookup"><span data-stu-id="74dc3-173">Response</span></span>

<span data-ttu-id="74dc3-174">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="74dc3-174">The following is an example of the response.</span></span>

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

<span data-ttu-id="74dc3-175">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="74dc3-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Used Web,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Used Others,Report Period
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
