---
title: 'reportRoot: getOffice365GroupsActivityCounts'
description: グループ ワークロード全体のグループ活動の数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e83c32ffbd1a079c3a294eb3179c3737a0e31b02
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35446900"
---
# <a name="reportroot-getoffice365groupsactivitycounts"></a><span data-ttu-id="987c0-103">reportRoot: getOffice365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="987c0-103">reportRoot: getOffice365GroupsActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="987c0-104">グループ ワークロード全体のグループ活動の数を取得します。</span><span class="sxs-lookup"><span data-stu-id="987c0-104">Get the number of group activities across group workloads.</span></span>

> <span data-ttu-id="987c0-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Office 365 グループ](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="987c0-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="987c0-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="987c0-106">Permissions</span></span>

<span data-ttu-id="987c0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="987c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="987c0-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="987c0-109">Permission type</span></span>                        | <span data-ttu-id="987c0-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="987c0-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="987c0-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="987c0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="987c0-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="987c0-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="987c0-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="987c0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="987c0-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="987c0-114">Not supported.</span></span>                           |
| <span data-ttu-id="987c0-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="987c0-115">Application</span></span>                            | <span data-ttu-id="987c0-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="987c0-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="987c0-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="987c0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="987c0-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="987c0-118">Function parameters</span></span>

<span data-ttu-id="987c0-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="987c0-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="987c0-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="987c0-120">Parameter</span></span> | <span data-ttu-id="987c0-121">型</span><span class="sxs-lookup"><span data-stu-id="987c0-121">Type</span></span>   | <span data-ttu-id="987c0-122">説明</span><span class="sxs-lookup"><span data-stu-id="987c0-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="987c0-123">period</span><span class="sxs-lookup"><span data-stu-id="987c0-123">period</span></span>    | <span data-ttu-id="987c0-124">文字列</span><span class="sxs-lookup"><span data-stu-id="987c0-124">string</span></span> | <span data-ttu-id="987c0-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="987c0-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="987c0-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="987c0-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="987c0-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="987c0-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="987c0-128">必須。</span><span class="sxs-lookup"><span data-stu-id="987c0-128">Required.</span></span> |

<span data-ttu-id="987c0-129">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="987c0-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="987c0-130">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="987c0-130">The default output type is text/csv.</span></span> <span data-ttu-id="987c0-131">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="987c0-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="987c0-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="987c0-132">Request headers</span></span>

| <span data-ttu-id="987c0-133">名前</span><span class="sxs-lookup"><span data-stu-id="987c0-133">Name</span></span>          | <span data-ttu-id="987c0-134">説明</span><span class="sxs-lookup"><span data-stu-id="987c0-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="987c0-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="987c0-135">Authorization</span></span> | <span data-ttu-id="987c0-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="987c0-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="987c0-138">応答</span><span class="sxs-lookup"><span data-stu-id="987c0-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="987c0-139">CSV</span><span class="sxs-lookup"><span data-stu-id="987c0-139">CSV</span></span>

<span data-ttu-id="987c0-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="987c0-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="987c0-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="987c0-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="987c0-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="987c0-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="987c0-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="987c0-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="987c0-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="987c0-144">Report Refresh Date</span></span>
- <span data-ttu-id="987c0-145">受信した Exchange の電子メール</span><span class="sxs-lookup"><span data-stu-id="987c0-145">Exchange Emails Received</span></span>
- <span data-ttu-id="987c0-146">投稿された Yammer メッセージ</span><span class="sxs-lookup"><span data-stu-id="987c0-146">Yammer Messages Posted</span></span>
- <span data-ttu-id="987c0-147">読み取られた Yammer メッセージ</span><span class="sxs-lookup"><span data-stu-id="987c0-147">Yammer Messages Read</span></span>
- <span data-ttu-id="987c0-148">「いいね!」された Yammer メッセージ</span><span class="sxs-lookup"><span data-stu-id="987c0-148">Yammer Messages Liked</span></span>
- <span data-ttu-id="987c0-149">レポート日付</span><span class="sxs-lookup"><span data-stu-id="987c0-149">Report Date</span></span>
- <span data-ttu-id="987c0-150">レポート期間</span><span class="sxs-lookup"><span data-stu-id="987c0-150">Report Period</span></span>

