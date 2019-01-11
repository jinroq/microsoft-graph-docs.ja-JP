---
title: 'reportRoot: getYammerDeviceUsageUserCounts'
description: デバイスの種類別に日次ユーザーの数を取得します。
localization_priority: Normal
ms.openlocfilehash: 78c17de276e45b12936fcdf0f4b58c975388d101
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812622"
---
# <a name="reportroot-getyammerdeviceusageusercounts"></a><span data-ttu-id="7f5ea-103">reportRoot: getYammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="7f5ea-103">reportRoot: getYammerDeviceUsageUserCounts</span></span>

> <span data-ttu-id="7f5ea-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7f5ea-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f5ea-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f5ea-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7f5ea-106">デバイスの種類別に日次ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="7f5ea-106">Get the number of daily users by device type.</span></span>

> <span data-ttu-id="7f5ea-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer デバイスの使用状況](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f5ea-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="7f5ea-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7f5ea-108">Permissions</span></span>

<span data-ttu-id="7f5ea-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f5ea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7f5ea-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7f5ea-111">Permission type</span></span>                        | <span data-ttu-id="7f5ea-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7f5ea-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7f5ea-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="7f5ea-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="7f5ea-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f5ea-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7f5ea-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7f5ea-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f5ea-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f5ea-116">Not supported.</span></span>                           |
| <span data-ttu-id="7f5ea-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7f5ea-117">Application</span></span>                            | <span data-ttu-id="7f5ea-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f5ea-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7f5ea-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7f5ea-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="7f5ea-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="7f5ea-120">Function parameters</span></span>

<span data-ttu-id="7f5ea-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="7f5ea-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="7f5ea-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="7f5ea-122">Parameter</span></span> | <span data-ttu-id="7f5ea-123">Type</span><span class="sxs-lookup"><span data-stu-id="7f5ea-123">Type</span></span>   | <span data-ttu-id="7f5ea-124">説明</span><span class="sxs-lookup"><span data-stu-id="7f5ea-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7f5ea-125">period</span><span class="sxs-lookup"><span data-stu-id="7f5ea-125">period</span></span>    | <span data-ttu-id="7f5ea-126">文字列</span><span class="sxs-lookup"><span data-stu-id="7f5ea-126">string</span></span> | <span data-ttu-id="7f5ea-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="7f5ea-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7f5ea-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="7f5ea-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7f5ea-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="7f5ea-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="7f5ea-130">必須。</span><span class="sxs-lookup"><span data-stu-id="7f5ea-130">Required.</span></span> |

<span data-ttu-id="7f5ea-131">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="7f5ea-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="7f5ea-132">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="7f5ea-132">The default output type is text/csv.</span></span> <span data-ttu-id="7f5ea-133">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="7f5ea-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7f5ea-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f5ea-134">Request headers</span></span>

| <span data-ttu-id="7f5ea-135">名前</span><span class="sxs-lookup"><span data-stu-id="7f5ea-135">Name</span></span>          | <span data-ttu-id="7f5ea-136">説明</span><span class="sxs-lookup"><span data-stu-id="7f5ea-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7f5ea-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f5ea-137">Authorization</span></span> | <span data-ttu-id="7f5ea-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7f5ea-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7f5ea-140">応答</span><span class="sxs-lookup"><span data-stu-id="7f5ea-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="7f5ea-141">CSV</span><span class="sxs-lookup"><span data-stu-id="7f5ea-141">CSV</span></span>

<span data-ttu-id="7f5ea-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="7f5ea-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7f5ea-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="7f5ea-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7f5ea-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="7f5ea-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7f5ea-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="7f5ea-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7f5ea-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="7f5ea-146">Report Refresh Date</span></span>
- <span data-ttu-id="7f5ea-147">Web</span><span class="sxs-lookup"><span data-stu-id="7f5ea-147">Web</span></span>
- <span data-ttu-id="7f5ea-148">Windows スマートフォン</span><span class="sxs-lookup"><span data-stu-id="7f5ea-148">Windows Phone</span></span>
- <span data-ttu-id="7f5ea-149">Android スマートフォン</span><span class="sxs-lookup"><span data-stu-id="7f5ea-149">Android Phone</span></span>
- <span data-ttu-id="7f5ea-150">iPhone</span><span class="sxs-lookup"><span data-stu-id="7f5ea-150">iPhone</span></span>
- <span data-ttu-id="7f5ea-151">iPad</span><span class="sxs-lookup"><span data-stu-id="7f5ea-151">iPad</span></span>
- <span data-ttu-id="7f5ea-152">その他</span><span class="sxs-lookup"><span data-stu-id="7f5ea-152">Other</span></span>
- <span data-ttu-id="7f5ea-153">レポート日付</span><span class="sxs-lookup"><span data-stu-id="7f5ea-153">Report Date</span></span>
- <span data-ttu-id="7f5ea-154">レポート期間</span><span class="sxs-lookup"><span data-stu-id="7f5ea-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="7f5ea-155">JSON</span><span class="sxs-lookup"><span data-stu-id="7f5ea-155">JSON</span></span>

<span data-ttu-id="7f5ea-156">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="7f5ea-156">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f5ea-157">例</span><span class="sxs-lookup"><span data-stu-id="7f5ea-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="7f5ea-158">CSV</span><span class="sxs-lookup"><span data-stu-id="7f5ea-158">CSV</span></span>

<span data-ttu-id="7f5ea-159">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="7f5ea-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="7f5ea-160">要求</span><span class="sxs-lookup"><span data-stu-id="7f5ea-160">Request</span></span>

<span data-ttu-id="7f5ea-161">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7f5ea-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="7f5ea-162">応答</span><span class="sxs-lookup"><span data-stu-id="7f5ea-162">Response</span></span>

<span data-ttu-id="7f5ea-163">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7f5ea-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7f5ea-164">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="7f5ea-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="7f5ea-165">JSON</span><span class="sxs-lookup"><span data-stu-id="7f5ea-165">JSON</span></span>

<span data-ttu-id="7f5ea-166">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="7f5ea-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="7f5ea-167">要求</span><span class="sxs-lookup"><span data-stu-id="7f5ea-167">Request</span></span>

<span data-ttu-id="7f5ea-168">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7f5ea-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="7f5ea-169">応答</span><span class="sxs-lookup"><span data-stu-id="7f5ea-169">Response</span></span>

<span data-ttu-id="7f5ea-170">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7f5ea-170">The following is an example of the response.</span></span>

> <span data-ttu-id="7f5ea-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7f5ea-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 284

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerDeviceUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 63, 
      "windowsPhone": 1, 
      "androidPhone": 17, 
      "iPhone": 23, 
      "iPad": 1, 
      "other": 2, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
