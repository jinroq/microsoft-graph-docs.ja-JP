---
title: 'reportRoot: getSkypeForBusinessActivityUserCounts'
description: Skype for Business を介して組織内で行われた会議セッションにおける、それぞれ別個の開催ユーザー数と参加ユーザー数の傾向を取得します。 レポートには、ピア ツー ピア セッションの数も含まれます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: b4d6c70f2c6dc8045696982ec2b402a2d899076c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359702"
---
# <a name="reportroot-getskypeforbusinessactivityusercounts"></a><span data-ttu-id="cb0ce-104">reportRoot: getSkypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="cb0ce-104">reportRoot: getSkypeForBusinessActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb0ce-105">Skype for Business を介して組織内で行われた会議セッションにおける、それぞれ別個の開催ユーザー数と参加ユーザー数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="cb0ce-105">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="cb0ce-106">レポートには、ピア ツー ピア セッションの数も含まれます。</span><span class="sxs-lookup"><span data-stu-id="cb0ce-106">The report also includes the number of peer-to-peer sessions.</span></span>

> <span data-ttu-id="cb0ce-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business アクティビティ](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cb0ce-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="cb0ce-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cb0ce-108">Permissions</span></span>

<span data-ttu-id="cb0ce-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cb0ce-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cb0ce-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cb0ce-111">Permission type</span></span>                        | <span data-ttu-id="cb0ce-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cb0ce-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="cb0ce-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="cb0ce-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb0ce-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb0ce-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="cb0ce-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cb0ce-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb0ce-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cb0ce-116">Not supported.</span></span>                           |
| <span data-ttu-id="cb0ce-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cb0ce-117">Application</span></span>                            | <span data-ttu-id="cb0ce-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb0ce-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="cb0ce-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cb0ce-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="cb0ce-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="cb0ce-120">Function parameters</span></span>

<span data-ttu-id="cb0ce-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="cb0ce-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="cb0ce-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="cb0ce-122">Parameter</span></span> | <span data-ttu-id="cb0ce-123">型</span><span class="sxs-lookup"><span data-stu-id="cb0ce-123">Type</span></span>   | <span data-ttu-id="cb0ce-124">説明</span><span class="sxs-lookup"><span data-stu-id="cb0ce-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="cb0ce-125">period</span><span class="sxs-lookup"><span data-stu-id="cb0ce-125">period</span></span>    | <span data-ttu-id="cb0ce-126">文字列</span><span class="sxs-lookup"><span data-stu-id="cb0ce-126">string</span></span> | <span data-ttu-id="cb0ce-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="cb0ce-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="cb0ce-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="cb0ce-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="cb0ce-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="cb0ce-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="cb0ce-130">必須。</span><span class="sxs-lookup"><span data-stu-id="cb0ce-130">Required.</span></span> |

<span data-ttu-id="cb0ce-131">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="cb0ce-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="cb0ce-132">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="cb0ce-132">The default output type is text/csv.</span></span> <span data-ttu-id="cb0ce-133">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="cb0ce-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cb0ce-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cb0ce-134">Request headers</span></span>

| <span data-ttu-id="cb0ce-135">名前</span><span class="sxs-lookup"><span data-stu-id="cb0ce-135">Name</span></span>          | <span data-ttu-id="cb0ce-136">説明</span><span class="sxs-lookup"><span data-stu-id="cb0ce-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="cb0ce-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb0ce-137">Authorization</span></span> | <span data-ttu-id="cb0ce-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cb0ce-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="cb0ce-140">応答</span><span class="sxs-lookup"><span data-stu-id="cb0ce-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="cb0ce-141">CSV</span><span class="sxs-lookup"><span data-stu-id="cb0ce-141">CSV</span></span>

