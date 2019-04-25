---
title: 'reportRoot: getYammerDeviceUsageUserDetail function'
description: ユーザー別の Yammer デバイス使用状況に関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 37e3a5fae633dd3d202c82d54573a77a8f6dfd6c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537863"
---
# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="4bfcd-103">reportRoot: getYammerDeviceUsageUserDetail function</span><span class="sxs-lookup"><span data-stu-id="4bfcd-103">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bfcd-104">ユーザー別の Yammer デバイス使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-104">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="4bfcd-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer デバイスの使用状況](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="4bfcd-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4bfcd-106">Permissions</span></span>

<span data-ttu-id="4bfcd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4bfcd-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4bfcd-109">Permission type</span></span>                        | <span data-ttu-id="4bfcd-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4bfcd-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4bfcd-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4bfcd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4bfcd-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4bfcd-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4bfcd-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4bfcd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bfcd-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-114">Not supported.</span></span>                           |
| <span data-ttu-id="4bfcd-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4bfcd-115">Application</span></span>                            | <span data-ttu-id="4bfcd-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4bfcd-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4bfcd-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4bfcd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="4bfcd-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="4bfcd-118">Function parameters</span></span>

<span data-ttu-id="4bfcd-119">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="4bfcd-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="4bfcd-120">Parameter</span></span> | <span data-ttu-id="4bfcd-121">型</span><span class="sxs-lookup"><span data-stu-id="4bfcd-121">Type</span></span>   | <span data-ttu-id="4bfcd-122">説明</span><span class="sxs-lookup"><span data-stu-id="4bfcd-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4bfcd-123">period</span><span class="sxs-lookup"><span data-stu-id="4bfcd-123">period</span></span>    | <span data-ttu-id="4bfcd-124">文字列</span><span class="sxs-lookup"><span data-stu-id="4bfcd-124">string</span></span> | <span data-ttu-id="4bfcd-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4bfcd-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4bfcd-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="4bfcd-128">date</span><span class="sxs-lookup"><span data-stu-id="4bfcd-128">date</span></span>      | <span data-ttu-id="4bfcd-129">日付</span><span class="sxs-lookup"><span data-stu-id="4bfcd-129">Date</span></span>   | <span data-ttu-id="4bfcd-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="4bfcd-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="4bfcd-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="4bfcd-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="4bfcd-134">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4bfcd-135">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-135">The default output type is text/csv.</span></span> <span data-ttu-id="4bfcd-136">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4bfcd-137">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4bfcd-137">Request headers</span></span>

| <span data-ttu-id="4bfcd-138">名前</span><span class="sxs-lookup"><span data-stu-id="4bfcd-138">Name</span></span>          | <span data-ttu-id="4bfcd-139">説明</span><span class="sxs-lookup"><span data-stu-id="4bfcd-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4bfcd-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bfcd-140">Authorization</span></span> | <span data-ttu-id="4bfcd-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4bfcd-143">応答</span><span class="sxs-lookup"><span data-stu-id="4bfcd-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4bfcd-144">CSV</span><span class="sxs-lookup"><span data-stu-id="4bfcd-144">CSV</span></span>

<span data-ttu-id="4bfcd-145">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4bfcd-146">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4bfcd-147">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4bfcd-148">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4bfcd-149">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="4bfcd-149">Report Refresh Date</span></span>
- <span data-ttu-id="4bfcd-150">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="4bfcd-150">User Principal Name</span></span>
- <span data-ttu-id="4bfcd-151">表示名</span><span class="sxs-lookup"><span data-stu-id="4bfcd-151">Display Name</span></span>
- <span data-ttu-id="4bfcd-152">ユーザーの状態</span><span class="sxs-lookup"><span data-stu-id="4bfcd-152">User State</span></span>
- <span data-ttu-id="4bfcd-153">状態変更日付</span><span class="sxs-lookup"><span data-stu-id="4bfcd-153">State Change Date</span></span>
- <span data-ttu-id="4bfcd-154">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="4bfcd-154">Last Activity Date</span></span>
- <span data-ttu-id="4bfcd-155">Web の使用</span><span class="sxs-lookup"><span data-stu-id="4bfcd-155">Used Web</span></span>
- <span data-ttu-id="4bfcd-156">Windows スマートフォンの使用</span><span class="sxs-lookup"><span data-stu-id="4bfcd-156">Used Windows Phone</span></span>
- <span data-ttu-id="4bfcd-157">Android スマートフォンの使用</span><span class="sxs-lookup"><span data-stu-id="4bfcd-157">Used Android Phone</span></span>
- <span data-ttu-id="4bfcd-158">iPhone の使用</span><span class="sxs-lookup"><span data-stu-id="4bfcd-158">Used iPhone</span></span>
- <span data-ttu-id="4bfcd-159">IPad の使用</span><span class="sxs-lookup"><span data-stu-id="4bfcd-159">Used iPad</span></span>
- <span data-ttu-id="4bfcd-160">その他の使用</span><span class="sxs-lookup"><span data-stu-id="4bfcd-160">Used Others</span></span>
- <span data-ttu-id="4bfcd-161">レポート期間</span><span class="sxs-lookup"><span data-stu-id="4bfcd-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="4bfcd-162">JSON</span><span class="sxs-lookup"><span data-stu-id="4bfcd-162">JSON</span></span>

<span data-ttu-id="4bfcd-163">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-163">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="4bfcd-164">この要求の既定のページサイズは200アイテムです。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-164">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="4bfcd-165">例</span><span class="sxs-lookup"><span data-stu-id="4bfcd-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4bfcd-166">CSV</span><span class="sxs-lookup"><span data-stu-id="4bfcd-166">CSV</span></span>

<span data-ttu-id="4bfcd-167">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4bfcd-168">要求</span><span class="sxs-lookup"><span data-stu-id="4bfcd-168">Request</span></span>

<span data-ttu-id="4bfcd-169">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="4bfcd-170">応答</span><span class="sxs-lookup"><span data-stu-id="4bfcd-170">Response</span></span>

<span data-ttu-id="4bfcd-171">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4bfcd-172">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="4bfcd-173">JSON</span><span class="sxs-lookup"><span data-stu-id="4bfcd-173">JSON</span></span>

<span data-ttu-id="4bfcd-174">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4bfcd-175">要求</span><span class="sxs-lookup"><span data-stu-id="4bfcd-175">Request</span></span>

<span data-ttu-id="4bfcd-176">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="4bfcd-177">応答</span><span class="sxs-lookup"><span data-stu-id="4bfcd-177">Response</span></span>

<span data-ttu-id="4bfcd-178">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-178">The following is an example of the response.</span></span>

> <span data-ttu-id="4bfcd-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4bfcd-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getyammerdeviceusageuserdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
