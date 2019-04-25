---
title: 'reportRoot: getEmailAppUsageUserCounts'
description: 任意のメール アプリを使用して Exchange Online に接続されている、それぞれ別個のユーザー数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 4887910d6b0bdc1474be83ad0fc146a41051e396
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546089"
---
# <a name="reportroot-getemailappusageusercounts"></a><span data-ttu-id="8bdca-103">reportRoot: getEmailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="8bdca-103">reportRoot: getEmailAppUsageUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bdca-104">任意のメール アプリを使用して Exchange Online に接続されている、それぞれ別個のユーザー数を取得します。</span><span class="sxs-lookup"><span data-stu-id="8bdca-104">Get the count of unique users that connected to Exchange Online using any email app.</span></span>

> <span data-ttu-id="8bdca-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メール アプリの使用状況](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8bdca-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="8bdca-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8bdca-106">Permissions</span></span>

<span data-ttu-id="8bdca-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8bdca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8bdca-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8bdca-109">Permission type</span></span>                        | <span data-ttu-id="8bdca-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8bdca-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8bdca-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8bdca-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8bdca-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bdca-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8bdca-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8bdca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bdca-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8bdca-114">Not supported.</span></span>                           |
| <span data-ttu-id="8bdca-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8bdca-115">Application</span></span>                            | <span data-ttu-id="8bdca-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bdca-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8bdca-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8bdca-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="8bdca-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="8bdca-118">Function parameters</span></span>

<span data-ttu-id="8bdca-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="8bdca-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="8bdca-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="8bdca-120">Parameter</span></span> | <span data-ttu-id="8bdca-121">型</span><span class="sxs-lookup"><span data-stu-id="8bdca-121">Type</span></span>   | <span data-ttu-id="8bdca-122">説明</span><span class="sxs-lookup"><span data-stu-id="8bdca-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8bdca-123">period</span><span class="sxs-lookup"><span data-stu-id="8bdca-123">period</span></span>    | <span data-ttu-id="8bdca-124">文字列</span><span class="sxs-lookup"><span data-stu-id="8bdca-124">string</span></span> | <span data-ttu-id="8bdca-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="8bdca-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8bdca-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="8bdca-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8bdca-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="8bdca-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="8bdca-128">必須。</span><span class="sxs-lookup"><span data-stu-id="8bdca-128">Required.</span></span> |

<span data-ttu-id="8bdca-129">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8bdca-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="8bdca-130">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="8bdca-130">The default output type is text/csv.</span></span> <span data-ttu-id="8bdca-131">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="8bdca-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8bdca-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8bdca-132">Request headers</span></span>

| <span data-ttu-id="8bdca-133">名前</span><span class="sxs-lookup"><span data-stu-id="8bdca-133">Name</span></span>          | <span data-ttu-id="8bdca-134">説明</span><span class="sxs-lookup"><span data-stu-id="8bdca-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8bdca-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="8bdca-135">Authorization</span></span> | <span data-ttu-id="8bdca-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8bdca-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8bdca-138">応答</span><span class="sxs-lookup"><span data-stu-id="8bdca-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="8bdca-139">CSV</span><span class="sxs-lookup"><span data-stu-id="8bdca-139">CSV</span></span>

<span data-ttu-id="8bdca-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="8bdca-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8bdca-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="8bdca-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8bdca-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="8bdca-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8bdca-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="8bdca-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8bdca-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="8bdca-144">Report Refresh Date</span></span>
- <span data-ttu-id="8bdca-145">Mail For Mac</span><span class="sxs-lookup"><span data-stu-id="8bdca-145">Mail For Mac</span></span>
- <span data-ttu-id="8bdca-146">Outlook For Mac</span><span class="sxs-lookup"><span data-stu-id="8bdca-146">Outlook For Mac</span></span>
- <span data-ttu-id="8bdca-147">Outlook For Windows</span><span class="sxs-lookup"><span data-stu-id="8bdca-147">Outlook For Windows</span></span>
- <span data-ttu-id="8bdca-148">Outlook For Mobile</span><span class="sxs-lookup"><span data-stu-id="8bdca-148">Outlook For Mobile</span></span>
- <span data-ttu-id="8bdca-149">Other For Mobile</span><span class="sxs-lookup"><span data-stu-id="8bdca-149">Other For Mobile</span></span>
- <span data-ttu-id="8bdca-150">Outlook For Web</span><span class="sxs-lookup"><span data-stu-id="8bdca-150">Outlook For Web</span></span>
- <span data-ttu-id="8bdca-151">POP3 アプリ</span><span class="sxs-lookup"><span data-stu-id="8bdca-151">POP3 App</span></span>
- <span data-ttu-id="8bdca-152">IMAP4 アプリ</span><span class="sxs-lookup"><span data-stu-id="8bdca-152">IMAP4 App</span></span>
- <span data-ttu-id="8bdca-153">SMTP アプリ</span><span class="sxs-lookup"><span data-stu-id="8bdca-153">SMTP App</span></span>
- <span data-ttu-id="8bdca-154">レポート日付</span><span class="sxs-lookup"><span data-stu-id="8bdca-154">Report Date</span></span>
- <span data-ttu-id="8bdca-155">レポート期間</span><span class="sxs-lookup"><span data-stu-id="8bdca-155">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="8bdca-156">JSON</span><span class="sxs-lookup"><span data-stu-id="8bdca-156">JSON</span></span>

<span data-ttu-id="8bdca-157">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[emailappusageusercounts](../resources/emailappusageusercounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8bdca-157">If successful, this method returns a `200 OK` response code and an **[emailAppUsageUserCounts](../resources/emailappusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bdca-158">例</span><span class="sxs-lookup"><span data-stu-id="8bdca-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="8bdca-159">CSV</span><span class="sxs-lookup"><span data-stu-id="8bdca-159">CSV</span></span>

<span data-ttu-id="8bdca-160">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8bdca-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="8bdca-161">要求</span><span class="sxs-lookup"><span data-stu-id="8bdca-161">Request</span></span>

<span data-ttu-id="8bdca-162">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8bdca-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="8bdca-163">応答</span><span class="sxs-lookup"><span data-stu-id="8bdca-163">Response</span></span>

<span data-ttu-id="8bdca-164">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8bdca-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="8bdca-165">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="8bdca-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="8bdca-166">JSON</span><span class="sxs-lookup"><span data-stu-id="8bdca-166">JSON</span></span>

<span data-ttu-id="8bdca-167">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="8bdca-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="8bdca-168">要求</span><span class="sxs-lookup"><span data-stu-id="8bdca-168">Request</span></span>

<span data-ttu-id="8bdca-169">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8bdca-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="8bdca-170">応答</span><span class="sxs-lookup"><span data-stu-id="8bdca-170">Response</span></span>

<span data-ttu-id="8bdca-171">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8bdca-171">The following is an example of the response.</span></span>

> <span data-ttu-id="8bdca-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8bdca-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAppUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "mailForMac": 0, 
      "outlookForMac": 0, 
      "outlookForWindows": 0, 
      "outlookForMobile": 0, 
      "otherForMobile": 0, 
      "outlookForWeb": 0, 
      "pop3App": 0, 
      "imap4App": 0, 
      "smtpApp": 0, 
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
    "Error: /api-reference/beta/api/reportroot-getemailappusageusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
