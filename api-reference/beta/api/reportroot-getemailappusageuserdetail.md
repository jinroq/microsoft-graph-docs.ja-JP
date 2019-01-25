---
title: 'reportRoot: getEmailAppUsageUserDetail'
description: メール アプリの各バージョンでユーザーが実行したアクティビティの詳細を取得します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: adc34468f7dc66f2ef15e50c389e9989599c2b49
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513082"
---
# <a name="reportroot-getemailappusageuserdetail"></a><span data-ttu-id="885c7-103">reportRoot: getEmailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="885c7-103">reportRoot: getEmailAppUsageUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="885c7-104">メール アプリの各バージョンでユーザーが実行したアクティビティの詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="885c7-104">Get details about which activities users performed on the various email apps.</span></span>

> <span data-ttu-id="885c7-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メール アプリの使用状況](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="885c7-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="885c7-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="885c7-106">Permissions</span></span>

<span data-ttu-id="885c7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="885c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="885c7-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="885c7-109">Permission type</span></span>                        | <span data-ttu-id="885c7-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="885c7-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="885c7-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="885c7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="885c7-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="885c7-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="885c7-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="885c7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="885c7-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="885c7-114">Not supported.</span></span>                           |
| <span data-ttu-id="885c7-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="885c7-115">Application</span></span>                            | <span data-ttu-id="885c7-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="885c7-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="885c7-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="885c7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserDetail(period='{period_value}')
GET /reports/getEmailAppUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="885c7-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="885c7-118">Function parameters</span></span>

<span data-ttu-id="885c7-119">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="885c7-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="885c7-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="885c7-120">Parameter</span></span> | <span data-ttu-id="885c7-121">型</span><span class="sxs-lookup"><span data-stu-id="885c7-121">Type</span></span>   | <span data-ttu-id="885c7-122">説明</span><span class="sxs-lookup"><span data-stu-id="885c7-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="885c7-123">period</span><span class="sxs-lookup"><span data-stu-id="885c7-123">period</span></span>    | <span data-ttu-id="885c7-124">文字列</span><span class="sxs-lookup"><span data-stu-id="885c7-124">string</span></span> | <span data-ttu-id="885c7-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="885c7-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="885c7-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="885c7-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="885c7-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="885c7-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="885c7-128">date</span><span class="sxs-lookup"><span data-stu-id="885c7-128">date</span></span>      | <span data-ttu-id="885c7-129">日付</span><span class="sxs-lookup"><span data-stu-id="885c7-129">Date</span></span>   | <span data-ttu-id="885c7-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="885c7-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="885c7-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="885c7-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="885c7-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="885c7-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="885c7-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="885c7-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="885c7-134">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="885c7-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="885c7-135">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="885c7-135">The default output type is text/csv.</span></span> <span data-ttu-id="885c7-136">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="885c7-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="885c7-137">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="885c7-137">Request headers</span></span>

| <span data-ttu-id="885c7-138">名前</span><span class="sxs-lookup"><span data-stu-id="885c7-138">Name</span></span>          | <span data-ttu-id="885c7-139">説明</span><span class="sxs-lookup"><span data-stu-id="885c7-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="885c7-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="885c7-140">Authorization</span></span> | <span data-ttu-id="885c7-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="885c7-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="885c7-143">応答</span><span class="sxs-lookup"><span data-stu-id="885c7-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="885c7-144">CSV</span><span class="sxs-lookup"><span data-stu-id="885c7-144">CSV</span></span>

