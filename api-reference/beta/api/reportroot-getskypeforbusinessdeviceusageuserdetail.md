---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserDetail'
description: ユーザー別の Skype for Business デバイス使用状況に関する詳細を取得します。
ms.openlocfilehash: fc3e5387c6842d86ace676fea64366d913bfdd73
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067490"
---
# <a name="reportroot-getskypeforbusinessdeviceusageuserdetail"></a><span data-ttu-id="1de0c-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="1de0c-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span></span>

> <span data-ttu-id="1de0c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1de0c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1de0c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1de0c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1de0c-106">ユーザー別の Skype for Business デバイス使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="1de0c-106">Get details about Skype for Business device usage by user.</span></span>

> <span data-ttu-id="1de0c-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: 使用している Skype for Business クライアント](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1de0c-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="1de0c-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1de0c-108">Permissions</span></span>

<span data-ttu-id="1de0c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1de0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1de0c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1de0c-111">Permission type</span></span>                        | <span data-ttu-id="1de0c-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1de0c-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1de0c-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="1de0c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1de0c-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1de0c-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1de0c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1de0c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1de0c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1de0c-116">Not supported.</span></span>                           |
| <span data-ttu-id="1de0c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1de0c-117">Application</span></span>                            | <span data-ttu-id="1de0c-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1de0c-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1de0c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1de0c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="1de0c-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="1de0c-120">Function parameters</span></span>

<span data-ttu-id="1de0c-121">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="1de0c-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="1de0c-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="1de0c-122">Parameter</span></span> | <span data-ttu-id="1de0c-123">型</span><span class="sxs-lookup"><span data-stu-id="1de0c-123">Type</span></span>   | <span data-ttu-id="1de0c-124">説明</span><span class="sxs-lookup"><span data-stu-id="1de0c-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1de0c-125">period</span><span class="sxs-lookup"><span data-stu-id="1de0c-125">period</span></span>    | <span data-ttu-id="1de0c-126">文字列</span><span class="sxs-lookup"><span data-stu-id="1de0c-126">string</span></span> | <span data-ttu-id="1de0c-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="1de0c-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1de0c-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="1de0c-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1de0c-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="1de0c-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="1de0c-130">date</span><span class="sxs-lookup"><span data-stu-id="1de0c-130">date</span></span>      | <span data-ttu-id="1de0c-131">日付</span><span class="sxs-lookup"><span data-stu-id="1de0c-131">Date</span></span>   | <span data-ttu-id="1de0c-132">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="1de0c-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="1de0c-133">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="1de0c-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="1de0c-134">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="1de0c-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="1de0c-135">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1de0c-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="1de0c-136">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1de0c-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="1de0c-137">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="1de0c-137">The default output type is text/csv.</span></span> <span data-ttu-id="1de0c-138">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="1de0c-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1de0c-139">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1de0c-139">Request headers</span></span>

| <span data-ttu-id="1de0c-140">名前</span><span class="sxs-lookup"><span data-stu-id="1de0c-140">Name</span></span>          | <span data-ttu-id="1de0c-141">説明</span><span class="sxs-lookup"><span data-stu-id="1de0c-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1de0c-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="1de0c-142">Authorization</span></span> | <span data-ttu-id="1de0c-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1de0c-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1de0c-145">応答</span><span class="sxs-lookup"><span data-stu-id="1de0c-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="1de0c-146">CSV</span><span class="sxs-lookup"><span data-stu-id="1de0c-146">CSV</span></span>

<span data-ttu-id="1de0c-147">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="1de0c-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1de0c-148">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="1de0c-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1de0c-149">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="1de0c-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1de0c-150">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="1de0c-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1de0c-151">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="1de0c-151">Report Refresh Date</span></span>
- <span data-ttu-id="1de0c-152">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="1de0c-152">User Principal Name</span></span>
- <span data-ttu-id="1de0c-153">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="1de0c-153">Last Activity Date</span></span>
- <span data-ttu-id="1de0c-154">Windows の使用</span><span class="sxs-lookup"><span data-stu-id="1de0c-154">Used Windows</span></span>
- <span data-ttu-id="1de0c-155">Windows スマートフォンの使用</span><span class="sxs-lookup"><span data-stu-id="1de0c-155">Used Windows Phone</span></span>
- <span data-ttu-id="1de0c-156">Android スマートフォンの使用</span><span class="sxs-lookup"><span data-stu-id="1de0c-156">Used Android Phone</span></span>
- <span data-ttu-id="1de0c-157">iPhone の使用</span><span class="sxs-lookup"><span data-stu-id="1de0c-157">Used iPhone</span></span>
- <span data-ttu-id="1de0c-158">IPad の使用</span><span class="sxs-lookup"><span data-stu-id="1de0c-158">Used iPad</span></span>
- <span data-ttu-id="1de0c-159">レポート期間</span><span class="sxs-lookup"><span data-stu-id="1de0c-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="1de0c-160">JSON</span><span class="sxs-lookup"><span data-stu-id="1de0c-160">JSON</span></span>

<span data-ttu-id="1de0c-161">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[skypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="1de0c-161">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="1de0c-162">この要求の既定のページ サイズは、アイテムは 200 個です。</span><span class="sxs-lookup"><span data-stu-id="1de0c-162">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="1de0c-163">使用例</span><span class="sxs-lookup"><span data-stu-id="1de0c-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="1de0c-164">CSV</span><span class="sxs-lookup"><span data-stu-id="1de0c-164">CSV</span></span>

<span data-ttu-id="1de0c-165">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="1de0c-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="1de0c-166">要求</span><span class="sxs-lookup"><span data-stu-id="1de0c-166">Request</span></span>

<span data-ttu-id="1de0c-167">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1de0c-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="1de0c-168">応答</span><span class="sxs-lookup"><span data-stu-id="1de0c-168">Response</span></span>

<span data-ttu-id="1de0c-169">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1de0c-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="1de0c-170">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="1de0c-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Used Windows,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Report Period
```

### <a name="json"></a><span data-ttu-id="1de0c-171">JSON</span><span class="sxs-lookup"><span data-stu-id="1de0c-171">JSON</span></span>

<span data-ttu-id="1de0c-172">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="1de0c-172">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="1de0c-173">要求</span><span class="sxs-lookup"><span data-stu-id="1de0c-173">Request</span></span>

<span data-ttu-id="1de0c-174">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1de0c-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="1de0c-175">応答</span><span class="sxs-lookup"><span data-stu-id="1de0c-175">Response</span></span>

<span data-ttu-id="1de0c-176">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1de0c-176">The following is an example of the response.</span></span>

> <span data-ttu-id="1de0c-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1de0c-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 356

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessDeviceUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "lastActivityDate": "2017-09-01", 
      "usedWindows": true, 
      "usedWindowsPhone": false, 
      "usedAndroidPhone": false, 
      "usediPhone": false, 
      "usediPad": false, 
      "reportPeriod": "7"
    }
  ]
}
```