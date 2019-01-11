---
title: 'reportRoot: getEmailAppUsageAppsUserCounts'
description: メール アプリごとの、それぞれ別個のユーザーの数を取得します。
localization_priority: Normal
ms.openlocfilehash: 7aab9765092218c5f0555ec84099c826ae29fa94
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826958"
---
# <a name="reportroot-getemailappusageappsusercounts"></a><span data-ttu-id="6b8ed-103">reportRoot: getEmailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="6b8ed-103">reportRoot: getEmailAppUsageAppsUserCounts</span></span>

> <span data-ttu-id="6b8ed-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6b8ed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b8ed-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b8ed-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6b8ed-106">メール アプリごとの、それぞれ別個のユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="6b8ed-106">Get the count of unique users per email app.</span></span>

> <span data-ttu-id="6b8ed-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メール アプリの使用状況](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6b8ed-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="6b8ed-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6b8ed-108">Permissions</span></span>

<span data-ttu-id="6b8ed-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6b8ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6b8ed-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6b8ed-111">Permission type</span></span>                        | <span data-ttu-id="6b8ed-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6b8ed-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6b8ed-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="6b8ed-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="6b8ed-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b8ed-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6b8ed-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6b8ed-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b8ed-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b8ed-116">Not supported.</span></span>                           |
| <span data-ttu-id="6b8ed-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6b8ed-117">Application</span></span>                            | <span data-ttu-id="6b8ed-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b8ed-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6b8ed-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6b8ed-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageAppsUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="6b8ed-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="6b8ed-120">Function parameters</span></span>

<span data-ttu-id="6b8ed-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="6b8ed-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="6b8ed-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="6b8ed-122">Parameter</span></span> | <span data-ttu-id="6b8ed-123">Type</span><span class="sxs-lookup"><span data-stu-id="6b8ed-123">Type</span></span>   | <span data-ttu-id="6b8ed-124">説明</span><span class="sxs-lookup"><span data-stu-id="6b8ed-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6b8ed-125">period</span><span class="sxs-lookup"><span data-stu-id="6b8ed-125">period</span></span>    | <span data-ttu-id="6b8ed-126">文字列</span><span class="sxs-lookup"><span data-stu-id="6b8ed-126">string</span></span> | <span data-ttu-id="6b8ed-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="6b8ed-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6b8ed-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="6b8ed-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6b8ed-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="6b8ed-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="6b8ed-130">必須。</span><span class="sxs-lookup"><span data-stu-id="6b8ed-130">Required.</span></span> |

<span data-ttu-id="6b8ed-131">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="6b8ed-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="6b8ed-132">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="6b8ed-132">The default output type is text/csv.</span></span> <span data-ttu-id="6b8ed-133">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="6b8ed-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6b8ed-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6b8ed-134">Request headers</span></span>

| <span data-ttu-id="6b8ed-135">名前</span><span class="sxs-lookup"><span data-stu-id="6b8ed-135">Name</span></span>          | <span data-ttu-id="6b8ed-136">説明</span><span class="sxs-lookup"><span data-stu-id="6b8ed-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="6b8ed-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b8ed-137">Authorization</span></span> | <span data-ttu-id="6b8ed-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6b8ed-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6b8ed-140">応答</span><span class="sxs-lookup"><span data-stu-id="6b8ed-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="6b8ed-141">CSV</span><span class="sxs-lookup"><span data-stu-id="6b8ed-141">CSV</span></span>

<span data-ttu-id="6b8ed-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="6b8ed-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6b8ed-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="6b8ed-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6b8ed-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="6b8ed-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6b8ed-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="6b8ed-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6b8ed-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="6b8ed-146">Report Refresh Date</span></span>
- <span data-ttu-id="6b8ed-147">Mail For Mac</span><span class="sxs-lookup"><span data-stu-id="6b8ed-147">Mail For Mac</span></span>
- <span data-ttu-id="6b8ed-148">Outlook For Mac</span><span class="sxs-lookup"><span data-stu-id="6b8ed-148">Outlook For Mac</span></span>
- <span data-ttu-id="6b8ed-149">Outlook For Windows</span><span class="sxs-lookup"><span data-stu-id="6b8ed-149">Outlook For Windows</span></span>
- <span data-ttu-id="6b8ed-150">Outlook For Mobile</span><span class="sxs-lookup"><span data-stu-id="6b8ed-150">Outlook For Mobile</span></span>
- <span data-ttu-id="6b8ed-151">Other For Mobile</span><span class="sxs-lookup"><span data-stu-id="6b8ed-151">Other For Mobile</span></span>
- <span data-ttu-id="6b8ed-152">Outlook For Web</span><span class="sxs-lookup"><span data-stu-id="6b8ed-152">Outlook For Web</span></span>
- <span data-ttu-id="6b8ed-153">POP3 アプリ</span><span class="sxs-lookup"><span data-stu-id="6b8ed-153">POP3 App</span></span>
- <span data-ttu-id="6b8ed-154">IMAP4 アプリ</span><span class="sxs-lookup"><span data-stu-id="6b8ed-154">IMAP4 App</span></span>
- <span data-ttu-id="6b8ed-155">SMTP アプリ</span><span class="sxs-lookup"><span data-stu-id="6b8ed-155">SMTP App</span></span>
- <span data-ttu-id="6b8ed-156">レポート期間</span><span class="sxs-lookup"><span data-stu-id="6b8ed-156">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="6b8ed-157">JSON</span><span class="sxs-lookup"><span data-stu-id="6b8ed-157">JSON</span></span>

<span data-ttu-id="6b8ed-158">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の**[emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="6b8ed-158">If successful, this method returns a `200 OK` response code and an **[emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b8ed-159">例</span><span class="sxs-lookup"><span data-stu-id="6b8ed-159">Example</span></span>

### <a name="csv"></a><span data-ttu-id="6b8ed-160">CSV</span><span class="sxs-lookup"><span data-stu-id="6b8ed-160">CSV</span></span>

<span data-ttu-id="6b8ed-161">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="6b8ed-161">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="6b8ed-162">要求</span><span class="sxs-lookup"><span data-stu-id="6b8ed-162">Request</span></span>

<span data-ttu-id="6b8ed-163">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6b8ed-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageappsusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageAppsUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="6b8ed-164">応答</span><span class="sxs-lookup"><span data-stu-id="6b8ed-164">Response</span></span>

<span data-ttu-id="6b8ed-165">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6b8ed-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="6b8ed-166">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="6b8ed-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Period
```

### <a name="json"></a><span data-ttu-id="6b8ed-167">JSON</span><span class="sxs-lookup"><span data-stu-id="6b8ed-167">JSON</span></span>

<span data-ttu-id="6b8ed-168">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="6b8ed-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="6b8ed-169">要求</span><span class="sxs-lookup"><span data-stu-id="6b8ed-169">Request</span></span>

<span data-ttu-id="6b8ed-170">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6b8ed-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageappsusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageAppsUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="6b8ed-171">応答</span><span class="sxs-lookup"><span data-stu-id="6b8ed-171">Response</span></span>

<span data-ttu-id="6b8ed-172">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6b8ed-172">The following is an example of the response.</span></span>

> <span data-ttu-id="6b8ed-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6b8ed-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageAppsUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 345

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAppUsageAppsUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "mailForMac": 4, 
      "outlookForMac": 105, 
      "outlookForWindows": 1589, 
      "outlookForMobile": 1116, 
      "otherForMobile": 485, 
      "outlookForWeb": 753, 
      "pop3App": 0, 
      "imap4App": 0, 
      "smtpApp": 0, 
      "reportPeriod": "7"
    }
  ]
}
```
