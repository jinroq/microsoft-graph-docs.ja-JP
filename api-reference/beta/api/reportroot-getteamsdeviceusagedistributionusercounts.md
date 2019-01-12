---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: デバイスの種類ごとに、選択した期間の Microsoft Teams のユニーク ユーザーの数を取得します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 7c5b96200eb48b4d4009ad9602bc6cc001e441e3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930580"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="8b6d7-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="8b6d7-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

> <span data-ttu-id="8b6d7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8b6d7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b6d7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b6d7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8b6d7-106">デバイスの種類ごとに、選択した期間の Microsoft Teams のユニーク ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="8b6d7-106">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b6d7-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8b6d7-107">Permissions</span></span>

<span data-ttu-id="8b6d7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8b6d7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8b6d7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8b6d7-110">Permission type</span></span>                        | <span data-ttu-id="8b6d7-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8b6d7-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8b6d7-112">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="8b6d7-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b6d7-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b6d7-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8b6d7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8b6d7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b6d7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b6d7-115">Not supported.</span></span>                           |
| <span data-ttu-id="8b6d7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8b6d7-116">Application</span></span>                            | <span data-ttu-id="8b6d7-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b6d7-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8b6d7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8b6d7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="8b6d7-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="8b6d7-119">Function parameters</span></span>

<span data-ttu-id="8b6d7-120">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="8b6d7-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="8b6d7-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="8b6d7-121">Parameter</span></span> | <span data-ttu-id="8b6d7-122">Type</span><span class="sxs-lookup"><span data-stu-id="8b6d7-122">Type</span></span>   | <span data-ttu-id="8b6d7-123">説明</span><span class="sxs-lookup"><span data-stu-id="8b6d7-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8b6d7-124">period</span><span class="sxs-lookup"><span data-stu-id="8b6d7-124">period</span></span>    | <span data-ttu-id="8b6d7-125">文字列</span><span class="sxs-lookup"><span data-stu-id="8b6d7-125">string</span></span> | <span data-ttu-id="8b6d7-126">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="8b6d7-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8b6d7-127">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="8b6d7-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8b6d7-128">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="8b6d7-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="8b6d7-129">必須。</span><span class="sxs-lookup"><span data-stu-id="8b6d7-129">Required.</span></span> |

<span data-ttu-id="8b6d7-130">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="8b6d7-130">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="8b6d7-131">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="8b6d7-131">The default output type is text/csv.</span></span> <span data-ttu-id="8b6d7-132">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="8b6d7-132">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8b6d7-133">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8b6d7-133">Request headers</span></span>

| <span data-ttu-id="8b6d7-134">名前</span><span class="sxs-lookup"><span data-stu-id="8b6d7-134">Name</span></span>          | <span data-ttu-id="8b6d7-135">説明</span><span class="sxs-lookup"><span data-stu-id="8b6d7-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8b6d7-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b6d7-136">Authorization</span></span> | <span data-ttu-id="8b6d7-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8b6d7-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8b6d7-139">応答</span><span class="sxs-lookup"><span data-stu-id="8b6d7-139">Response</span></span>

### <a name="csv"></a><span data-ttu-id="8b6d7-140">CSV</span><span class="sxs-lookup"><span data-stu-id="8b6d7-140">CSV</span></span>

<span data-ttu-id="8b6d7-141">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="8b6d7-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8b6d7-142">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="8b6d7-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8b6d7-143">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="8b6d7-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8b6d7-144">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="8b6d7-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8b6d7-145">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="8b6d7-145">Report Refresh Date</span></span>
- <span data-ttu-id="8b6d7-146">Web</span><span class="sxs-lookup"><span data-stu-id="8b6d7-146">Web</span></span>
- <span data-ttu-id="8b6d7-147">Windows スマートフォン</span><span class="sxs-lookup"><span data-stu-id="8b6d7-147">Windows Phone</span></span>
- <span data-ttu-id="8b6d7-148">Android スマートフォン</span><span class="sxs-lookup"><span data-stu-id="8b6d7-148">Android Phone</span></span>
- <span data-ttu-id="8b6d7-149">iOS</span><span class="sxs-lookup"><span data-stu-id="8b6d7-149">iOS</span></span>
- <span data-ttu-id="8b6d7-150">Mac</span><span class="sxs-lookup"><span data-stu-id="8b6d7-150">Mac</span></span>
- <span data-ttu-id="8b6d7-151">Windows</span><span class="sxs-lookup"><span data-stu-id="8b6d7-151">Windows</span></span>
- <span data-ttu-id="8b6d7-152">レポート期間</span><span class="sxs-lookup"><span data-stu-id="8b6d7-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="8b6d7-153">JSON</span><span class="sxs-lookup"><span data-stu-id="8b6d7-153">JSON</span></span>

<span data-ttu-id="8b6d7-154">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="8b6d7-154">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b6d7-155">例</span><span class="sxs-lookup"><span data-stu-id="8b6d7-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="8b6d7-156">CSV</span><span class="sxs-lookup"><span data-stu-id="8b6d7-156">CSV</span></span>

<span data-ttu-id="8b6d7-157">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="8b6d7-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="8b6d7-158">要求</span><span class="sxs-lookup"><span data-stu-id="8b6d7-158">Request</span></span>

<span data-ttu-id="8b6d7-159">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8b6d7-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="8b6d7-160">応答</span><span class="sxs-lookup"><span data-stu-id="8b6d7-160">Response</span></span>

<span data-ttu-id="8b6d7-161">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8b6d7-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="8b6d7-162">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="8b6d7-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Period
```

### <a name="json"></a><span data-ttu-id="8b6d7-163">JSON</span><span class="sxs-lookup"><span data-stu-id="8b6d7-163">JSON</span></span>

<span data-ttu-id="8b6d7-164">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="8b6d7-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="8b6d7-165">要求</span><span class="sxs-lookup"><span data-stu-id="8b6d7-165">Request</span></span>

<span data-ttu-id="8b6d7-166">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8b6d7-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="8b6d7-167">応答</span><span class="sxs-lookup"><span data-stu-id="8b6d7-167">Response</span></span>

<span data-ttu-id="8b6d7-168">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8b6d7-168">The following is an example of the response.</span></span>

> <span data-ttu-id="8b6d7-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8b6d7-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 243

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageDistributionUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 51, 
      "windowsPhone": 2, 
      "androidPhone": 34, 
      "ios": 76, 
      "mac": 40, 
      "windows": 491, 
      "reportPeriod": "7"
    }
  ]
}
```
