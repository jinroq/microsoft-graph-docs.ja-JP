---
title: 'reportRoot: getOffice365GroupsActivityCounts'
description: グループ ワークロード全体のグループ活動の数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: baf9a5390075c893acd4ac081bcbff4e50e1f0cb
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639426"
---
# <a name="reportroot-getoffice365groupsactivitycounts"></a><span data-ttu-id="5431b-103">reportRoot: getOffice365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="5431b-103">reportRoot: getOffice365GroupsActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5431b-104">グループ ワークロード全体のグループ活動の数を取得します。</span><span class="sxs-lookup"><span data-stu-id="5431b-104">Get the number of group activities across group workloads.</span></span>

> <span data-ttu-id="5431b-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Office 365 グループ](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5431b-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="5431b-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5431b-106">Permissions</span></span>

<span data-ttu-id="5431b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5431b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5431b-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5431b-109">Permission type</span></span>                        | <span data-ttu-id="5431b-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5431b-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5431b-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="5431b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5431b-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5431b-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5431b-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5431b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5431b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5431b-114">Not supported.</span></span>                           |
| <span data-ttu-id="5431b-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5431b-115">Application</span></span>                            | <span data-ttu-id="5431b-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5431b-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5431b-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5431b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="5431b-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="5431b-118">Function parameters</span></span>

<span data-ttu-id="5431b-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="5431b-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5431b-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="5431b-120">Parameter</span></span> | <span data-ttu-id="5431b-121">型</span><span class="sxs-lookup"><span data-stu-id="5431b-121">Type</span></span>   | <span data-ttu-id="5431b-122">説明</span><span class="sxs-lookup"><span data-stu-id="5431b-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5431b-123">period</span><span class="sxs-lookup"><span data-stu-id="5431b-123">period</span></span>    | <span data-ttu-id="5431b-124">文字列</span><span class="sxs-lookup"><span data-stu-id="5431b-124">string</span></span> | <span data-ttu-id="5431b-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="5431b-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5431b-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="5431b-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5431b-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="5431b-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5431b-128">必須。</span><span class="sxs-lookup"><span data-stu-id="5431b-128">Required.</span></span> |

<span data-ttu-id="5431b-129">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5431b-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="5431b-130">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="5431b-130">The default output type is text/csv.</span></span> <span data-ttu-id="5431b-131">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="5431b-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5431b-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5431b-132">Request headers</span></span>

| <span data-ttu-id="5431b-133">名前</span><span class="sxs-lookup"><span data-stu-id="5431b-133">Name</span></span>          | <span data-ttu-id="5431b-134">説明</span><span class="sxs-lookup"><span data-stu-id="5431b-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5431b-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="5431b-135">Authorization</span></span> | <span data-ttu-id="5431b-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5431b-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5431b-138">応答</span><span class="sxs-lookup"><span data-stu-id="5431b-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="5431b-139">CSV</span><span class="sxs-lookup"><span data-stu-id="5431b-139">CSV</span></span>

<span data-ttu-id="5431b-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="5431b-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5431b-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="5431b-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5431b-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="5431b-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5431b-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="5431b-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5431b-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="5431b-144">Report Refresh Date</span></span>
- <span data-ttu-id="5431b-145">受信した Exchange の電子メール</span><span class="sxs-lookup"><span data-stu-id="5431b-145">Exchange Emails Received</span></span>
- <span data-ttu-id="5431b-146">投稿された Yammer メッセージ</span><span class="sxs-lookup"><span data-stu-id="5431b-146">Yammer Messages Posted</span></span>
- <span data-ttu-id="5431b-147">読み取られた Yammer メッセージ</span><span class="sxs-lookup"><span data-stu-id="5431b-147">Yammer Messages Read</span></span>
- <span data-ttu-id="5431b-148">「いいね!」された Yammer メッセージ</span><span class="sxs-lookup"><span data-stu-id="5431b-148">Yammer Messages Liked</span></span>
- <span data-ttu-id="5431b-149">レポート日付</span><span class="sxs-lookup"><span data-stu-id="5431b-149">Report Date</span></span>
- <span data-ttu-id="5431b-150">レポート期間</span><span class="sxs-lookup"><span data-stu-id="5431b-150">Report Period</span></span>

<span data-ttu-id="5431b-151">次の列は、21Vianet が運用している Microsoft Graph 中国ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5431b-151">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="5431b-152">投稿された Yammer メッセージ</span><span class="sxs-lookup"><span data-stu-id="5431b-152">Yammer Messages Posted</span></span>
- <span data-ttu-id="5431b-153">読み取られた Yammer メッセージ</span><span class="sxs-lookup"><span data-stu-id="5431b-153">Yammer Messages Read</span></span>
- <span data-ttu-id="5431b-154">「いいね!」された Yammer メッセージ</span><span class="sxs-lookup"><span data-stu-id="5431b-154">Yammer Messages Liked</span></span>

### <a name="json"></a><span data-ttu-id="5431b-155">JSON</span><span class="sxs-lookup"><span data-stu-id="5431b-155">JSON</span></span>

<span data-ttu-id="5431b-156">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5431b-156">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object in the response body.</span></span>

<span data-ttu-id="5431b-157">**[Office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** オブジェクトの次のプロパティは、21vianet が運用している Microsoft Graph の中国ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5431b-157">The following properties in **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="5431b-158">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="5431b-158">yammerMessagesPosted</span></span>
- <span data-ttu-id="5431b-159">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="5431b-159">yammerMessagesRead</span></span>
- <span data-ttu-id="5431b-160">yammerMessagesLiked</span><span class="sxs-lookup"><span data-stu-id="5431b-160">yammerMessagesLiked</span></span>

## <a name="example"></a><span data-ttu-id="5431b-161">例</span><span class="sxs-lookup"><span data-stu-id="5431b-161">Example</span></span>

### <a name="csv"></a><span data-ttu-id="5431b-162">CSV</span><span class="sxs-lookup"><span data-stu-id="5431b-162">CSV</span></span>

<span data-ttu-id="5431b-163">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5431b-163">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="5431b-164">要求</span><span class="sxs-lookup"><span data-stu-id="5431b-164">Request</span></span>

<span data-ttu-id="5431b-165">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5431b-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="5431b-166">応答</span><span class="sxs-lookup"><span data-stu-id="5431b-166">Response</span></span>

<span data-ttu-id="5431b-167">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5431b-167">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5431b-168">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="5431b-168">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5431b-169">Visual</span><span class="sxs-lookup"><span data-stu-id="5431b-169">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivitycounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5431b-170">Java</span><span class="sxs-lookup"><span data-stu-id="5431b-170">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivitycounts_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="5431b-171">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="5431b-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="5431b-172">JSON</span><span class="sxs-lookup"><span data-stu-id="5431b-172">JSON</span></span>

<span data-ttu-id="5431b-173">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="5431b-173">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="5431b-174">要求</span><span class="sxs-lookup"><span data-stu-id="5431b-174">Request</span></span>

<span data-ttu-id="5431b-175">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5431b-175">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="5431b-176">応答</span><span class="sxs-lookup"><span data-stu-id="5431b-176">Response</span></span>

<span data-ttu-id="5431b-177">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5431b-177">The following is an example of the response.</span></span>

> <span data-ttu-id="5431b-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5431b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5431b-180">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="5431b-180">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5431b-181">Visual</span><span class="sxs-lookup"><span data-stu-id="5431b-181">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivitycounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5431b-182">Java</span><span class="sxs-lookup"><span data-stu-id="5431b-182">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivitycounts_json-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitycounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitycounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitycounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitycounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
