---
title: 'reportRoot: getEmailAppUsageUserDetail'
description: メール アプリの各バージョンでユーザーが実行したアクティビティの詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5fe3bfacb247ee4435494c35c8186a89b8d80423
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639482"
---
# <a name="reportroot-getemailappusageuserdetail"></a><span data-ttu-id="62e8b-103">reportRoot: getEmailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="62e8b-103">reportRoot: getEmailAppUsageUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62e8b-104">メール アプリの各バージョンでユーザーが実行したアクティビティの詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="62e8b-104">Get details about which activities users performed on the various email apps.</span></span>

> <span data-ttu-id="62e8b-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メール アプリの使用状況](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="62e8b-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="62e8b-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="62e8b-106">Permissions</span></span>

<span data-ttu-id="62e8b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="62e8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="62e8b-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="62e8b-109">Permission type</span></span>                        | <span data-ttu-id="62e8b-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="62e8b-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="62e8b-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="62e8b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="62e8b-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="62e8b-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="62e8b-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="62e8b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62e8b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62e8b-114">Not supported.</span></span>                           |
| <span data-ttu-id="62e8b-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="62e8b-115">Application</span></span>                            | <span data-ttu-id="62e8b-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="62e8b-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="62e8b-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="62e8b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserDetail(period='{period_value}')
GET /reports/getEmailAppUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="62e8b-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="62e8b-118">Function parameters</span></span>

<span data-ttu-id="62e8b-119">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="62e8b-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="62e8b-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="62e8b-120">Parameter</span></span> | <span data-ttu-id="62e8b-121">型</span><span class="sxs-lookup"><span data-stu-id="62e8b-121">Type</span></span>   | <span data-ttu-id="62e8b-122">説明</span><span class="sxs-lookup"><span data-stu-id="62e8b-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="62e8b-123">period</span><span class="sxs-lookup"><span data-stu-id="62e8b-123">period</span></span>    | <span data-ttu-id="62e8b-124">文字列</span><span class="sxs-lookup"><span data-stu-id="62e8b-124">string</span></span> | <span data-ttu-id="62e8b-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="62e8b-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="62e8b-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="62e8b-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="62e8b-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="62e8b-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="62e8b-128">date</span><span class="sxs-lookup"><span data-stu-id="62e8b-128">date</span></span>      | <span data-ttu-id="62e8b-129">日付</span><span class="sxs-lookup"><span data-stu-id="62e8b-129">Date</span></span>   | <span data-ttu-id="62e8b-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="62e8b-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="62e8b-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="62e8b-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="62e8b-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="62e8b-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="62e8b-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="62e8b-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="62e8b-134">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="62e8b-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="62e8b-135">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="62e8b-135">The default output type is text/csv.</span></span> <span data-ttu-id="62e8b-136">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="62e8b-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="62e8b-137">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="62e8b-137">Request headers</span></span>

| <span data-ttu-id="62e8b-138">名前</span><span class="sxs-lookup"><span data-stu-id="62e8b-138">Name</span></span>          | <span data-ttu-id="62e8b-139">説明</span><span class="sxs-lookup"><span data-stu-id="62e8b-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="62e8b-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="62e8b-140">Authorization</span></span> | <span data-ttu-id="62e8b-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="62e8b-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="62e8b-143">応答</span><span class="sxs-lookup"><span data-stu-id="62e8b-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="62e8b-144">CSV</span><span class="sxs-lookup"><span data-stu-id="62e8b-144">CSV</span></span>

