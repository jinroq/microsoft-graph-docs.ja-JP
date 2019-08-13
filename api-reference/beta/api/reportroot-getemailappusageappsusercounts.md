---
title: 'reportRoot: getEmailAppUsageAppsUserCounts'
description: メール アプリごとの、それぞれ別個のユーザーの数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 59d6b6943957983ed852675687c7a72b61d2caa5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308624"
---
# <a name="reportroot-getemailappusageappsusercounts"></a><span data-ttu-id="dcd33-103">reportRoot: getEmailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="dcd33-103">reportRoot: getEmailAppUsageAppsUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcd33-104">メール アプリごとの、それぞれ別個のユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="dcd33-104">Get the count of unique users per email app.</span></span>

> <span data-ttu-id="dcd33-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メール アプリの使用状況](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dcd33-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="dcd33-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dcd33-106">Permissions</span></span>

<span data-ttu-id="dcd33-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dcd33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dcd33-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dcd33-109">Permission type</span></span>                        | <span data-ttu-id="dcd33-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dcd33-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="dcd33-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="dcd33-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dcd33-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dcd33-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="dcd33-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dcd33-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcd33-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dcd33-114">Not supported.</span></span>                           |
| <span data-ttu-id="dcd33-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dcd33-115">Application</span></span>                            | <span data-ttu-id="dcd33-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dcd33-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="dcd33-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dcd33-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageAppsUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="dcd33-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="dcd33-118">Function parameters</span></span>

<span data-ttu-id="dcd33-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="dcd33-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="dcd33-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="dcd33-120">Parameter</span></span> | <span data-ttu-id="dcd33-121">型</span><span class="sxs-lookup"><span data-stu-id="dcd33-121">Type</span></span>   | <span data-ttu-id="dcd33-122">説明</span><span class="sxs-lookup"><span data-stu-id="dcd33-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="dcd33-123">period</span><span class="sxs-lookup"><span data-stu-id="dcd33-123">period</span></span>    | <span data-ttu-id="dcd33-124">文字列</span><span class="sxs-lookup"><span data-stu-id="dcd33-124">string</span></span> | <span data-ttu-id="dcd33-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="dcd33-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="dcd33-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="dcd33-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="dcd33-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="dcd33-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="dcd33-128">必須。</span><span class="sxs-lookup"><span data-stu-id="dcd33-128">Required.</span></span> |

<span data-ttu-id="dcd33-129">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="dcd33-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="dcd33-130">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="dcd33-130">The default output type is text/csv.</span></span> <span data-ttu-id="dcd33-131">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="dcd33-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dcd33-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dcd33-132">Request headers</span></span>

| <span data-ttu-id="dcd33-133">名前</span><span class="sxs-lookup"><span data-stu-id="dcd33-133">Name</span></span>          | <span data-ttu-id="dcd33-134">説明</span><span class="sxs-lookup"><span data-stu-id="dcd33-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="dcd33-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="dcd33-135">Authorization</span></span> | <span data-ttu-id="dcd33-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="dcd33-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="dcd33-138">応答</span><span class="sxs-lookup"><span data-stu-id="dcd33-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="dcd33-139">CSV</span><span class="sxs-lookup"><span data-stu-id="dcd33-139">CSV</span></span>

