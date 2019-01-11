---
title: 'reportRoot: getEmailActivityUserCounts'
description: 送信、読み取り、受信などの電子メール アクティビティを実行しているそれぞれ別個のユーザーの数に関する傾向を把握することができます。
localization_priority: Normal
ms.openlocfilehash: de31c804bde4de615ec2c431b1fd31868723d058
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856624"
---
# <a name="reportroot-getemailactivityusercounts"></a><span data-ttu-id="267fc-103">reportRoot: getEmailActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="267fc-103">reportRoot: getEmailActivityUserCounts</span></span>

> <span data-ttu-id="267fc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="267fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="267fc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="267fc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="267fc-106">送信、読み取り、受信などの電子メール アクティビティを実行しているそれぞれ別個のユーザーの数に関する傾向を把握することができます。</span><span class="sxs-lookup"><span data-stu-id="267fc-106">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span>

> <span data-ttu-id="267fc-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: 電子メール アクティビティ](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="267fc-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="267fc-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="267fc-108">Permissions</span></span>

<span data-ttu-id="267fc-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="267fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="267fc-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="267fc-111">Permission type</span></span>                        | <span data-ttu-id="267fc-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="267fc-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="267fc-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="267fc-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="267fc-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="267fc-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="267fc-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="267fc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="267fc-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="267fc-116">Not supported.</span></span>                           |
| <span data-ttu-id="267fc-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="267fc-117">Application</span></span>                            | <span data-ttu-id="267fc-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="267fc-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="267fc-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="267fc-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="267fc-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="267fc-120">Function parameters</span></span>

<span data-ttu-id="267fc-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="267fc-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="267fc-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="267fc-122">Parameter</span></span> | <span data-ttu-id="267fc-123">Type</span><span class="sxs-lookup"><span data-stu-id="267fc-123">Type</span></span>   | <span data-ttu-id="267fc-124">説明</span><span class="sxs-lookup"><span data-stu-id="267fc-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="267fc-125">period</span><span class="sxs-lookup"><span data-stu-id="267fc-125">period</span></span>    | <span data-ttu-id="267fc-126">文字列</span><span class="sxs-lookup"><span data-stu-id="267fc-126">string</span></span> | <span data-ttu-id="267fc-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="267fc-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="267fc-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="267fc-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="267fc-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="267fc-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="267fc-130">必須。</span><span class="sxs-lookup"><span data-stu-id="267fc-130">Required.</span></span> |

<span data-ttu-id="267fc-131">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="267fc-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="267fc-132">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="267fc-132">The default output type is text/csv.</span></span> <span data-ttu-id="267fc-133">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="267fc-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="267fc-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="267fc-134">Request headers</span></span>

| <span data-ttu-id="267fc-135">名前</span><span class="sxs-lookup"><span data-stu-id="267fc-135">Name</span></span>          | <span data-ttu-id="267fc-136">説明</span><span class="sxs-lookup"><span data-stu-id="267fc-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="267fc-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="267fc-137">Authorization</span></span> | <span data-ttu-id="267fc-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="267fc-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="267fc-140">応答</span><span class="sxs-lookup"><span data-stu-id="267fc-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="267fc-141">CSV</span><span class="sxs-lookup"><span data-stu-id="267fc-141">CSV</span></span>

<span data-ttu-id="267fc-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="267fc-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="267fc-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="267fc-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="267fc-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="267fc-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="267fc-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="267fc-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="267fc-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="267fc-146">Report Refresh Date</span></span>
- <span data-ttu-id="267fc-147">送信</span><span class="sxs-lookup"><span data-stu-id="267fc-147">Send</span></span>
- <span data-ttu-id="267fc-148">受信</span><span class="sxs-lookup"><span data-stu-id="267fc-148">Receive</span></span>
- <span data-ttu-id="267fc-149">読み取り</span><span class="sxs-lookup"><span data-stu-id="267fc-149">Read</span></span>
- <span data-ttu-id="267fc-150">レポート日付</span><span class="sxs-lookup"><span data-stu-id="267fc-150">Report Date</span></span>
- <span data-ttu-id="267fc-151">レポート期間</span><span class="sxs-lookup"><span data-stu-id="267fc-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="267fc-152">JSON</span><span class="sxs-lookup"><span data-stu-id="267fc-152">JSON</span></span>

<span data-ttu-id="267fc-153">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の**[emailActivitySummary](../resources/emailactivitysummary.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="267fc-153">If successful, this method returns a `200 OK` response code and an **[emailActivitySummary](../resources/emailactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="267fc-154">例</span><span class="sxs-lookup"><span data-stu-id="267fc-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="267fc-155">CSV</span><span class="sxs-lookup"><span data-stu-id="267fc-155">CSV</span></span>

<span data-ttu-id="267fc-156">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="267fc-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="267fc-157">要求</span><span class="sxs-lookup"><span data-stu-id="267fc-157">Request</span></span>

<span data-ttu-id="267fc-158">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="267fc-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="267fc-159">応答</span><span class="sxs-lookup"><span data-stu-id="267fc-159">Response</span></span>

<span data-ttu-id="267fc-160">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="267fc-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="267fc-161">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="267fc-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Send,Receive,Read,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="267fc-162">JSON</span><span class="sxs-lookup"><span data-stu-id="267fc-162">JSON</span></span>

<span data-ttu-id="267fc-163">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="267fc-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="267fc-164">要求</span><span class="sxs-lookup"><span data-stu-id="267fc-164">Request</span></span>

<span data-ttu-id="267fc-165">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="267fc-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="267fc-166">応答</span><span class="sxs-lookup"><span data-stu-id="267fc-166">Response</span></span>

<span data-ttu-id="267fc-167">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="267fc-167">The following is an example of the response.</span></span>

> <span data-ttu-id="267fc-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="267fc-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 237

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "send": 69, 
      "receive": 197, 
      "read": 158, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