<span data-ttu-id="62e8b-145">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="62e8b-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="62e8b-146">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="62e8b-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="62e8b-147">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="62e8b-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="62e8b-148">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="62e8b-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="62e8b-149">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="62e8b-149">Report Refresh Date</span></span>
- <span data-ttu-id="62e8b-150">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="62e8b-150">User Principal Name</span></span>
- <span data-ttu-id="62e8b-151">表示名</span><span class="sxs-lookup"><span data-stu-id="62e8b-151">Display Name</span></span>
- <span data-ttu-id="62e8b-152">削除済み</span><span class="sxs-lookup"><span data-stu-id="62e8b-152">Is Deleted</span></span>
- <span data-ttu-id="62e8b-153">削除日</span><span class="sxs-lookup"><span data-stu-id="62e8b-153">Deleted Date</span></span>
- <span data-ttu-id="62e8b-154">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="62e8b-154">Last Activity Date</span></span>
- <span data-ttu-id="62e8b-155">Mail For Mac</span><span class="sxs-lookup"><span data-stu-id="62e8b-155">Mail For Mac</span></span>
- <span data-ttu-id="62e8b-156">Outlook For Mac</span><span class="sxs-lookup"><span data-stu-id="62e8b-156">Outlook For Mac</span></span>
- <span data-ttu-id="62e8b-157">Outlook For Windows</span><span class="sxs-lookup"><span data-stu-id="62e8b-157">Outlook For Windows</span></span>
- <span data-ttu-id="62e8b-158">Outlook For Mobile</span><span class="sxs-lookup"><span data-stu-id="62e8b-158">Outlook For Mobile</span></span>
- <span data-ttu-id="62e8b-159">Other For Mobile</span><span class="sxs-lookup"><span data-stu-id="62e8b-159">Other For Mobile</span></span>
- <span data-ttu-id="62e8b-160">Outlook For Web</span><span class="sxs-lookup"><span data-stu-id="62e8b-160">Outlook For Web</span></span>
- <span data-ttu-id="62e8b-161">POP3 アプリ</span><span class="sxs-lookup"><span data-stu-id="62e8b-161">POP3 App</span></span>
- <span data-ttu-id="62e8b-162">IMAP4 アプリ</span><span class="sxs-lookup"><span data-stu-id="62e8b-162">IMAP4 App</span></span>
- <span data-ttu-id="62e8b-163">SMTP アプリ</span><span class="sxs-lookup"><span data-stu-id="62e8b-163">SMTP App</span></span>
- <span data-ttu-id="62e8b-164">レポート期間</span><span class="sxs-lookup"><span data-stu-id="62e8b-164">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="62e8b-165">JSON</span><span class="sxs-lookup"><span data-stu-id="62e8b-165">JSON</span></span>

<span data-ttu-id="62e8b-166">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[Emailappusageuserdetail](../resources/emailappusageuserdetail.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="62e8b-166">If successful, this method returns a `200 OK` response code and an **[emailAppUsageUserDetail](../resources/emailappusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="62e8b-167">この要求の既定のページサイズは200アイテムです。</span><span class="sxs-lookup"><span data-stu-id="62e8b-167">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="62e8b-168">例</span><span class="sxs-lookup"><span data-stu-id="62e8b-168">Example</span></span>

### <a name="csv"></a><span data-ttu-id="62e8b-169">CSV</span><span class="sxs-lookup"><span data-stu-id="62e8b-169">CSV</span></span>

<span data-ttu-id="62e8b-170">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="62e8b-170">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="62e8b-171">要求</span><span class="sxs-lookup"><span data-stu-id="62e8b-171">Request</span></span>

<span data-ttu-id="62e8b-172">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="62e8b-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="62e8b-173">応答</span><span class="sxs-lookup"><span data-stu-id="62e8b-173">Response</span></span>

<span data-ttu-id="62e8b-174">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="62e8b-174">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="62e8b-175">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="62e8b-175">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="62e8b-176">Visual</span><span class="sxs-lookup"><span data-stu-id="62e8b-176">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getemailappusageuserdetail_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="62e8b-177">Java</span><span class="sxs-lookup"><span data-stu-id="62e8b-177">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getemailappusageuserdetail_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="62e8b-178">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="62e8b-178">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Period
```

### <a name="json"></a><span data-ttu-id="62e8b-179">JSON</span><span class="sxs-lookup"><span data-stu-id="62e8b-179">JSON</span></span>

<span data-ttu-id="62e8b-180">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="62e8b-180">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="62e8b-181">要求</span><span class="sxs-lookup"><span data-stu-id="62e8b-181">Request</span></span>

<span data-ttu-id="62e8b-182">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="62e8b-182">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="62e8b-183">応答</span><span class="sxs-lookup"><span data-stu-id="62e8b-183">Response</span></span>

<span data-ttu-id="62e8b-184">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="62e8b-184">The following is an example of the response.</span></span>

> <span data-ttu-id="62e8b-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="62e8b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 515

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAppUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "mailForMac": [ ], 
      "outlookForMac": [ ], 
      "outlookForWindows": [ ], 
      "outlookForMobile": [
        "Undetermined"
      ], 
      "otherForMobile": [ ], 
      "outlookForWeb": [
        "Undetermined"
      ], 
      "pop3App": [ ], 
      "imap4App": [ ], 
      "smtpApp": [ ], 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="62e8b-187">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="62e8b-187">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="62e8b-188">Visual</span><span class="sxs-lookup"><span data-stu-id="62e8b-188">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getemailappusageuserdetail_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="62e8b-189">Java</span><span class="sxs-lookup"><span data-stu-id="62e8b-189">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getemailappusageuserdetail_json-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getemailappusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getemailappusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getemailappusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getemailappusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
