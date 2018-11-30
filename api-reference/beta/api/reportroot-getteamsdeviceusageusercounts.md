---
title: 'reportRoot: getTeamsDeviceUsageUserCounts'
description: デバイスの種類ごとに、Microsoft Teams の日次ユニーク ユーザーの数を取得します。
ms.openlocfilehash: f672e434588f4a9d9a80ddb72bbd80e36c134b5e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074550"
---
# <a name="reportroot-getteamsdeviceusageusercounts"></a><span data-ttu-id="1165a-103">reportRoot: getTeamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="1165a-103">reportRoot: getTeamsDeviceUsageUserCounts</span></span>

> <span data-ttu-id="1165a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1165a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1165a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1165a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1165a-106">デバイスの種類ごとに、Microsoft Teams の日次ユニーク ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="1165a-106">Get the number of Microsoft Teams daily unique users by device type.</span></span>

## <a name="permissions"></a><span data-ttu-id="1165a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1165a-107">Permissions</span></span>

<span data-ttu-id="1165a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1165a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1165a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1165a-110">Permission type</span></span>                        | <span data-ttu-id="1165a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1165a-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1165a-112">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="1165a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="1165a-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1165a-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1165a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1165a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1165a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1165a-115">Not supported.</span></span>                           |
| <span data-ttu-id="1165a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1165a-116">Application</span></span>                            | <span data-ttu-id="1165a-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1165a-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1165a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1165a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="1165a-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="1165a-119">Function parameters</span></span>

<span data-ttu-id="1165a-120">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="1165a-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="1165a-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="1165a-121">Parameter</span></span> | <span data-ttu-id="1165a-122">型</span><span class="sxs-lookup"><span data-stu-id="1165a-122">Type</span></span>   | <span data-ttu-id="1165a-123">説明</span><span class="sxs-lookup"><span data-stu-id="1165a-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1165a-124">period</span><span class="sxs-lookup"><span data-stu-id="1165a-124">period</span></span>    | <span data-ttu-id="1165a-125">文字列</span><span class="sxs-lookup"><span data-stu-id="1165a-125">string</span></span> | <span data-ttu-id="1165a-126">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="1165a-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1165a-127">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="1165a-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1165a-128">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="1165a-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="1165a-129">必須。</span><span class="sxs-lookup"><span data-stu-id="1165a-129">Required.</span></span> |

<span data-ttu-id="1165a-130">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="1165a-130">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="1165a-131">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="1165a-131">The default output type is text/csv.</span></span> <span data-ttu-id="1165a-132">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="1165a-132">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1165a-133">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1165a-133">Request headers</span></span>

| <span data-ttu-id="1165a-134">名前</span><span class="sxs-lookup"><span data-stu-id="1165a-134">Name</span></span>          | <span data-ttu-id="1165a-135">説明</span><span class="sxs-lookup"><span data-stu-id="1165a-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1165a-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="1165a-136">Authorization</span></span> | <span data-ttu-id="1165a-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1165a-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1165a-139">応答</span><span class="sxs-lookup"><span data-stu-id="1165a-139">Response</span></span>

### <a name="csv"></a><span data-ttu-id="1165a-140">CSV</span><span class="sxs-lookup"><span data-stu-id="1165a-140">CSV</span></span>

<span data-ttu-id="1165a-141">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="1165a-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1165a-142">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="1165a-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1165a-143">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="1165a-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1165a-144">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="1165a-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1165a-145">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="1165a-145">Report Refresh Date</span></span>
- <span data-ttu-id="1165a-146">Web</span><span class="sxs-lookup"><span data-stu-id="1165a-146">Web</span></span>
- <span data-ttu-id="1165a-147">Windows スマートフォン</span><span class="sxs-lookup"><span data-stu-id="1165a-147">Windows Phone</span></span>
- <span data-ttu-id="1165a-148">Android スマートフォン</span><span class="sxs-lookup"><span data-stu-id="1165a-148">Android Phone</span></span>
- <span data-ttu-id="1165a-149">iOS</span><span class="sxs-lookup"><span data-stu-id="1165a-149">iOS</span></span>
- <span data-ttu-id="1165a-150">Mac</span><span class="sxs-lookup"><span data-stu-id="1165a-150">Mac</span></span>
- <span data-ttu-id="1165a-151">Windows</span><span class="sxs-lookup"><span data-stu-id="1165a-151">Windows</span></span>
- <span data-ttu-id="1165a-152">レポート日付</span><span class="sxs-lookup"><span data-stu-id="1165a-152">Report Date</span></span>
- <span data-ttu-id="1165a-153">レポート期間</span><span class="sxs-lookup"><span data-stu-id="1165a-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="1165a-154">JSON</span><span class="sxs-lookup"><span data-stu-id="1165a-154">JSON</span></span>

<span data-ttu-id="1165a-155">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="1165a-155">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1165a-156">使用例</span><span class="sxs-lookup"><span data-stu-id="1165a-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="1165a-157">CSV</span><span class="sxs-lookup"><span data-stu-id="1165a-157">CSV</span></span>

<span data-ttu-id="1165a-158">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="1165a-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="1165a-159">要求</span><span class="sxs-lookup"><span data-stu-id="1165a-159">Request</span></span>

<span data-ttu-id="1165a-160">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1165a-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="1165a-161">応答</span><span class="sxs-lookup"><span data-stu-id="1165a-161">Response</span></span>

<span data-ttu-id="1165a-162">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1165a-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="1165a-163">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="1165a-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="1165a-164">JSON</span><span class="sxs-lookup"><span data-stu-id="1165a-164">JSON</span></span>

<span data-ttu-id="1165a-165">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="1165a-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="1165a-166">要求</span><span class="sxs-lookup"><span data-stu-id="1165a-166">Request</span></span>

<span data-ttu-id="1165a-167">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1165a-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="1165a-168">応答</span><span class="sxs-lookup"><span data-stu-id="1165a-168">Response</span></span>

<span data-ttu-id="1165a-169">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1165a-169">The following is an example of the response.</span></span>

> <span data-ttu-id="1165a-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1165a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 269

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 13, 
      "windowsPhone": 0, 
      "androidPhone": 22, 
      "ios": 75, 
      "mac": 16, 
      "windows": 257, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
