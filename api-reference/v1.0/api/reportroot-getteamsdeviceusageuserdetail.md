---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: ユーザーごとに、Microsoft Teams デバイスの使用状況の詳細を取得します。
localization_priority: Normal
ms.openlocfilehash: 8e3f19d0e95c5b69109787208b4d75613922bd91
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840804"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="bab15-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="bab15-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

<span data-ttu-id="bab15-104">ユーザーごとに、Microsoft Teams デバイスの使用状況の詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="bab15-104">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="bab15-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bab15-105">Permissions</span></span>

<span data-ttu-id="bab15-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bab15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bab15-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bab15-108">Permission type</span></span>                        | <span data-ttu-id="bab15-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bab15-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="bab15-110">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="bab15-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bab15-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bab15-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="bab15-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bab15-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bab15-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bab15-113">Not supported.</span></span>                           |
| <span data-ttu-id="bab15-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bab15-114">Application</span></span>                            | <span data-ttu-id="bab15-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bab15-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bab15-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bab15-116">HTTP request</span></span>

<!-- { "blockType": "samples" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='{period_value}')
GET /reports/getTeamsDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="bab15-117">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="bab15-117">Function parameters</span></span>

<span data-ttu-id="bab15-118">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="bab15-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="bab15-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="bab15-119">Parameter</span></span> | <span data-ttu-id="bab15-120">Type</span><span class="sxs-lookup"><span data-stu-id="bab15-120">Type</span></span>   | <span data-ttu-id="bab15-121">説明</span><span class="sxs-lookup"><span data-stu-id="bab15-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="bab15-122">period</span><span class="sxs-lookup"><span data-stu-id="bab15-122">period</span></span>    | <span data-ttu-id="bab15-123">文字列</span><span class="sxs-lookup"><span data-stu-id="bab15-123">string</span></span> | <span data-ttu-id="bab15-124">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="bab15-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="bab15-125">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="bab15-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="bab15-126">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="bab15-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="bab15-127">date</span><span class="sxs-lookup"><span data-stu-id="bab15-127">date</span></span>      | <span data-ttu-id="bab15-128">日付</span><span class="sxs-lookup"><span data-stu-id="bab15-128">Date</span></span>   | <span data-ttu-id="bab15-129">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="bab15-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="bab15-130">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="bab15-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="bab15-131">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="bab15-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="bab15-132">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="bab15-132">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bab15-133">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bab15-133">Request headers</span></span>

| <span data-ttu-id="bab15-134">名前</span><span class="sxs-lookup"><span data-stu-id="bab15-134">Name</span></span>          | <span data-ttu-id="bab15-135">説明</span><span class="sxs-lookup"><span data-stu-id="bab15-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="bab15-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="bab15-136">Authorization</span></span> | <span data-ttu-id="bab15-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bab15-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="bab15-139">応答</span><span class="sxs-lookup"><span data-stu-id="bab15-139">Response</span></span>

<span data-ttu-id="bab15-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="bab15-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="bab15-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="bab15-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="bab15-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="bab15-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="bab15-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="bab15-143">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="bab15-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="bab15-144">Report Refresh Date</span></span>
- <span data-ttu-id="bab15-145">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="bab15-145">User Principal Name</span></span>
- <span data-ttu-id="bab15-146">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="bab15-146">Last Activity Date</span></span>
- <span data-ttu-id="bab15-147">削除済み</span><span class="sxs-lookup"><span data-stu-id="bab15-147">Is Deleted</span></span>
- <span data-ttu-id="bab15-148">削除日</span><span class="sxs-lookup"><span data-stu-id="bab15-148">Deleted Date</span></span>
- <span data-ttu-id="bab15-149">Web の使用</span><span class="sxs-lookup"><span data-stu-id="bab15-149">Used Web</span></span>
- <span data-ttu-id="bab15-150">Windows スマートフォンの使用</span><span class="sxs-lookup"><span data-stu-id="bab15-150">Used Windows Phone</span></span>
- <span data-ttu-id="bab15-151">iOS の使用</span><span class="sxs-lookup"><span data-stu-id="bab15-151">Used iOS</span></span>
- <span data-ttu-id="bab15-152">Mac の使用</span><span class="sxs-lookup"><span data-stu-id="bab15-152">Used Mac</span></span>
- <span data-ttu-id="bab15-153">Android スマートフォンの使用</span><span class="sxs-lookup"><span data-stu-id="bab15-153">Used Android Phone</span></span>
- <span data-ttu-id="bab15-154">Windows の使用</span><span class="sxs-lookup"><span data-stu-id="bab15-154">Used Windows</span></span>
- <span data-ttu-id="bab15-155">レポート期間</span><span class="sxs-lookup"><span data-stu-id="bab15-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="bab15-156">例</span><span class="sxs-lookup"><span data-stu-id="bab15-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="bab15-157">要求</span><span class="sxs-lookup"><span data-stu-id="bab15-157">Request</span></span>

<span data-ttu-id="bab15-158">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bab15-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="bab15-159">応答</span><span class="sxs-lookup"><span data-stu-id="bab15-159">Response</span></span>

<span data-ttu-id="bab15-160">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bab15-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="bab15-161">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="bab15-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Used Web,Used Windows Phone,Used iOS,Used Mac,Used Android Phone,Used Windows,Report Period
```
