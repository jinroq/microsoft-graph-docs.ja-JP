---
title: 'reportRoot: getYammerActivityCounts'
description: 投稿、読み取り、および " いいね!" を付けられたメッセージの数によって、組織内での Yammer アクティビティの量の傾向を取得します。
localization_priority: Normal
ms.openlocfilehash: 05d6a5265bab2f4cc647b9cc7849606e6bb97a66
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817774"
---
# <a name="reportroot-getyammeractivitycounts"></a><span data-ttu-id="65e2b-103">reportRoot: getYammerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="65e2b-103">reportRoot: getYammerActivityCounts</span></span>

> <span data-ttu-id="65e2b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="65e2b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65e2b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65e2b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="65e2b-106">投稿、読み取り、および " いいね!" を付けられたメッセージの数によって、組織内での Yammer アクティビティの量の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="65e2b-106">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span>

> <span data-ttu-id="65e2b-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer アクティビティ](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65e2b-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="65e2b-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="65e2b-108">Permissions</span></span>

<span data-ttu-id="65e2b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65e2b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="65e2b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="65e2b-111">Permission type</span></span>                        | <span data-ttu-id="65e2b-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="65e2b-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="65e2b-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="65e2b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="65e2b-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="65e2b-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="65e2b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="65e2b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65e2b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65e2b-116">Not supported.</span></span>                           |
| <span data-ttu-id="65e2b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="65e2b-117">Application</span></span>                            | <span data-ttu-id="65e2b-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="65e2b-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="65e2b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="65e2b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="65e2b-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="65e2b-120">Function parameters</span></span>

<span data-ttu-id="65e2b-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="65e2b-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="65e2b-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="65e2b-122">Parameter</span></span> | <span data-ttu-id="65e2b-123">Type</span><span class="sxs-lookup"><span data-stu-id="65e2b-123">Type</span></span>   | <span data-ttu-id="65e2b-124">説明</span><span class="sxs-lookup"><span data-stu-id="65e2b-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="65e2b-125">period</span><span class="sxs-lookup"><span data-stu-id="65e2b-125">period</span></span>    | <span data-ttu-id="65e2b-126">文字列</span><span class="sxs-lookup"><span data-stu-id="65e2b-126">string</span></span> | <span data-ttu-id="65e2b-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="65e2b-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="65e2b-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="65e2b-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="65e2b-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="65e2b-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="65e2b-130">必須。</span><span class="sxs-lookup"><span data-stu-id="65e2b-130">Required.</span></span> |

<span data-ttu-id="65e2b-131">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="65e2b-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="65e2b-132">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="65e2b-132">The default output type is text/csv.</span></span> <span data-ttu-id="65e2b-133">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="65e2b-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="65e2b-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="65e2b-134">Request headers</span></span>

| <span data-ttu-id="65e2b-135">名前</span><span class="sxs-lookup"><span data-stu-id="65e2b-135">Name</span></span>          | <span data-ttu-id="65e2b-136">説明</span><span class="sxs-lookup"><span data-stu-id="65e2b-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="65e2b-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="65e2b-137">Authorization</span></span> | <span data-ttu-id="65e2b-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="65e2b-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="65e2b-140">応答</span><span class="sxs-lookup"><span data-stu-id="65e2b-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="65e2b-141">CSV</span><span class="sxs-lookup"><span data-stu-id="65e2b-141">CSV</span></span>

<span data-ttu-id="65e2b-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="65e2b-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="65e2b-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="65e2b-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="65e2b-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="65e2b-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="65e2b-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="65e2b-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="65e2b-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="65e2b-146">Report Refresh Date</span></span>
- <span data-ttu-id="65e2b-147">いいね!</span><span class="sxs-lookup"><span data-stu-id="65e2b-147">Liked</span></span>
- <span data-ttu-id="65e2b-148">投稿</span><span class="sxs-lookup"><span data-stu-id="65e2b-148">Posted</span></span>
- <span data-ttu-id="65e2b-149">読み取り</span><span class="sxs-lookup"><span data-stu-id="65e2b-149">Read</span></span>
- <span data-ttu-id="65e2b-150">レポート日付</span><span class="sxs-lookup"><span data-stu-id="65e2b-150">Report Date</span></span>
- <span data-ttu-id="65e2b-151">レポート期間</span><span class="sxs-lookup"><span data-stu-id="65e2b-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="65e2b-152">JSON</span><span class="sxs-lookup"><span data-stu-id="65e2b-152">JSON</span></span>

<span data-ttu-id="65e2b-153">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[yammerActivitySummary](../resources/yammeractivitysummary.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="65e2b-153">If successful, this method returns a `200 OK` response code and a **[yammerActivitySummary](../resources/yammeractivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65e2b-154">例</span><span class="sxs-lookup"><span data-stu-id="65e2b-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="65e2b-155">CSV</span><span class="sxs-lookup"><span data-stu-id="65e2b-155">CSV</span></span>

<span data-ttu-id="65e2b-156">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="65e2b-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="65e2b-157">要求</span><span class="sxs-lookup"><span data-stu-id="65e2b-157">Request</span></span>

<span data-ttu-id="65e2b-158">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="65e2b-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="65e2b-159">応答</span><span class="sxs-lookup"><span data-stu-id="65e2b-159">Response</span></span>

<span data-ttu-id="65e2b-160">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="65e2b-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="65e2b-161">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="65e2b-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="65e2b-162">JSON</span><span class="sxs-lookup"><span data-stu-id="65e2b-162">JSON</span></span>

<span data-ttu-id="65e2b-163">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="65e2b-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="65e2b-164">要求</span><span class="sxs-lookup"><span data-stu-id="65e2b-164">Request</span></span>

<span data-ttu-id="65e2b-165">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="65e2b-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="65e2b-166">応答</span><span class="sxs-lookup"><span data-stu-id="65e2b-166">Response</span></span>

<span data-ttu-id="65e2b-167">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="65e2b-167">The following is an example of the response.</span></span>

> <span data-ttu-id="65e2b-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="65e2b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 237

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "liked": 47, 
      "posted": 59, 
      "read": 986, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
