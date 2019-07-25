---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: ユーザーごとに、Microsoft Teams デバイスの使用状況の詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: f0606b14c23063e3784818529b7a5f7e47d05cdb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871776"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="7febc-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="7febc-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7febc-104">ユーザーごとに、Microsoft Teams デバイスの使用状況の詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="7febc-104">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="7febc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7febc-105">Permissions</span></span>

<span data-ttu-id="7febc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7febc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7febc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7febc-108">Permission type</span></span>                        | <span data-ttu-id="7febc-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7febc-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7febc-110">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="7febc-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7febc-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7febc-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7febc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7febc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7febc-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7febc-113">Not supported.</span></span>                           |
| <span data-ttu-id="7febc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7febc-114">Application</span></span>                            | <span data-ttu-id="7febc-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7febc-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7febc-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7febc-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='D7')
GET /reports/getTeamsDeviceUsageUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="7febc-117">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="7febc-117">Function parameters</span></span>

<span data-ttu-id="7febc-118">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="7febc-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="7febc-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="7febc-119">Parameter</span></span> | <span data-ttu-id="7febc-120">型</span><span class="sxs-lookup"><span data-stu-id="7febc-120">Type</span></span>   | <span data-ttu-id="7febc-121">説明</span><span class="sxs-lookup"><span data-stu-id="7febc-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7febc-122">period</span><span class="sxs-lookup"><span data-stu-id="7febc-122">period</span></span>    | <span data-ttu-id="7febc-123">文字列</span><span class="sxs-lookup"><span data-stu-id="7febc-123">string</span></span> | <span data-ttu-id="7febc-124">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="7febc-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7febc-125">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="7febc-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7febc-126">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="7febc-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="7febc-127">date</span><span class="sxs-lookup"><span data-stu-id="7febc-127">date</span></span>      | <span data-ttu-id="7febc-128">日付</span><span class="sxs-lookup"><span data-stu-id="7febc-128">Date</span></span>   | <span data-ttu-id="7febc-129">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="7febc-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="7febc-130">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="7febc-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="7febc-131">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="7febc-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="7febc-132">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7febc-132">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="7febc-133">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7febc-133">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="7febc-134">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="7febc-134">The default output type is text/csv.</span></span> <span data-ttu-id="7febc-135">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="7febc-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7febc-136">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7febc-136">Request headers</span></span>

| <span data-ttu-id="7febc-137">名前</span><span class="sxs-lookup"><span data-stu-id="7febc-137">Name</span></span>          | <span data-ttu-id="7febc-138">説明</span><span class="sxs-lookup"><span data-stu-id="7febc-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7febc-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="7febc-139">Authorization</span></span> | <span data-ttu-id="7febc-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7febc-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7febc-142">応答</span><span class="sxs-lookup"><span data-stu-id="7febc-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="7febc-143">CSV</span><span class="sxs-lookup"><span data-stu-id="7febc-143">CSV</span></span>

<span data-ttu-id="7febc-144">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="7febc-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7febc-145">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="7febc-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7febc-146">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="7febc-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7febc-147">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="7febc-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7febc-148">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="7febc-148">Report Refresh Date</span></span>
- <span data-ttu-id="7febc-149">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="7febc-149">User Principal Name</span></span>
- <span data-ttu-id="7febc-150">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="7febc-150">Last Activity Date</span></span>
- <span data-ttu-id="7febc-151">削除済み</span><span class="sxs-lookup"><span data-stu-id="7febc-151">Is Deleted</span></span>
- <span data-ttu-id="7febc-152">削除日</span><span class="sxs-lookup"><span data-stu-id="7febc-152">Deleted Date</span></span>
- <span data-ttu-id="7febc-153">Web の使用</span><span class="sxs-lookup"><span data-stu-id="7febc-153">Used Web</span></span>
- <span data-ttu-id="7febc-154">Windows スマートフォンの使用</span><span class="sxs-lookup"><span data-stu-id="7febc-154">Used Windows Phone</span></span>
- <span data-ttu-id="7febc-155">iOS の使用</span><span class="sxs-lookup"><span data-stu-id="7febc-155">Used iOS</span></span>
- <span data-ttu-id="7febc-156">Mac の使用</span><span class="sxs-lookup"><span data-stu-id="7febc-156">Used Mac</span></span>
- <span data-ttu-id="7febc-157">Android スマートフォンの使用</span><span class="sxs-lookup"><span data-stu-id="7febc-157">Used Android Phone</span></span>
- <span data-ttu-id="7febc-158">Windows の使用</span><span class="sxs-lookup"><span data-stu-id="7febc-158">Used Windows</span></span>
- <span data-ttu-id="7febc-159">レポート期間</span><span class="sxs-lookup"><span data-stu-id="7febc-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="7febc-160">JSON</span><span class="sxs-lookup"><span data-stu-id="7febc-160">JSON</span></span>