<span data-ttu-id="987c0-151">次の列は、21Vianet が運用している Microsoft Graph 中国ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="987c0-151">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="987c0-152">投稿された Yammer メッセージ</span><span class="sxs-lookup"><span data-stu-id="987c0-152">Yammer Messages Posted</span></span>
- <span data-ttu-id="987c0-153">読み取られた Yammer メッセージ</span><span class="sxs-lookup"><span data-stu-id="987c0-153">Yammer Messages Read</span></span>
- <span data-ttu-id="987c0-154">「いいね!」された Yammer メッセージ</span><span class="sxs-lookup"><span data-stu-id="987c0-154">Yammer Messages Liked</span></span>

### <a name="json"></a><span data-ttu-id="987c0-155">JSON</span><span class="sxs-lookup"><span data-stu-id="987c0-155">JSON</span></span>

<span data-ttu-id="987c0-156">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="987c0-156">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object in the response body.</span></span>

<span data-ttu-id="987c0-157">**[Office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** オブジェクトの次のプロパティは、21vianet が運用している Microsoft Graph の中国ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="987c0-157">The following properties in **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="987c0-158">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="987c0-158">yammerMessagesPosted</span></span>
- <span data-ttu-id="987c0-159">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="987c0-159">yammerMessagesRead</span></span>
- <span data-ttu-id="987c0-160">yammerMessagesLiked</span><span class="sxs-lookup"><span data-stu-id="987c0-160">yammerMessagesLiked</span></span>

## <a name="example"></a><span data-ttu-id="987c0-161">例</span><span class="sxs-lookup"><span data-stu-id="987c0-161">Example</span></span>

### <a name="csv"></a><span data-ttu-id="987c0-162">CSV</span><span class="sxs-lookup"><span data-stu-id="987c0-162">CSV</span></span>

<span data-ttu-id="987c0-163">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="987c0-163">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="987c0-164">要求</span><span class="sxs-lookup"><span data-stu-id="987c0-164">Request</span></span>

<span data-ttu-id="987c0-165">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="987c0-165">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="987c0-166">プロトコル</span><span class="sxs-lookup"><span data-stu-id="987c0-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="987c0-167">C#</span><span class="sxs-lookup"><span data-stu-id="987c0-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivitycounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="987c0-168">Javascript</span><span class="sxs-lookup"><span data-stu-id="987c0-168">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivitycounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="987c0-169">目的-C</span><span class="sxs-lookup"><span data-stu-id="987c0-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivitycounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="987c0-170">応答</span><span class="sxs-lookup"><span data-stu-id="987c0-170">Response</span></span>

<span data-ttu-id="987c0-171">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="987c0-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="987c0-172">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="987c0-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Emails Received,Yammer Messages Posted,Yammer Messages Read,Yammer Messages Liked,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="987c0-173">JSON</span><span class="sxs-lookup"><span data-stu-id="987c0-173">JSON</span></span>

<span data-ttu-id="987c0-174">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="987c0-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="987c0-175">要求</span><span class="sxs-lookup"><span data-stu-id="987c0-175">Request</span></span>

<span data-ttu-id="987c0-176">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="987c0-176">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="987c0-177">プロトコル</span><span class="sxs-lookup"><span data-stu-id="987c0-177">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="987c0-178">C#</span><span class="sxs-lookup"><span data-stu-id="987c0-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivitycounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="987c0-179">Javascript</span><span class="sxs-lookup"><span data-stu-id="987c0-179">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivitycounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="987c0-180">目的-C</span><span class="sxs-lookup"><span data-stu-id="987c0-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivitycounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="987c0-181">応答</span><span class="sxs-lookup"><span data-stu-id="987c0-181">Response</span></span>

<span data-ttu-id="987c0-182">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="987c0-182">The following is an example of the response.</span></span>

> <span data-ttu-id="987c0-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="987c0-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 310

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "exchangeEmailsReceived": 0, 
      "yammerMessagesPosted": 0, 
      "yammerMessagesRead": 0, 
      "yammerMessagesLiked": 0, 
      "reportDate": "2017-09-01", 
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
