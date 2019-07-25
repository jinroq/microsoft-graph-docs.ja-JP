---
title: 'reportRoot: getSharePointActivityFileCounts'
description: SharePoint サイトに保存されているファイルを操作した、それぞれ別個のライセンス ユーザーの数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 73e9c18603756a90b7c5ed9e4823d07b4f627a3e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872892"
---
# <a name="reportroot-getsharepointactivityfilecounts"></a><span data-ttu-id="4ecf0-103">reportRoot: getSharePointActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="4ecf0-103">reportRoot: getSharePointActivityFileCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ecf0-104">SharePoint サイトに保存されているファイルを操作した、それぞれ別個のライセンス ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="4ecf0-104">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span>

> <span data-ttu-id="4ecf0-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint アクティビティ](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4ecf0-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="4ecf0-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4ecf0-106">Permissions</span></span>

<span data-ttu-id="4ecf0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4ecf0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4ecf0-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4ecf0-109">Permission type</span></span>                        | <span data-ttu-id="4ecf0-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4ecf0-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4ecf0-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="4ecf0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4ecf0-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ecf0-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4ecf0-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4ecf0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ecf0-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4ecf0-114">Not supported.</span></span>                           |
| <span data-ttu-id="4ecf0-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4ecf0-115">Application</span></span>                            | <span data-ttu-id="4ecf0-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ecf0-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4ecf0-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4ecf0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4ecf0-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="4ecf0-118">Function parameters</span></span>

<span data-ttu-id="4ecf0-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="4ecf0-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4ecf0-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="4ecf0-120">Parameter</span></span> | <span data-ttu-id="4ecf0-121">型</span><span class="sxs-lookup"><span data-stu-id="4ecf0-121">Type</span></span>   | <span data-ttu-id="4ecf0-122">説明</span><span class="sxs-lookup"><span data-stu-id="4ecf0-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4ecf0-123">period</span><span class="sxs-lookup"><span data-stu-id="4ecf0-123">period</span></span>    | <span data-ttu-id="4ecf0-124">文字列</span><span class="sxs-lookup"><span data-stu-id="4ecf0-124">string</span></span> | <span data-ttu-id="4ecf0-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="4ecf0-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4ecf0-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="4ecf0-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4ecf0-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="4ecf0-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4ecf0-128">必須。</span><span class="sxs-lookup"><span data-stu-id="4ecf0-128">Required.</span></span> |

<span data-ttu-id="4ecf0-129">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="4ecf0-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4ecf0-130">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="4ecf0-130">The default output type is text/csv.</span></span> <span data-ttu-id="4ecf0-131">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="4ecf0-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ecf0-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4ecf0-132">Request headers</span></span>

| <span data-ttu-id="4ecf0-133">名前</span><span class="sxs-lookup"><span data-stu-id="4ecf0-133">Name</span></span>          | <span data-ttu-id="4ecf0-134">説明</span><span class="sxs-lookup"><span data-stu-id="4ecf0-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4ecf0-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ecf0-135">Authorization</span></span> | <span data-ttu-id="4ecf0-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4ecf0-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4ecf0-138">応答</span><span class="sxs-lookup"><span data-stu-id="4ecf0-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4ecf0-139">CSV</span><span class="sxs-lookup"><span data-stu-id="4ecf0-139">CSV</span></span>

<span data-ttu-id="4ecf0-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="4ecf0-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4ecf0-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="4ecf0-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4ecf0-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="4ecf0-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4ecf0-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="4ecf0-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4ecf0-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="4ecf0-144">Report Refresh Date</span></span>
- <span data-ttu-id="4ecf0-145">表示済みまたは編集済み</span><span class="sxs-lookup"><span data-stu-id="4ecf0-145">Viewed Or Edited</span></span>
- <span data-ttu-id="4ecf0-146">同期済み</span><span class="sxs-lookup"><span data-stu-id="4ecf0-146">Synced</span></span>
- <span data-ttu-id="4ecf0-147">社内で共有済み</span><span class="sxs-lookup"><span data-stu-id="4ecf0-147">Shared Internally</span></span>
- <span data-ttu-id="4ecf0-148">外部で共有済み</span><span class="sxs-lookup"><span data-stu-id="4ecf0-148">Shared Externally</span></span>
- <span data-ttu-id="4ecf0-149">レポート日付</span><span class="sxs-lookup"><span data-stu-id="4ecf0-149">Report Date</span></span>
- <span data-ttu-id="4ecf0-150">レポート期間</span><span class="sxs-lookup"><span data-stu-id="4ecf0-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="4ecf0-151">JSON</span><span class="sxs-lookup"><span data-stu-id="4ecf0-151">JSON</span></span>

<span data-ttu-id="4ecf0-152">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[siteactivitysummary](../resources/siteactivitysummary.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4ecf0-152">If successful, this method returns a `200 OK` response code and a **[siteActivitySummary](../resources/siteactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ecf0-153">例</span><span class="sxs-lookup"><span data-stu-id="4ecf0-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4ecf0-154">CSV</span><span class="sxs-lookup"><span data-stu-id="4ecf0-154">CSV</span></span>

<span data-ttu-id="4ecf0-155">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4ecf0-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4ecf0-156">要求</span><span class="sxs-lookup"><span data-stu-id="4ecf0-156">Request</span></span>

<span data-ttu-id="4ecf0-157">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4ecf0-157">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4ecf0-158">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4ecf0-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityfilecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityFileCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4ecf0-159">C#</span><span class="sxs-lookup"><span data-stu-id="4ecf0-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointactivityfilecounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4ecf0-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="4ecf0-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointactivityfilecounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4ecf0-161">目的-C</span><span class="sxs-lookup"><span data-stu-id="4ecf0-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointactivityfilecounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4ecf0-162">Java</span><span class="sxs-lookup"><span data-stu-id="4ecf0-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointactivityfilecounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4ecf0-163">応答</span><span class="sxs-lookup"><span data-stu-id="4ecf0-163">Response</span></span>

<span data-ttu-id="4ecf0-164">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4ecf0-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4ecf0-165">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="4ecf0-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="4ecf0-166">JSON</span><span class="sxs-lookup"><span data-stu-id="4ecf0-166">JSON</span></span>

<span data-ttu-id="4ecf0-167">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="4ecf0-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4ecf0-168">要求</span><span class="sxs-lookup"><span data-stu-id="4ecf0-168">Request</span></span>

<span data-ttu-id="4ecf0-169">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4ecf0-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4ecf0-170">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4ecf0-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4ecf0-171">C#</span><span class="sxs-lookup"><span data-stu-id="4ecf0-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4ecf0-172">Javascript</span><span class="sxs-lookup"><span data-stu-id="4ecf0-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4ecf0-173">目的-C</span><span class="sxs-lookup"><span data-stu-id="4ecf0-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4ecf0-174">Java</span><span class="sxs-lookup"><span data-stu-id="4ecf0-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activeusercounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4ecf0-175">応答</span><span class="sxs-lookup"><span data-stu-id="4ecf0-175">Response</span></span>

<span data-ttu-id="4ecf0-176">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4ecf0-176">The following is an example of the response.</span></span>

> <span data-ttu-id="4ecf0-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4ecf0-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 278

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "viewedOrEdited": 2141, 
      "synced": 614, 
      "sharedInternally": 9, 
      "sharedExternally": 0, 
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
