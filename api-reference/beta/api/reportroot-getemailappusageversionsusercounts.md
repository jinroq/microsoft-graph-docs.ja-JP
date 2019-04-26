---
title: 'reportRoot: getEmailAppUsageVersionsUserCounts'
description: Outlook デスクトップ版ごとの、それぞれ別個のユーザー数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 2d6442de0f92aac5c607a77b74a7862264e2ccfd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336748"
---
# <a name="reportroot-getemailappusageversionsusercounts"></a><span data-ttu-id="39e26-103">reportRoot: getEmailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="39e26-103">reportRoot: getEmailAppUsageVersionsUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39e26-104">Outlook デスクトップ版ごとの、それぞれ別個のユーザー数を取得します。</span><span class="sxs-lookup"><span data-stu-id="39e26-104">Get the count of unique users by Outlook desktop version.</span></span>

> <span data-ttu-id="39e26-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メール アプリの使用状況](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="39e26-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="39e26-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="39e26-106">Permissions</span></span>

<span data-ttu-id="39e26-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="39e26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="39e26-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="39e26-109">Permission type</span></span>                        | <span data-ttu-id="39e26-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="39e26-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="39e26-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="39e26-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="39e26-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="39e26-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="39e26-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="39e26-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39e26-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="39e26-114">Not supported.</span></span>                           |
| <span data-ttu-id="39e26-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="39e26-115">Application</span></span>                            | <span data-ttu-id="39e26-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="39e26-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="39e26-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="39e26-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageVersionsUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="39e26-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="39e26-118">Function parameters</span></span>

<span data-ttu-id="39e26-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="39e26-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="39e26-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="39e26-120">Parameter</span></span> | <span data-ttu-id="39e26-121">型</span><span class="sxs-lookup"><span data-stu-id="39e26-121">Type</span></span>   | <span data-ttu-id="39e26-122">説明</span><span class="sxs-lookup"><span data-stu-id="39e26-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="39e26-123">period</span><span class="sxs-lookup"><span data-stu-id="39e26-123">period</span></span>    | <span data-ttu-id="39e26-124">文字列</span><span class="sxs-lookup"><span data-stu-id="39e26-124">string</span></span> | <span data-ttu-id="39e26-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="39e26-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="39e26-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="39e26-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="39e26-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="39e26-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="39e26-128">必須。</span><span class="sxs-lookup"><span data-stu-id="39e26-128">Required.</span></span> |

<span data-ttu-id="39e26-129">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="39e26-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="39e26-130">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="39e26-130">The default output type is text/csv.</span></span> <span data-ttu-id="39e26-131">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="39e26-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="39e26-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="39e26-132">Request headers</span></span>

| <span data-ttu-id="39e26-133">名前</span><span class="sxs-lookup"><span data-stu-id="39e26-133">Name</span></span>          | <span data-ttu-id="39e26-134">説明</span><span class="sxs-lookup"><span data-stu-id="39e26-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="39e26-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="39e26-135">Authorization</span></span> | <span data-ttu-id="39e26-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="39e26-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="39e26-138">応答</span><span class="sxs-lookup"><span data-stu-id="39e26-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="39e26-139">CSV</span><span class="sxs-lookup"><span data-stu-id="39e26-139">CSV</span></span>

<span data-ttu-id="39e26-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="39e26-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="39e26-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="39e26-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="39e26-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="39e26-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="39e26-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="39e26-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="39e26-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="39e26-144">Report Refresh Date</span></span>
- <span data-ttu-id="39e26-145">Outlook 2016</span><span class="sxs-lookup"><span data-stu-id="39e26-145">Outlook 2016</span></span>
- <span data-ttu-id="39e26-146">Outlook 2013</span><span class="sxs-lookup"><span data-stu-id="39e26-146">Outlook 2013</span></span>
- <span data-ttu-id="39e26-147">Outlook 2010</span><span class="sxs-lookup"><span data-stu-id="39e26-147">Outlook 2010</span></span>
- <span data-ttu-id="39e26-148">Outlook 2007</span><span class="sxs-lookup"><span data-stu-id="39e26-148">Outlook 2007</span></span>
- <span data-ttu-id="39e26-149">未定義</span><span class="sxs-lookup"><span data-stu-id="39e26-149">Undetermined</span></span>
- <span data-ttu-id="39e26-150">レポート期間</span><span class="sxs-lookup"><span data-stu-id="39e26-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="39e26-151">JSON</span><span class="sxs-lookup"><span data-stu-id="39e26-151">JSON</span></span>

<span data-ttu-id="39e26-152">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="39e26-152">If successful, this method returns a `200 OK` response code and an **[emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39e26-153">例</span><span class="sxs-lookup"><span data-stu-id="39e26-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="39e26-154">CSV</span><span class="sxs-lookup"><span data-stu-id="39e26-154">CSV</span></span>

<span data-ttu-id="39e26-155">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="39e26-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="39e26-156">要求</span><span class="sxs-lookup"><span data-stu-id="39e26-156">Request</span></span>

<span data-ttu-id="39e26-157">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="39e26-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageversionsusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageVersionsUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="39e26-158">応答</span><span class="sxs-lookup"><span data-stu-id="39e26-158">Response</span></span>

<span data-ttu-id="39e26-159">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="39e26-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="39e26-160">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="39e26-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Outlook 2016,Outlook 2013,Outlook 2010,Outlook 2007,Undetermined,Report Period
```

### <a name="json"></a><span data-ttu-id="39e26-161">JSON</span><span class="sxs-lookup"><span data-stu-id="39e26-161">JSON</span></span>

<span data-ttu-id="39e26-162">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="39e26-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="39e26-163">要求</span><span class="sxs-lookup"><span data-stu-id="39e26-163">Request</span></span>

<span data-ttu-id="39e26-164">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="39e26-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageversionsusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageVersionsUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="39e26-165">応答</span><span class="sxs-lookup"><span data-stu-id="39e26-165">Response</span></span>

<span data-ttu-id="39e26-166">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="39e26-166">The following is an example of the response.</span></span>

> <span data-ttu-id="39e26-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="39e26-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageVersionsUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAppUsageVersionsUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "outlook2016": 1554, 
      "outlook2013": 64, 
      "outlook2010": 1, 
      "outlook2007": 0, 
      "undetermined": 1259, 
      "reportPeriod": "7"
    }
  ]
}
```
