---
title: 'reportRoot: getYammerDeviceUsageUserDetail function'
description: ユーザー別の Yammer デバイス使用状況に関する詳細を取得します。
ms.openlocfilehash: c112ba0948adb07dbb5264ab73f6458f2ef97b09
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022371"
---
# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="1e4d5-103">reportRoot: getYammerDeviceUsageUserDetail function</span><span class="sxs-lookup"><span data-stu-id="1e4d5-103">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

<span data-ttu-id="1e4d5-104">ユーザー別の Yammer デバイス使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="1e4d5-104">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="1e4d5-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer デバイスの使用状況](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e4d5-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="1e4d5-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1e4d5-106">Permissions</span></span>

<span data-ttu-id="1e4d5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e4d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1e4d5-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1e4d5-109">Permission type</span></span>                        | <span data-ttu-id="1e4d5-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1e4d5-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1e4d5-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="1e4d5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1e4d5-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e4d5-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1e4d5-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1e4d5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e4d5-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e4d5-114">Not supported.</span></span>                           |
| <span data-ttu-id="1e4d5-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1e4d5-115">Application</span></span>                            | <span data-ttu-id="1e4d5-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e4d5-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1e4d5-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1e4d5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="1e4d5-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="1e4d5-118">Function parameters</span></span>

<span data-ttu-id="1e4d5-119">要求 URL に、クエリ パラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="1e4d5-119">In the request URL, provide the query parameter with a valid value.</span></span>

| <span data-ttu-id="1e4d5-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="1e4d5-120">Parameter</span></span> | <span data-ttu-id="1e4d5-121">型</span><span class="sxs-lookup"><span data-stu-id="1e4d5-121">Type</span></span>   | <span data-ttu-id="1e4d5-122">説明</span><span class="sxs-lookup"><span data-stu-id="1e4d5-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1e4d5-123">period</span><span class="sxs-lookup"><span data-stu-id="1e4d5-123">period</span></span>    | <span data-ttu-id="1e4d5-124">文字列</span><span class="sxs-lookup"><span data-stu-id="1e4d5-124">string</span></span> | <span data-ttu-id="1e4d5-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="1e4d5-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1e4d5-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="1e4d5-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1e4d5-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="1e4d5-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="1e4d5-128">date</span><span class="sxs-lookup"><span data-stu-id="1e4d5-128">date</span></span>      | <span data-ttu-id="1e4d5-129">日付</span><span class="sxs-lookup"><span data-stu-id="1e4d5-129">Date</span></span>   | <span data-ttu-id="1e4d5-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="1e4d5-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="1e4d5-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="1e4d5-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="1e4d5-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="1e4d5-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="1e4d5-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1e4d5-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1e4d5-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e4d5-134">Request headers</span></span>

| <span data-ttu-id="1e4d5-135">名前</span><span class="sxs-lookup"><span data-stu-id="1e4d5-135">Name</span></span>          | <span data-ttu-id="1e4d5-136">説明</span><span class="sxs-lookup"><span data-stu-id="1e4d5-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="1e4d5-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e4d5-137">Authorization</span></span> | <span data-ttu-id="1e4d5-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1e4d5-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="1e4d5-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="1e4d5-140">If-None-Match</span></span> | <span data-ttu-id="1e4d5-141">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="1e4d5-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="1e4d5-142">省略可能。</span><span class="sxs-lookup"><span data-stu-id="1e4d5-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="1e4d5-143">応答</span><span class="sxs-lookup"><span data-stu-id="1e4d5-143">Response</span></span>

<span data-ttu-id="1e4d5-144">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="1e4d5-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1e4d5-145">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="1e4d5-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1e4d5-146">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="1e4d5-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1e4d5-147">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="1e4d5-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1e4d5-148">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="1e4d5-148">Report Refresh Date</span></span>
- <span data-ttu-id="1e4d5-149">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="1e4d5-149">User Principal Name</span></span>
- <span data-ttu-id="1e4d5-150">表示名</span><span class="sxs-lookup"><span data-stu-id="1e4d5-150">Display Name</span></span>
- <span data-ttu-id="1e4d5-151">ユーザーの状態</span><span class="sxs-lookup"><span data-stu-id="1e4d5-151">User State</span></span>
- <span data-ttu-id="1e4d5-152">状態変更日付</span><span class="sxs-lookup"><span data-stu-id="1e4d5-152">State Change Date</span></span>
- <span data-ttu-id="1e4d5-153">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="1e4d5-153">Last Activity Date</span></span>
- <span data-ttu-id="1e4d5-154">Web の使用</span><span class="sxs-lookup"><span data-stu-id="1e4d5-154">Used Web</span></span>
- <span data-ttu-id="1e4d5-155">Windows スマートフォンの使用</span><span class="sxs-lookup"><span data-stu-id="1e4d5-155">Used Windows Phone</span></span>
- <span data-ttu-id="1e4d5-156">Android スマートフォンの使用</span><span class="sxs-lookup"><span data-stu-id="1e4d5-156">Used Android Phone</span></span>
- <span data-ttu-id="1e4d5-157">iPhone の使用</span><span class="sxs-lookup"><span data-stu-id="1e4d5-157">Used iPhone</span></span>
- <span data-ttu-id="1e4d5-158">IPad の使用</span><span class="sxs-lookup"><span data-stu-id="1e4d5-158">Used iPad</span></span>
- <span data-ttu-id="1e4d5-159">その他の使用</span><span class="sxs-lookup"><span data-stu-id="1e4d5-159">Used Others</span></span>
- <span data-ttu-id="1e4d5-160">レポート期間</span><span class="sxs-lookup"><span data-stu-id="1e4d5-160">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="1e4d5-161">例</span><span class="sxs-lookup"><span data-stu-id="1e4d5-161">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1e4d5-162">要求</span><span class="sxs-lookup"><span data-stu-id="1e4d5-162">Request</span></span>

<span data-ttu-id="1e4d5-163">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1e4d5-163">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="1e4d5-164">応答</span><span class="sxs-lookup"><span data-stu-id="1e4d5-164">Response</span></span>

<span data-ttu-id="1e4d5-165">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1e4d5-165">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="1e4d5-166">要求</span><span class="sxs-lookup"><span data-stu-id="1e4d5-166">Request</span></span>

<span data-ttu-id="1e4d5-167">呼び出した場合、`date`パラメーター、レポートの使用方法にスコープは、特定の日にします。</span><span class="sxs-lookup"><span data-stu-id="1e4d5-167">If called with the `date` parameter, the report is scoped to usage on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="1e4d5-168">応答</span><span class="sxs-lookup"><span data-stu-id="1e4d5-168">Response</span></span>

<span data-ttu-id="1e4d5-169">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1e4d5-169">The following is an example of the response.</span></span>

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

<span data-ttu-id="1e4d5-170">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="1e4d5-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Used Web,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Used Others,Report Period
```