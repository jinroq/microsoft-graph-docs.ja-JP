---
title: 'reportRoot: getYammerDeviceUsageUserCounts'
description: デバイスの種類別に日次ユーザーの数を取得します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: bee50d497bb44ccdfdc5d7e9940818f639c39fa9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510380"
---
# <a name="reportroot-getyammerdeviceusageusercounts"></a><span data-ttu-id="868b8-103">reportRoot: getYammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="868b8-103">reportRoot: getYammerDeviceUsageUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="868b8-104">デバイスの種類別に日次ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="868b8-104">Get the number of daily users by device type.</span></span>

> <span data-ttu-id="868b8-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer デバイスの使用状況](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="868b8-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="868b8-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="868b8-106">Permissions</span></span>

<span data-ttu-id="868b8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="868b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="868b8-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="868b8-109">Permission type</span></span>                        | <span data-ttu-id="868b8-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="868b8-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="868b8-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="868b8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="868b8-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="868b8-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="868b8-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="868b8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="868b8-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="868b8-114">Not supported.</span></span>                           |
| <span data-ttu-id="868b8-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="868b8-115">Application</span></span>                            | <span data-ttu-id="868b8-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="868b8-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="868b8-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="868b8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="868b8-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="868b8-118">Function parameters</span></span>

<span data-ttu-id="868b8-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="868b8-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="868b8-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="868b8-120">Parameter</span></span> | <span data-ttu-id="868b8-121">型</span><span class="sxs-lookup"><span data-stu-id="868b8-121">Type</span></span>   | <span data-ttu-id="868b8-122">説明</span><span class="sxs-lookup"><span data-stu-id="868b8-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="868b8-123">period</span><span class="sxs-lookup"><span data-stu-id="868b8-123">period</span></span>    | <span data-ttu-id="868b8-124">文字列</span><span class="sxs-lookup"><span data-stu-id="868b8-124">string</span></span> | <span data-ttu-id="868b8-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="868b8-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="868b8-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="868b8-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="868b8-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="868b8-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="868b8-128">必須。</span><span class="sxs-lookup"><span data-stu-id="868b8-128">Required.</span></span> |

<span data-ttu-id="868b8-129">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="868b8-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="868b8-130">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="868b8-130">The default output type is text/csv.</span></span> <span data-ttu-id="868b8-131">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="868b8-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="868b8-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="868b8-132">Request headers</span></span>

| <span data-ttu-id="868b8-133">名前</span><span class="sxs-lookup"><span data-stu-id="868b8-133">Name</span></span>          | <span data-ttu-id="868b8-134">説明</span><span class="sxs-lookup"><span data-stu-id="868b8-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="868b8-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="868b8-135">Authorization</span></span> | <span data-ttu-id="868b8-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="868b8-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="868b8-138">応答</span><span class="sxs-lookup"><span data-stu-id="868b8-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="868b8-139">CSV</span><span class="sxs-lookup"><span data-stu-id="868b8-139">CSV</span></span>

<span data-ttu-id="868b8-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="868b8-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="868b8-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="868b8-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="868b8-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="868b8-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="868b8-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="868b8-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="868b8-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="868b8-144">Report Refresh Date</span></span>
- <span data-ttu-id="868b8-145">Web</span><span class="sxs-lookup"><span data-stu-id="868b8-145">Web</span></span>
- <span data-ttu-id="868b8-146">Windows スマートフォン</span><span class="sxs-lookup"><span data-stu-id="868b8-146">Windows Phone</span></span>
- <span data-ttu-id="868b8-147">Android スマートフォン</span><span class="sxs-lookup"><span data-stu-id="868b8-147">Android Phone</span></span>
- <span data-ttu-id="868b8-148">iPhone</span><span class="sxs-lookup"><span data-stu-id="868b8-148">iPhone</span></span>
- <span data-ttu-id="868b8-149">iPad</span><span class="sxs-lookup"><span data-stu-id="868b8-149">iPad</span></span>
- <span data-ttu-id="868b8-150">その他</span><span class="sxs-lookup"><span data-stu-id="868b8-150">Other</span></span>
- <span data-ttu-id="868b8-151">レポート日付</span><span class="sxs-lookup"><span data-stu-id="868b8-151">Report Date</span></span>
- <span data-ttu-id="868b8-152">レポート期間</span><span class="sxs-lookup"><span data-stu-id="868b8-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="868b8-153">JSON</span><span class="sxs-lookup"><span data-stu-id="868b8-153">JSON</span></span>

<span data-ttu-id="868b8-154">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="868b8-154">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="868b8-155">例</span><span class="sxs-lookup"><span data-stu-id="868b8-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="868b8-156">CSV</span><span class="sxs-lookup"><span data-stu-id="868b8-156">CSV</span></span>

<span data-ttu-id="868b8-157">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="868b8-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="868b8-158">要求</span><span class="sxs-lookup"><span data-stu-id="868b8-158">Request</span></span>

<span data-ttu-id="868b8-159">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="868b8-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="868b8-160">応答</span><span class="sxs-lookup"><span data-stu-id="868b8-160">Response</span></span>

<span data-ttu-id="868b8-161">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="868b8-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="868b8-162">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="868b8-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="868b8-163">JSON</span><span class="sxs-lookup"><span data-stu-id="868b8-163">JSON</span></span>

<span data-ttu-id="868b8-164">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="868b8-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="868b8-165">要求</span><span class="sxs-lookup"><span data-stu-id="868b8-165">Request</span></span>

<span data-ttu-id="868b8-166">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="868b8-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="868b8-167">応答</span><span class="sxs-lookup"><span data-stu-id="868b8-167">Response</span></span>

<span data-ttu-id="868b8-168">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="868b8-168">The following is an example of the response.</span></span>

> <span data-ttu-id="868b8-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="868b8-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getyammerdeviceusageusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
