---
title: 'reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts'
description: 組織内でそれぞれ別個のデバイスを使用するユーザーの数を取得します。 このレポートでは、Windows、Windows スマートフォン、Android スマートフォン、iPhone、iPad を含むデバイス別のユーザーの数を表示します。
ms.openlocfilehash: bee105fc41d18543c611f05d2a3e389ff6a84526
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068416"
---
# <a name="reportroot-getskypeforbusinessdeviceusagedistributionusercounts"></a><span data-ttu-id="b7f90-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="b7f90-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span></span>

> <span data-ttu-id="b7f90-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b7f90-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7f90-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7f90-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b7f90-107">組織内でそれぞれ別個のデバイスを使用するユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="b7f90-107">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="b7f90-108">このレポートでは、Windows、Windows スマートフォン、Android スマートフォン、iPhone、iPad を含むデバイス別のユーザーの数を表示します。</span><span class="sxs-lookup"><span data-stu-id="b7f90-108">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span>

> <span data-ttu-id="b7f90-109">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: 使用している Skype for Business クライアント](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b7f90-109">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="b7f90-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b7f90-110">Permissions</span></span>

<span data-ttu-id="b7f90-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b7f90-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b7f90-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b7f90-113">Permission type</span></span>                        | <span data-ttu-id="b7f90-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b7f90-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b7f90-115">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="b7f90-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="b7f90-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7f90-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b7f90-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b7f90-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7f90-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7f90-118">Not supported.</span></span>                           |
| <span data-ttu-id="b7f90-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b7f90-119">Application</span></span>                            | <span data-ttu-id="b7f90-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7f90-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b7f90-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b7f90-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="b7f90-122">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="b7f90-122">Function parameters</span></span>

<span data-ttu-id="b7f90-123">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="b7f90-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b7f90-124">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b7f90-124">Parameter</span></span> | <span data-ttu-id="b7f90-125">型</span><span class="sxs-lookup"><span data-stu-id="b7f90-125">Type</span></span>   | <span data-ttu-id="b7f90-126">説明</span><span class="sxs-lookup"><span data-stu-id="b7f90-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b7f90-127">period</span><span class="sxs-lookup"><span data-stu-id="b7f90-127">period</span></span>    | <span data-ttu-id="b7f90-128">文字列</span><span class="sxs-lookup"><span data-stu-id="b7f90-128">string</span></span> | <span data-ttu-id="b7f90-129">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="b7f90-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b7f90-130">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="b7f90-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b7f90-131">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="b7f90-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b7f90-132">必須。</span><span class="sxs-lookup"><span data-stu-id="b7f90-132">Required.</span></span> |

<span data-ttu-id="b7f90-133">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="b7f90-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="b7f90-134">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="b7f90-134">The default output type is text/csv.</span></span> <span data-ttu-id="b7f90-135">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="b7f90-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b7f90-136">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b7f90-136">Request headers</span></span>

| <span data-ttu-id="b7f90-137">名前</span><span class="sxs-lookup"><span data-stu-id="b7f90-137">Name</span></span>          | <span data-ttu-id="b7f90-138">説明</span><span class="sxs-lookup"><span data-stu-id="b7f90-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b7f90-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7f90-139">Authorization</span></span> | <span data-ttu-id="b7f90-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b7f90-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b7f90-142">応答</span><span class="sxs-lookup"><span data-stu-id="b7f90-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="b7f90-143">CSV</span><span class="sxs-lookup"><span data-stu-id="b7f90-143">CSV</span></span>

<span data-ttu-id="b7f90-144">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="b7f90-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b7f90-145">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="b7f90-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b7f90-146">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="b7f90-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b7f90-147">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="b7f90-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b7f90-148">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="b7f90-148">Report Refresh Date</span></span>
- <span data-ttu-id="b7f90-149">Windows</span><span class="sxs-lookup"><span data-stu-id="b7f90-149">Windows</span></span>
- <span data-ttu-id="b7f90-150">Windows スマートフォン</span><span class="sxs-lookup"><span data-stu-id="b7f90-150">Windows Phone</span></span>
- <span data-ttu-id="b7f90-151">Android スマートフォン</span><span class="sxs-lookup"><span data-stu-id="b7f90-151">Android Phone</span></span>
- <span data-ttu-id="b7f90-152">iPhone</span><span class="sxs-lookup"><span data-stu-id="b7f90-152">iPhone</span></span>
- <span data-ttu-id="b7f90-153">iPad</span><span class="sxs-lookup"><span data-stu-id="b7f90-153">iPad</span></span>
- <span data-ttu-id="b7f90-154">レポート期間</span><span class="sxs-lookup"><span data-stu-id="b7f90-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="b7f90-155">JSON</span><span class="sxs-lookup"><span data-stu-id="b7f90-155">JSON</span></span>

<span data-ttu-id="b7f90-156">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="b7f90-156">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7f90-157">使用例</span><span class="sxs-lookup"><span data-stu-id="b7f90-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="b7f90-158">CSV</span><span class="sxs-lookup"><span data-stu-id="b7f90-158">CSV</span></span>

<span data-ttu-id="b7f90-159">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="b7f90-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="b7f90-160">要求</span><span class="sxs-lookup"><span data-stu-id="b7f90-160">Request</span></span>

<span data-ttu-id="b7f90-161">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b7f90-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="b7f90-162">応答</span><span class="sxs-lookup"><span data-stu-id="b7f90-162">Response</span></span>

<span data-ttu-id="b7f90-163">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b7f90-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b7f90-164">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="b7f90-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Period
```

### <a name="json"></a><span data-ttu-id="b7f90-165">JSON</span><span class="sxs-lookup"><span data-stu-id="b7f90-165">JSON</span></span>

<span data-ttu-id="b7f90-166">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="b7f90-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="b7f90-167">要求</span><span class="sxs-lookup"><span data-stu-id="b7f90-167">Request</span></span>

<span data-ttu-id="b7f90-168">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b7f90-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="b7f90-169">応答</span><span class="sxs-lookup"><span data-stu-id="b7f90-169">Response</span></span>

<span data-ttu-id="b7f90-170">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b7f90-170">The following is an example of the response.</span></span>

> <span data-ttu-id="b7f90-p109">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b7f90-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "windows": 122, 
      "windowsPhone": 8, 
      "androidPhone": 19, 
      "iPhone": 28, 
      "iPad": 1, 
      "reportPeriod": "7"
    }
  ]
}
```