---
title: 'reportRoot: getOneDriveActivityUserDetail'
description: ユーザー別の OneDrive アクティビティに関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: fc5d8e6374b7708932d46e1f6ef63e466c205164
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36411572"
---
# <a name="reportroot-getonedriveactivityuserdetail"></a><span data-ttu-id="7c2ee-103">reportRoot: getOneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="7c2ee-103">reportRoot: getOneDriveActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c2ee-104">ユーザー別の OneDrive アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-104">Get details about OneDrive activity by user.</span></span>

> <span data-ttu-id="7c2ee-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business のアクティビティ](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="7c2ee-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7c2ee-106">Permissions</span></span>

<span data-ttu-id="7c2ee-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7c2ee-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7c2ee-109">Permission type</span></span>                        | <span data-ttu-id="7c2ee-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7c2ee-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7c2ee-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="7c2ee-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7c2ee-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c2ee-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7c2ee-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7c2ee-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c2ee-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-114">Not supported.</span></span>                           |
| <span data-ttu-id="7c2ee-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7c2ee-115">Application</span></span>                            | <span data-ttu-id="7c2ee-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c2ee-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7c2ee-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7c2ee-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityUserDetail(period='{period_value}')
GET /reports/getOneDriveActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="7c2ee-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="7c2ee-118">Function parameters</span></span>

<span data-ttu-id="7c2ee-119">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="7c2ee-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="7c2ee-120">Parameter</span></span> | <span data-ttu-id="7c2ee-121">型</span><span class="sxs-lookup"><span data-stu-id="7c2ee-121">Type</span></span>   | <span data-ttu-id="7c2ee-122">説明</span><span class="sxs-lookup"><span data-stu-id="7c2ee-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7c2ee-123">period</span><span class="sxs-lookup"><span data-stu-id="7c2ee-123">period</span></span>    | <span data-ttu-id="7c2ee-124">文字列</span><span class="sxs-lookup"><span data-stu-id="7c2ee-124">string</span></span> | <span data-ttu-id="7c2ee-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7c2ee-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7c2ee-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="7c2ee-128">date</span><span class="sxs-lookup"><span data-stu-id="7c2ee-128">date</span></span>      | <span data-ttu-id="7c2ee-129">日付</span><span class="sxs-lookup"><span data-stu-id="7c2ee-129">Date</span></span>   | <span data-ttu-id="7c2ee-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="7c2ee-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="7c2ee-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="7c2ee-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="7c2ee-134">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="7c2ee-135">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-135">The default output type is text/csv.</span></span> <span data-ttu-id="7c2ee-136">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c2ee-137">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c2ee-137">Request headers</span></span>

| <span data-ttu-id="7c2ee-138">名前</span><span class="sxs-lookup"><span data-stu-id="7c2ee-138">Name</span></span>          | <span data-ttu-id="7c2ee-139">説明</span><span class="sxs-lookup"><span data-stu-id="7c2ee-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7c2ee-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c2ee-140">Authorization</span></span> | <span data-ttu-id="7c2ee-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7c2ee-143">応答</span><span class="sxs-lookup"><span data-stu-id="7c2ee-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="7c2ee-144">CSV</span><span class="sxs-lookup"><span data-stu-id="7c2ee-144">CSV</span></span>

<span data-ttu-id="7c2ee-145">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7c2ee-146">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7c2ee-147">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7c2ee-148">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7c2ee-149">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="7c2ee-149">Report Refresh Date</span></span>
- <span data-ttu-id="7c2ee-150">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="7c2ee-150">User Principal Name</span></span>
- <span data-ttu-id="7c2ee-151">削除済み</span><span class="sxs-lookup"><span data-stu-id="7c2ee-151">Is Deleted</span></span>
- <span data-ttu-id="7c2ee-152">削除日</span><span class="sxs-lookup"><span data-stu-id="7c2ee-152">Deleted Date</span></span>
- <span data-ttu-id="7c2ee-153">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="7c2ee-153">Last Activity Date</span></span>
- <span data-ttu-id="7c2ee-154">表示済みまたは編集済みファイルの数</span><span class="sxs-lookup"><span data-stu-id="7c2ee-154">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="7c2ee-155">同期済みファイルの数</span><span class="sxs-lookup"><span data-stu-id="7c2ee-155">Synced File Count</span></span>
- <span data-ttu-id="7c2ee-156">社内で共有済みファイルの数</span><span class="sxs-lookup"><span data-stu-id="7c2ee-156">Shared Internally File Count</span></span>
- <span data-ttu-id="7c2ee-157">外部で共有済みファイルの数</span><span class="sxs-lookup"><span data-stu-id="7c2ee-157">Shared Externally File Count</span></span>
- <span data-ttu-id="7c2ee-158">割り当て済み製品</span><span class="sxs-lookup"><span data-stu-id="7c2ee-158">Assigned Products</span></span>
- <span data-ttu-id="7c2ee-159">レポート期間</span><span class="sxs-lookup"><span data-stu-id="7c2ee-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="7c2ee-160">JSON</span><span class="sxs-lookup"><span data-stu-id="7c2ee-160">JSON</span></span>

<span data-ttu-id="7c2ee-161">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[Onedrive activityuserdetail](../resources/onedriveactivityuserdetail.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-161">If successful, this method returns a `200 OK` response code and a **[oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="7c2ee-162">この要求の既定のページサイズは200アイテムです。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-162">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="7c2ee-163">例</span><span class="sxs-lookup"><span data-stu-id="7c2ee-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="7c2ee-164">CSV</span><span class="sxs-lookup"><span data-stu-id="7c2ee-164">CSV</span></span>

<span data-ttu-id="7c2ee-165">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="7c2ee-166">要求</span><span class="sxs-lookup"><span data-stu-id="7c2ee-166">Request</span></span>

<span data-ttu-id="7c2ee-167">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-167">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7c2ee-168">プロトコル</span><span class="sxs-lookup"><span data-stu-id="7c2ee-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7c2ee-169">C#</span><span class="sxs-lookup"><span data-stu-id="7c2ee-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveactivityuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7c2ee-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c2ee-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveactivityuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7c2ee-171">目的-C</span><span class="sxs-lookup"><span data-stu-id="7c2ee-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveactivityuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7c2ee-172">応答</span><span class="sxs-lookup"><span data-stu-id="7c2ee-172">Response</span></span>

<span data-ttu-id="7c2ee-173">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-173">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7c2ee-174">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="7c2ee-175">JSON</span><span class="sxs-lookup"><span data-stu-id="7c2ee-175">JSON</span></span>

<span data-ttu-id="7c2ee-176">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-176">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="7c2ee-177">要求</span><span class="sxs-lookup"><span data-stu-id="7c2ee-177">Request</span></span>

<span data-ttu-id="7c2ee-178">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-178">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7c2ee-179">プロトコル</span><span class="sxs-lookup"><span data-stu-id="7c2ee-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7c2ee-180">C#</span><span class="sxs-lookup"><span data-stu-id="7c2ee-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveactivityuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7c2ee-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c2ee-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveactivityuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7c2ee-182">目的-C</span><span class="sxs-lookup"><span data-stu-id="7c2ee-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveactivityuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7c2ee-183">応答</span><span class="sxs-lookup"><span data-stu-id="7c2ee-183">Response</span></span>

<span data-ttu-id="7c2ee-184">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-184">The following is an example of the response.</span></span>

> <span data-ttu-id="7c2ee-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7c2ee-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "viewedOrEditedFileCount": 1, 
      "syncedFileCount": 0, 
      "sharedInternallyFileCount": 0, 
      "sharedExternallyFileCount": 0, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
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