<span data-ttu-id="dcd33-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="dcd33-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="dcd33-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="dcd33-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="dcd33-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="dcd33-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="dcd33-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="dcd33-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="dcd33-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="dcd33-144">Report Refresh Date</span></span>
- <span data-ttu-id="dcd33-145">Mail For Mac</span><span class="sxs-lookup"><span data-stu-id="dcd33-145">Mail For Mac</span></span>
- <span data-ttu-id="dcd33-146">Outlook For Mac</span><span class="sxs-lookup"><span data-stu-id="dcd33-146">Outlook For Mac</span></span>
- <span data-ttu-id="dcd33-147">Outlook For Windows</span><span class="sxs-lookup"><span data-stu-id="dcd33-147">Outlook For Windows</span></span>
- <span data-ttu-id="dcd33-148">Outlook For Mobile</span><span class="sxs-lookup"><span data-stu-id="dcd33-148">Outlook For Mobile</span></span>
- <span data-ttu-id="dcd33-149">Other For Mobile</span><span class="sxs-lookup"><span data-stu-id="dcd33-149">Other For Mobile</span></span>
- <span data-ttu-id="dcd33-150">Outlook For Web</span><span class="sxs-lookup"><span data-stu-id="dcd33-150">Outlook For Web</span></span>
- <span data-ttu-id="dcd33-151">POP3 アプリ</span><span class="sxs-lookup"><span data-stu-id="dcd33-151">POP3 App</span></span>
- <span data-ttu-id="dcd33-152">IMAP4 アプリ</span><span class="sxs-lookup"><span data-stu-id="dcd33-152">IMAP4 App</span></span>
- <span data-ttu-id="dcd33-153">SMTP アプリ</span><span class="sxs-lookup"><span data-stu-id="dcd33-153">SMTP App</span></span>
- <span data-ttu-id="dcd33-154">レポート期間</span><span class="sxs-lookup"><span data-stu-id="dcd33-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="dcd33-155">JSON</span><span class="sxs-lookup"><span data-stu-id="dcd33-155">JSON</span></span>

<span data-ttu-id="dcd33-156">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[Emailappusageappsusercounts](../resources/emailappusageappsusercounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dcd33-156">If successful, this method returns a `200 OK` response code and an **[emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcd33-157">例</span><span class="sxs-lookup"><span data-stu-id="dcd33-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="dcd33-158">CSV</span><span class="sxs-lookup"><span data-stu-id="dcd33-158">CSV</span></span>

<span data-ttu-id="dcd33-159">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dcd33-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="dcd33-160">要求</span><span class="sxs-lookup"><span data-stu-id="dcd33-160">Request</span></span>

<span data-ttu-id="dcd33-161">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dcd33-161">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dcd33-162">プロトコル</span><span class="sxs-lookup"><span data-stu-id="dcd33-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageappsusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageAppsUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dcd33-163">C#</span><span class="sxs-lookup"><span data-stu-id="dcd33-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageappsusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dcd33-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dcd33-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageappsusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dcd33-165">目的-C</span><span class="sxs-lookup"><span data-stu-id="dcd33-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageappsusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dcd33-166">Java</span><span class="sxs-lookup"><span data-stu-id="dcd33-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getemailappusageappsusercounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dcd33-167">応答</span><span class="sxs-lookup"><span data-stu-id="dcd33-167">Response</span></span>

<span data-ttu-id="dcd33-168">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dcd33-168">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="dcd33-169">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="dcd33-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="dcd33-170">JSON</span><span class="sxs-lookup"><span data-stu-id="dcd33-170">JSON</span></span>

<span data-ttu-id="dcd33-171">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="dcd33-171">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="dcd33-172">要求</span><span class="sxs-lookup"><span data-stu-id="dcd33-172">Request</span></span>

<span data-ttu-id="dcd33-173">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dcd33-173">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dcd33-174">プロトコル</span><span class="sxs-lookup"><span data-stu-id="dcd33-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageappsusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageAppsUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dcd33-175">C#</span><span class="sxs-lookup"><span data-stu-id="dcd33-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageappsusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dcd33-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dcd33-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageappsusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dcd33-177">目的-C</span><span class="sxs-lookup"><span data-stu-id="dcd33-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageappsusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dcd33-178">Java</span><span class="sxs-lookup"><span data-stu-id="dcd33-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getemailappusageappsusercounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dcd33-179">応答</span><span class="sxs-lookup"><span data-stu-id="dcd33-179">Response</span></span>

<span data-ttu-id="dcd33-180">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dcd33-180">The following is an example of the response.</span></span>

> <span data-ttu-id="dcd33-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="dcd33-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