<span data-ttu-id="885c7-145">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="885c7-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="885c7-146">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="885c7-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="885c7-147">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="885c7-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="885c7-148">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="885c7-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="885c7-149">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="885c7-149">Report Refresh Date</span></span>
- <span data-ttu-id="885c7-150">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="885c7-150">User Principal Name</span></span>
- <span data-ttu-id="885c7-151">表示名</span><span class="sxs-lookup"><span data-stu-id="885c7-151">Display Name</span></span>
- <span data-ttu-id="885c7-152">削除済み</span><span class="sxs-lookup"><span data-stu-id="885c7-152">Is Deleted</span></span>
- <span data-ttu-id="885c7-153">削除日</span><span class="sxs-lookup"><span data-stu-id="885c7-153">Deleted Date</span></span>
- <span data-ttu-id="885c7-154">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="885c7-154">Last Activity Date</span></span>
- <span data-ttu-id="885c7-155">Mail For Mac</span><span class="sxs-lookup"><span data-stu-id="885c7-155">Mail For Mac</span></span>
- <span data-ttu-id="885c7-156">Outlook For Mac</span><span class="sxs-lookup"><span data-stu-id="885c7-156">Outlook For Mac</span></span>
- <span data-ttu-id="885c7-157">Outlook For Windows</span><span class="sxs-lookup"><span data-stu-id="885c7-157">Outlook For Windows</span></span>
- <span data-ttu-id="885c7-158">Outlook For Mobile</span><span class="sxs-lookup"><span data-stu-id="885c7-158">Outlook For Mobile</span></span>
- <span data-ttu-id="885c7-159">Other For Mobile</span><span class="sxs-lookup"><span data-stu-id="885c7-159">Other For Mobile</span></span>
- <span data-ttu-id="885c7-160">Outlook For Web</span><span class="sxs-lookup"><span data-stu-id="885c7-160">Outlook For Web</span></span>
- <span data-ttu-id="885c7-161">POP3 アプリ</span><span class="sxs-lookup"><span data-stu-id="885c7-161">POP3 App</span></span>
- <span data-ttu-id="885c7-162">IMAP4 アプリ</span><span class="sxs-lookup"><span data-stu-id="885c7-162">IMAP4 App</span></span>
- <span data-ttu-id="885c7-163">SMTP アプリ</span><span class="sxs-lookup"><span data-stu-id="885c7-163">SMTP App</span></span>
- <span data-ttu-id="885c7-164">レポート期間</span><span class="sxs-lookup"><span data-stu-id="885c7-164">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="885c7-165">JSON</span><span class="sxs-lookup"><span data-stu-id="885c7-165">JSON</span></span>

<span data-ttu-id="885c7-166">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の**[emailAppUsageUserDetail](../resources/emailappusageuserdetail.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="885c7-166">If successful, this method returns a `200 OK` response code and an **[emailAppUsageUserDetail](../resources/emailappusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="885c7-167">この要求の既定のページ サイズは、アイテムは 200 個です。</span><span class="sxs-lookup"><span data-stu-id="885c7-167">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="885c7-168">例</span><span class="sxs-lookup"><span data-stu-id="885c7-168">Example</span></span>

### <a name="csv"></a><span data-ttu-id="885c7-169">CSV</span><span class="sxs-lookup"><span data-stu-id="885c7-169">CSV</span></span>

<span data-ttu-id="885c7-170">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="885c7-170">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="885c7-171">要求</span><span class="sxs-lookup"><span data-stu-id="885c7-171">Request</span></span>

<span data-ttu-id="885c7-172">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="885c7-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="885c7-173">応答</span><span class="sxs-lookup"><span data-stu-id="885c7-173">Response</span></span>

<span data-ttu-id="885c7-174">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="885c7-174">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="885c7-175">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="885c7-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="885c7-176">JSON</span><span class="sxs-lookup"><span data-stu-id="885c7-176">JSON</span></span>

<span data-ttu-id="885c7-177">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="885c7-177">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="885c7-178">要求</span><span class="sxs-lookup"><span data-stu-id="885c7-178">Request</span></span>

<span data-ttu-id="885c7-179">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="885c7-179">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="885c7-180">応答</span><span class="sxs-lookup"><span data-stu-id="885c7-180">Response</span></span>

<span data-ttu-id="885c7-181">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="885c7-181">The following is an example of the response.</span></span>

> <span data-ttu-id="885c7-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="885c7-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getemailappusageuserdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
