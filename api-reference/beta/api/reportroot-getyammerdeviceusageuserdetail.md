---
title: 'reportRoot: getYammerDeviceUsageUserDetail function'
description: ユーザー別の Yammer デバイス使用状況に関する詳細を取得します。
ms.openlocfilehash: 21026bf1cd92e6924bf1758bd6284c43ab877841
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070412"
---
# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="22324-103">reportRoot: getYammerDeviceUsageUserDetail function</span><span class="sxs-lookup"><span data-stu-id="22324-103">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

> <span data-ttu-id="22324-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="22324-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22324-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22324-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="22324-106">ユーザー別の Yammer デバイス使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="22324-106">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="22324-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer デバイスの使用状況](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="22324-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="22324-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="22324-108">Permissions</span></span>

<span data-ttu-id="22324-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="22324-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="22324-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="22324-111">Permission type</span></span>                        | <span data-ttu-id="22324-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="22324-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="22324-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="22324-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="22324-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="22324-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="22324-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="22324-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22324-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22324-116">Not supported.</span></span>                           |
| <span data-ttu-id="22324-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="22324-117">Application</span></span>                            | <span data-ttu-id="22324-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="22324-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="22324-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="22324-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="22324-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="22324-120">Function parameters</span></span>

<span data-ttu-id="22324-121">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="22324-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="22324-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="22324-122">Parameter</span></span> | <span data-ttu-id="22324-123">型</span><span class="sxs-lookup"><span data-stu-id="22324-123">Type</span></span>   | <span data-ttu-id="22324-124">説明</span><span class="sxs-lookup"><span data-stu-id="22324-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="22324-125">period</span><span class="sxs-lookup"><span data-stu-id="22324-125">period</span></span>    | <span data-ttu-id="22324-126">文字列</span><span class="sxs-lookup"><span data-stu-id="22324-126">string</span></span> | <span data-ttu-id="22324-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="22324-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="22324-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="22324-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="22324-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="22324-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="22324-130">date</span><span class="sxs-lookup"><span data-stu-id="22324-130">date</span></span>      | <span data-ttu-id="22324-131">日付</span><span class="sxs-lookup"><span data-stu-id="22324-131">Date</span></span>   | <span data-ttu-id="22324-132">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="22324-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="22324-133">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="22324-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="22324-134">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="22324-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="22324-135">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="22324-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="22324-136">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="22324-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="22324-137">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="22324-137">The default output type is text/csv.</span></span> <span data-ttu-id="22324-138">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="22324-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22324-139">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="22324-139">Request headers</span></span>

| <span data-ttu-id="22324-140">名前</span><span class="sxs-lookup"><span data-stu-id="22324-140">Name</span></span>          | <span data-ttu-id="22324-141">説明</span><span class="sxs-lookup"><span data-stu-id="22324-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="22324-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="22324-142">Authorization</span></span> | <span data-ttu-id="22324-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="22324-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="22324-145">応答</span><span class="sxs-lookup"><span data-stu-id="22324-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="22324-146">CSV</span><span class="sxs-lookup"><span data-stu-id="22324-146">CSV</span></span>

<span data-ttu-id="22324-147">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="22324-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="22324-148">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="22324-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="22324-149">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="22324-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="22324-150">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="22324-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="22324-151">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="22324-151">Report Refresh Date</span></span>
- <span data-ttu-id="22324-152">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="22324-152">User Principal Name</span></span>
- <span data-ttu-id="22324-153">表示名</span><span class="sxs-lookup"><span data-stu-id="22324-153">Display Name</span></span>
- <span data-ttu-id="22324-154">ユーザーの状態</span><span class="sxs-lookup"><span data-stu-id="22324-154">User State</span></span>
- <span data-ttu-id="22324-155">状態変更日付</span><span class="sxs-lookup"><span data-stu-id="22324-155">State Change Date</span></span>
- <span data-ttu-id="22324-156">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="22324-156">Last Activity Date</span></span>
- <span data-ttu-id="22324-157">Web の使用</span><span class="sxs-lookup"><span data-stu-id="22324-157">Used Web</span></span>
- <span data-ttu-id="22324-158">Windows スマートフォンの使用</span><span class="sxs-lookup"><span data-stu-id="22324-158">Used Windows Phone</span></span>
- <span data-ttu-id="22324-159">Android スマートフォンの使用</span><span class="sxs-lookup"><span data-stu-id="22324-159">Used Android Phone</span></span>
- <span data-ttu-id="22324-160">iPhone の使用</span><span class="sxs-lookup"><span data-stu-id="22324-160">Used iPhone</span></span>
- <span data-ttu-id="22324-161">IPad の使用</span><span class="sxs-lookup"><span data-stu-id="22324-161">Used iPad</span></span>
- <span data-ttu-id="22324-162">その他の使用</span><span class="sxs-lookup"><span data-stu-id="22324-162">Used Others</span></span>
- <span data-ttu-id="22324-163">レポート期間</span><span class="sxs-lookup"><span data-stu-id="22324-163">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="22324-164">JSON</span><span class="sxs-lookup"><span data-stu-id="22324-164">JSON</span></span>

<span data-ttu-id="22324-165">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="22324-165">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="22324-166">この要求の既定のページ サイズは、アイテムは 200 個です。</span><span class="sxs-lookup"><span data-stu-id="22324-166">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="22324-167">使用例</span><span class="sxs-lookup"><span data-stu-id="22324-167">Example</span></span>

### <a name="csv"></a><span data-ttu-id="22324-168">CSV</span><span class="sxs-lookup"><span data-stu-id="22324-168">CSV</span></span>

<span data-ttu-id="22324-169">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="22324-169">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="22324-170">要求</span><span class="sxs-lookup"><span data-stu-id="22324-170">Request</span></span>

<span data-ttu-id="22324-171">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="22324-171">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="22324-172">応答</span><span class="sxs-lookup"><span data-stu-id="22324-172">Response</span></span>

<span data-ttu-id="22324-173">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="22324-173">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="22324-174">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="22324-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Used Web,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Used Others,Report Period
```

### <a name="json"></a><span data-ttu-id="22324-175">JSON</span><span class="sxs-lookup"><span data-stu-id="22324-175">JSON</span></span>

<span data-ttu-id="22324-176">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="22324-176">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="22324-177">要求</span><span class="sxs-lookup"><span data-stu-id="22324-177">Request</span></span>

<span data-ttu-id="22324-178">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="22324-178">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="22324-179">応答</span><span class="sxs-lookup"><span data-stu-id="22324-179">Response</span></span>

<span data-ttu-id="22324-180">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="22324-180">The following is an example of the response.</span></span>

> <span data-ttu-id="22324-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="22324-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 442

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerDeviceUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-06", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "userState": "active", 
      "stateChangeDate": "2012-06-26", 
      "lastActivityDate": "2017-09-06", 
      "usedWeb": true, 
      "usedWindowsPhone": false, 
      "usedAndroidPhone": false, 
      "usediPhone": false, 
      "usediPad": false, 
      "usedOthers": false, 
      "reportPeriod": "7"
    }
  ]
}
```