<span data-ttu-id="7febc-161">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[teamsdevice使い方 userdetail](../resources/teamsdeviceusageuserdetail.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7febc-161">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="7febc-162">この要求の既定のページサイズは2000アイテムです。</span><span class="sxs-lookup"><span data-stu-id="7febc-162">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="7febc-163">例</span><span class="sxs-lookup"><span data-stu-id="7febc-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="7febc-164">CSV</span><span class="sxs-lookup"><span data-stu-id="7febc-164">CSV</span></span>

<span data-ttu-id="7febc-165">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7febc-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="7febc-166">要求</span><span class="sxs-lookup"><span data-stu-id="7febc-166">Request</span></span>

<span data-ttu-id="7febc-167">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7febc-167">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7febc-168">プロトコル</span><span class="sxs-lookup"><span data-stu-id="7febc-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7febc-169">C#</span><span class="sxs-lookup"><span data-stu-id="7febc-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7febc-170">Javascript</span><span class="sxs-lookup"><span data-stu-id="7febc-170">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7febc-171">目的-C</span><span class="sxs-lookup"><span data-stu-id="7febc-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7febc-172">Java</span><span class="sxs-lookup"><span data-stu-id="7febc-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsdeviceusageuserdetail-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7febc-173">応答</span><span class="sxs-lookup"><span data-stu-id="7febc-173">Response</span></span>

<span data-ttu-id="7febc-174">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7febc-174">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7febc-175">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="7febc-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Used Web,Used Windows Phone,Used iOS,Used Mac,Used Android Phone,Used Windows,Report Period
```

### <a name="json"></a><span data-ttu-id="7febc-176">JSON</span><span class="sxs-lookup"><span data-stu-id="7febc-176">JSON</span></span>

<span data-ttu-id="7febc-177">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="7febc-177">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="7febc-178">要求</span><span class="sxs-lookup"><span data-stu-id="7febc-178">Request</span></span>

<span data-ttu-id="7febc-179">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7febc-179">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7febc-180">プロトコル</span><span class="sxs-lookup"><span data-stu-id="7febc-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7febc-181">C#</span><span class="sxs-lookup"><span data-stu-id="7febc-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7febc-182">Javascript</span><span class="sxs-lookup"><span data-stu-id="7febc-182">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7febc-183">目的-C</span><span class="sxs-lookup"><span data-stu-id="7febc-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7febc-184">Java</span><span class="sxs-lookup"><span data-stu-id="7febc-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsdeviceusageuserdetail-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7febc-185">応答</span><span class="sxs-lookup"><span data-stu-id="7febc-185">Response</span></span>

<span data-ttu-id="7febc-186">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7febc-186">The following is an example of the response.</span></span>

> <span data-ttu-id="7febc-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7febc-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 374

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "lastActivityDate": "2017-09-01", 
      "isDeleted": false, 
      "deletedDate": null, 
      "usedWeb": false, 
      "usedWindowsPhone": false, 
      "usediOS": true, 
      "usedMac": false, 
      "usedAndroidPhone": false, 
      "usedWindows": true, 
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
