---
title: 'reportRoot: getTeamsUserActivityCounts'
description: アクティビティの種類ごとに、Microsoft Teams アクティビティの数を取得します。 アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話および会議です。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e221814d53c98d865a40a6c9e1d5d1917623f8d2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358811"
---
# <a name="reportroot-getteamsuseractivitycounts"></a><span data-ttu-id="60a20-104">reportRoot: getTeamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="60a20-104">reportRoot: getTeamsUserActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60a20-105">アクティビティの種類ごとに、Microsoft Teams アクティビティの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="60a20-105">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="60a20-106">アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話および会議です。</span><span class="sxs-lookup"><span data-stu-id="60a20-106">The activity types are team chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="60a20-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="60a20-107">Permissions</span></span>

<span data-ttu-id="60a20-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="60a20-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="60a20-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="60a20-110">Permission type</span></span>                        | <span data-ttu-id="60a20-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="60a20-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="60a20-112">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="60a20-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="60a20-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="60a20-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="60a20-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="60a20-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60a20-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60a20-115">Not supported.</span></span>                           |
| <span data-ttu-id="60a20-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="60a20-116">Application</span></span>                            | <span data-ttu-id="60a20-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="60a20-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="60a20-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="60a20-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="60a20-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="60a20-119">Function parameters</span></span>

<span data-ttu-id="60a20-120">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="60a20-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="60a20-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="60a20-121">Parameter</span></span> | <span data-ttu-id="60a20-122">型</span><span class="sxs-lookup"><span data-stu-id="60a20-122">Type</span></span>   | <span data-ttu-id="60a20-123">説明</span><span class="sxs-lookup"><span data-stu-id="60a20-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="60a20-124">period</span><span class="sxs-lookup"><span data-stu-id="60a20-124">period</span></span>    | <span data-ttu-id="60a20-125">文字列</span><span class="sxs-lookup"><span data-stu-id="60a20-125">string</span></span> | <span data-ttu-id="60a20-126">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="60a20-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="60a20-127">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="60a20-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="60a20-128">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="60a20-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="60a20-129">必須。</span><span class="sxs-lookup"><span data-stu-id="60a20-129">Required.</span></span> |

<span data-ttu-id="60a20-130">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="60a20-130">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="60a20-131">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="60a20-131">The default output type is text/csv.</span></span> <span data-ttu-id="60a20-132">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="60a20-132">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="60a20-133">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60a20-133">Request headers</span></span>

| <span data-ttu-id="60a20-134">名前</span><span class="sxs-lookup"><span data-stu-id="60a20-134">Name</span></span>          | <span data-ttu-id="60a20-135">説明</span><span class="sxs-lookup"><span data-stu-id="60a20-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="60a20-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="60a20-136">Authorization</span></span> | <span data-ttu-id="60a20-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="60a20-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="60a20-139">応答</span><span class="sxs-lookup"><span data-stu-id="60a20-139">Response</span></span>

### <a name="csv"></a><span data-ttu-id="60a20-140">CSV</span><span class="sxs-lookup"><span data-stu-id="60a20-140">CSV</span></span>

<span data-ttu-id="60a20-141">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="60a20-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="60a20-142">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="60a20-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="60a20-143">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="60a20-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="60a20-144">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="60a20-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="60a20-145">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="60a20-145">Report Refresh Date</span></span>
- <span data-ttu-id="60a20-146">レポート日付</span><span class="sxs-lookup"><span data-stu-id="60a20-146">Report Date</span></span>
- <span data-ttu-id="60a20-147">チーム チャット メッセージ</span><span class="sxs-lookup"><span data-stu-id="60a20-147">Team Chat Messages</span></span>
- <span data-ttu-id="60a20-148">非公開チャット メッセージ</span><span class="sxs-lookup"><span data-stu-id="60a20-148">Private Chat Messages</span></span>
- <span data-ttu-id="60a20-149">通話</span><span class="sxs-lookup"><span data-stu-id="60a20-149">Calls</span></span>
- <span data-ttu-id="60a20-150">会議</span><span class="sxs-lookup"><span data-stu-id="60a20-150">Meetings</span></span>
- <span data-ttu-id="60a20-151">レポート期間</span><span class="sxs-lookup"><span data-stu-id="60a20-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="60a20-152">JSON</span><span class="sxs-lookup"><span data-stu-id="60a20-152">JSON</span></span>

<span data-ttu-id="60a20-153">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[Teamsuseractivitycounts](../resources/teamsuseractivitycounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="60a20-153">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60a20-154">例</span><span class="sxs-lookup"><span data-stu-id="60a20-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="60a20-155">CSV</span><span class="sxs-lookup"><span data-stu-id="60a20-155">CSV</span></span>

<span data-ttu-id="60a20-156">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="60a20-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="60a20-157">要求</span><span class="sxs-lookup"><span data-stu-id="60a20-157">Request</span></span>

<span data-ttu-id="60a20-158">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="60a20-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="60a20-159">プロトコル</span><span class="sxs-lookup"><span data-stu-id="60a20-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="60a20-160">C#</span><span class="sxs-lookup"><span data-stu-id="60a20-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivitycounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="60a20-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60a20-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivitycounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="60a20-162">目的-C</span><span class="sxs-lookup"><span data-stu-id="60a20-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivitycounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="60a20-163">Java</span><span class="sxs-lookup"><span data-stu-id="60a20-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsuseractivitycounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="60a20-164">応答</span><span class="sxs-lookup"><span data-stu-id="60a20-164">Response</span></span>

<span data-ttu-id="60a20-165">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="60a20-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
<span data-ttu-id="60a20-166">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="60a20-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Report Period
```

### <a name="json"></a><span data-ttu-id="60a20-167">JSON</span><span class="sxs-lookup"><span data-stu-id="60a20-167">JSON</span></span>

<span data-ttu-id="60a20-168">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="60a20-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="60a20-169">要求</span><span class="sxs-lookup"><span data-stu-id="60a20-169">Request</span></span>

<span data-ttu-id="60a20-170">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="60a20-170">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="60a20-171">プロトコル</span><span class="sxs-lookup"><span data-stu-id="60a20-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="60a20-172">C#</span><span class="sxs-lookup"><span data-stu-id="60a20-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivitycounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="60a20-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60a20-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivitycounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="60a20-174">目的-C</span><span class="sxs-lookup"><span data-stu-id="60a20-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivitycounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="60a20-175">Java</span><span class="sxs-lookup"><span data-stu-id="60a20-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsuseractivitycounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="60a20-176">応答</span><span class="sxs-lookup"><span data-stu-id="60a20-176">Response</span></span>

<span data-ttu-id="60a20-177">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="60a20-177">The following is an example of the response.</span></span>

> <span data-ttu-id="60a20-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="60a20-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsUserActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 277

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsUserActivityCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "teamChatMessages": 26, 
      "privateChatMessages": 17, 
      "calls": 4, 
      "meetings": 0, 
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
