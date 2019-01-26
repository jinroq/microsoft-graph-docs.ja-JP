---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserDetail'
description: ユーザー別の Skype for Business デバイス使用状況に関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 32b3a3e2ebf0d05440cb38a1bc0ef7fdda983258
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576095"
---
# <a name="reportroot-getskypeforbusinessdeviceusageuserdetail"></a><span data-ttu-id="5ddde-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="5ddde-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ddde-104">ユーザー別の Skype for Business デバイス使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="5ddde-104">Get details about Skype for Business device usage by user.</span></span>

> <span data-ttu-id="5ddde-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: 使用している Skype for Business クライアント](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ddde-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="5ddde-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5ddde-106">Permissions</span></span>

<span data-ttu-id="5ddde-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ddde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5ddde-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5ddde-109">Permission type</span></span>                        | <span data-ttu-id="5ddde-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5ddde-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5ddde-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="5ddde-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5ddde-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ddde-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5ddde-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5ddde-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ddde-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ddde-114">Not supported.</span></span>                           |
| <span data-ttu-id="5ddde-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5ddde-115">Application</span></span>                            | <span data-ttu-id="5ddde-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ddde-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5ddde-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5ddde-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="5ddde-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="5ddde-118">Function parameters</span></span>

<span data-ttu-id="5ddde-119">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="5ddde-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="5ddde-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="5ddde-120">Parameter</span></span> | <span data-ttu-id="5ddde-121">型</span><span class="sxs-lookup"><span data-stu-id="5ddde-121">Type</span></span>   | <span data-ttu-id="5ddde-122">説明</span><span class="sxs-lookup"><span data-stu-id="5ddde-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5ddde-123">period</span><span class="sxs-lookup"><span data-stu-id="5ddde-123">period</span></span>    | <span data-ttu-id="5ddde-124">文字列</span><span class="sxs-lookup"><span data-stu-id="5ddde-124">string</span></span> | <span data-ttu-id="5ddde-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="5ddde-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5ddde-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="5ddde-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5ddde-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="5ddde-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="5ddde-128">date</span><span class="sxs-lookup"><span data-stu-id="5ddde-128">date</span></span>      | <span data-ttu-id="5ddde-129">日付</span><span class="sxs-lookup"><span data-stu-id="5ddde-129">Date</span></span>   | <span data-ttu-id="5ddde-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="5ddde-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="5ddde-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="5ddde-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="5ddde-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="5ddde-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="5ddde-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5ddde-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="5ddde-134">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5ddde-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="5ddde-135">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="5ddde-135">The default output type is text/csv.</span></span> <span data-ttu-id="5ddde-136">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="5ddde-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ddde-137">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5ddde-137">Request headers</span></span>

| <span data-ttu-id="5ddde-138">名前</span><span class="sxs-lookup"><span data-stu-id="5ddde-138">Name</span></span>          | <span data-ttu-id="5ddde-139">説明</span><span class="sxs-lookup"><span data-stu-id="5ddde-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5ddde-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ddde-140">Authorization</span></span> | <span data-ttu-id="5ddde-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5ddde-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5ddde-143">応答</span><span class="sxs-lookup"><span data-stu-id="5ddde-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="5ddde-144">CSV</span><span class="sxs-lookup"><span data-stu-id="5ddde-144">CSV</span></span>

<span data-ttu-id="5ddde-145">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="5ddde-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5ddde-146">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="5ddde-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5ddde-147">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="5ddde-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5ddde-148">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="5ddde-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5ddde-149">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="5ddde-149">Report Refresh Date</span></span>
- <span data-ttu-id="5ddde-150">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="5ddde-150">User Principal Name</span></span>
- <span data-ttu-id="5ddde-151">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="5ddde-151">Last Activity Date</span></span>
- <span data-ttu-id="5ddde-152">Windows の使用</span><span class="sxs-lookup"><span data-stu-id="5ddde-152">Used Windows</span></span>
- <span data-ttu-id="5ddde-153">Windows スマートフォンの使用</span><span class="sxs-lookup"><span data-stu-id="5ddde-153">Used Windows Phone</span></span>
- <span data-ttu-id="5ddde-154">Android スマートフォンの使用</span><span class="sxs-lookup"><span data-stu-id="5ddde-154">Used Android Phone</span></span>
- <span data-ttu-id="5ddde-155">iPhone の使用</span><span class="sxs-lookup"><span data-stu-id="5ddde-155">Used iPhone</span></span>
- <span data-ttu-id="5ddde-156">IPad の使用</span><span class="sxs-lookup"><span data-stu-id="5ddde-156">Used iPad</span></span>
- <span data-ttu-id="5ddde-157">レポート期間</span><span class="sxs-lookup"><span data-stu-id="5ddde-157">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="5ddde-158">JSON</span><span class="sxs-lookup"><span data-stu-id="5ddde-158">JSON</span></span>

<span data-ttu-id="5ddde-159">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[skypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="5ddde-159">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="5ddde-160">この要求の既定のページ サイズは、アイテムは 200 個です。</span><span class="sxs-lookup"><span data-stu-id="5ddde-160">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="5ddde-161">例</span><span class="sxs-lookup"><span data-stu-id="5ddde-161">Example</span></span>

### <a name="csv"></a><span data-ttu-id="5ddde-162">CSV</span><span class="sxs-lookup"><span data-stu-id="5ddde-162">CSV</span></span>

<span data-ttu-id="5ddde-163">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="5ddde-163">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="5ddde-164">要求</span><span class="sxs-lookup"><span data-stu-id="5ddde-164">Request</span></span>

<span data-ttu-id="5ddde-165">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5ddde-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="5ddde-166">応答</span><span class="sxs-lookup"><span data-stu-id="5ddde-166">Response</span></span>

<span data-ttu-id="5ddde-167">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5ddde-167">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="5ddde-168">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="5ddde-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="5ddde-169">JSON</span><span class="sxs-lookup"><span data-stu-id="5ddde-169">JSON</span></span>

<span data-ttu-id="5ddde-170">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="5ddde-170">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="5ddde-171">要求</span><span class="sxs-lookup"><span data-stu-id="5ddde-171">Request</span></span>

<span data-ttu-id="5ddde-172">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5ddde-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="5ddde-173">応答</span><span class="sxs-lookup"><span data-stu-id="5ddde-173">Response</span></span>

<span data-ttu-id="5ddde-174">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5ddde-174">The following is an example of the response.</span></span>

> <span data-ttu-id="5ddde-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5ddde-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessdeviceusageuserdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
