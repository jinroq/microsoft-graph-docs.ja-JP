---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserDetail'
description: ユーザー別の Skype for Business デバイス使用状況に関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 78ee4819bbddcf0619a9f378ff12507bc69534f6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919415"
---
# <a name="reportroot-getskypeforbusinessdeviceusageuserdetail"></a><span data-ttu-id="a7a39-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="a7a39-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span></span>

<span data-ttu-id="a7a39-104">ユーザー別の Skype for Business デバイス使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="a7a39-104">Get details about Skype for Business device usage by user.</span></span>

> <span data-ttu-id="a7a39-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: 使用している Skype for Business クライアント](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a7a39-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="a7a39-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a7a39-106">Permissions</span></span>

<span data-ttu-id="a7a39-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a7a39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a7a39-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a7a39-109">Permission type</span></span>                        | <span data-ttu-id="a7a39-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a7a39-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a7a39-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="a7a39-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a7a39-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7a39-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a7a39-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a7a39-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7a39-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7a39-114">Not supported.</span></span>                           |
| <span data-ttu-id="a7a39-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a7a39-115">Application</span></span>                            | <span data-ttu-id="a7a39-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7a39-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a7a39-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a7a39-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="a7a39-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="a7a39-118">Function parameters</span></span>

<span data-ttu-id="a7a39-119">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="a7a39-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="a7a39-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="a7a39-120">Parameter</span></span> | <span data-ttu-id="a7a39-121">型</span><span class="sxs-lookup"><span data-stu-id="a7a39-121">Type</span></span>   | <span data-ttu-id="a7a39-122">説明</span><span class="sxs-lookup"><span data-stu-id="a7a39-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a7a39-123">period</span><span class="sxs-lookup"><span data-stu-id="a7a39-123">period</span></span>    | <span data-ttu-id="a7a39-124">文字列</span><span class="sxs-lookup"><span data-stu-id="a7a39-124">string</span></span> | <span data-ttu-id="a7a39-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="a7a39-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a7a39-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="a7a39-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a7a39-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="a7a39-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="a7a39-128">date</span><span class="sxs-lookup"><span data-stu-id="a7a39-128">date</span></span>      | <span data-ttu-id="a7a39-129">日付</span><span class="sxs-lookup"><span data-stu-id="a7a39-129">Date</span></span>   | <span data-ttu-id="a7a39-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="a7a39-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="a7a39-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="a7a39-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="a7a39-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="a7a39-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="a7a39-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a7a39-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a7a39-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a7a39-134">Request headers</span></span>

| <span data-ttu-id="a7a39-135">名前</span><span class="sxs-lookup"><span data-stu-id="a7a39-135">Name</span></span>          | <span data-ttu-id="a7a39-136">説明</span><span class="sxs-lookup"><span data-stu-id="a7a39-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="a7a39-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7a39-137">Authorization</span></span> | <span data-ttu-id="a7a39-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a7a39-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="a7a39-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="a7a39-140">If-None-Match</span></span> | <span data-ttu-id="a7a39-141">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="a7a39-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="a7a39-142">省略可能。</span><span class="sxs-lookup"><span data-stu-id="a7a39-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="a7a39-143">応答</span><span class="sxs-lookup"><span data-stu-id="a7a39-143">Response</span></span>

<span data-ttu-id="a7a39-144">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="a7a39-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a7a39-145">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="a7a39-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a7a39-146">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="a7a39-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a7a39-147">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="a7a39-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a7a39-148">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="a7a39-148">Report Refresh Date</span></span>
- <span data-ttu-id="a7a39-149">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="a7a39-149">User Principal Name</span></span>
- <span data-ttu-id="a7a39-150">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="a7a39-150">Last Activity Date</span></span>
- <span data-ttu-id="a7a39-151">Windows の使用</span><span class="sxs-lookup"><span data-stu-id="a7a39-151">Used Windows</span></span>
- <span data-ttu-id="a7a39-152">Windows スマートフォンの使用</span><span class="sxs-lookup"><span data-stu-id="a7a39-152">Used Windows Phone</span></span>
- <span data-ttu-id="a7a39-153">Android スマートフォンの使用</span><span class="sxs-lookup"><span data-stu-id="a7a39-153">Used Android Phone</span></span>
- <span data-ttu-id="a7a39-154">iPhone の使用</span><span class="sxs-lookup"><span data-stu-id="a7a39-154">Used iPhone</span></span>
- <span data-ttu-id="a7a39-155">IPad の使用</span><span class="sxs-lookup"><span data-stu-id="a7a39-155">Used iPad</span></span>
- <span data-ttu-id="a7a39-156">レポート期間</span><span class="sxs-lookup"><span data-stu-id="a7a39-156">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="a7a39-157">例</span><span class="sxs-lookup"><span data-stu-id="a7a39-157">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a7a39-158">要求</span><span class="sxs-lookup"><span data-stu-id="a7a39-158">Request</span></span>

<span data-ttu-id="a7a39-159">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a7a39-159">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="a7a39-160">応答</span><span class="sxs-lookup"><span data-stu-id="a7a39-160">Response</span></span>

<span data-ttu-id="a7a39-161">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a7a39-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="a7a39-162">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="a7a39-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Used Windows,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Report Period
```