<span data-ttu-id="cb0ce-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="cb0ce-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="cb0ce-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="cb0ce-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="cb0ce-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="cb0ce-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="cb0ce-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="cb0ce-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="cb0ce-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="cb0ce-146">Report Refresh Date</span></span>
- <span data-ttu-id="cb0ce-147">レポート日付</span><span class="sxs-lookup"><span data-stu-id="cb0ce-147">Report Date</span></span>
- <span data-ttu-id="cb0ce-148">レポート期間</span><span class="sxs-lookup"><span data-stu-id="cb0ce-148">Report Period</span></span>
- <span data-ttu-id="cb0ce-149">ピアツーピア</span><span class="sxs-lookup"><span data-stu-id="cb0ce-149">Peer-to-peer</span></span>
- <span data-ttu-id="cb0ce-150">開催</span><span class="sxs-lookup"><span data-stu-id="cb0ce-150">Organized</span></span>
- <span data-ttu-id="cb0ce-151">参加</span><span class="sxs-lookup"><span data-stu-id="cb0ce-151">Participated</span></span>

### <a name="json"></a><span data-ttu-id="cb0ce-152">JSON</span><span class="sxs-lookup"><span data-stu-id="cb0ce-152">JSON</span></span>

<span data-ttu-id="cb0ce-153">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[Skypeforbusinessactivityusercounts](../resources/skypeforbusinessactivityusercounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cb0ce-153">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb0ce-154">例</span><span class="sxs-lookup"><span data-stu-id="cb0ce-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="cb0ce-155">CSV</span><span class="sxs-lookup"><span data-stu-id="cb0ce-155">CSV</span></span>

<span data-ttu-id="cb0ce-156">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cb0ce-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="cb0ce-157">要求</span><span class="sxs-lookup"><span data-stu-id="cb0ce-157">Request</span></span>

<span data-ttu-id="cb0ce-158">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cb0ce-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="cb0ce-159">プロトコル</span><span class="sxs-lookup"><span data-stu-id="cb0ce-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cb0ce-160">C#</span><span class="sxs-lookup"><span data-stu-id="cb0ce-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessactivityusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cb0ce-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cb0ce-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessactivityusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cb0ce-162">目的-C</span><span class="sxs-lookup"><span data-stu-id="cb0ce-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessactivityusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cb0ce-163">Java</span><span class="sxs-lookup"><span data-stu-id="cb0ce-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessactivityusercounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cb0ce-164">応答</span><span class="sxs-lookup"><span data-stu-id="cb0ce-164">Response</span></span>

<span data-ttu-id="cb0ce-165">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cb0ce-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="cb0ce-166">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="cb0ce-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Peer-to-peer,Organized,Participated
```

### <a name="json"></a><span data-ttu-id="cb0ce-167">JSON</span><span class="sxs-lookup"><span data-stu-id="cb0ce-167">JSON</span></span>

<span data-ttu-id="cb0ce-168">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="cb0ce-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="cb0ce-169">要求</span><span class="sxs-lookup"><span data-stu-id="cb0ce-169">Request</span></span>

<span data-ttu-id="cb0ce-170">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cb0ce-170">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="cb0ce-171">プロトコル</span><span class="sxs-lookup"><span data-stu-id="cb0ce-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cb0ce-172">C#</span><span class="sxs-lookup"><span data-stu-id="cb0ce-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessactivityusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cb0ce-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cb0ce-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessactivityusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cb0ce-174">目的-C</span><span class="sxs-lookup"><span data-stu-id="cb0ce-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessactivityusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cb0ce-175">Java</span><span class="sxs-lookup"><span data-stu-id="cb0ce-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessactivityusercounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cb0ce-176">応答</span><span class="sxs-lookup"><span data-stu-id="cb0ce-176">Response</span></span>

<span data-ttu-id="cb0ce-177">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cb0ce-177">The following is an example of the response.</span></span>

> <span data-ttu-id="cb0ce-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="cb0ce-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 266

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessActivityUserCounts)", 
  "value": [
    {
      "peerToPeer": 413, 
      "organized": 30, 
      "participated": 91, 
      "reportRefreshDate": "2017-09-01", 
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
