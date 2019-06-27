---
title: 'reportRoot: getOffice365GroupsActivityStorage'
description: すべてのグループ メールボックスとグループ サイトで使用されているストレージの合計を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c9f9c20c6bf0e9b7f33dc44307fa25cbe22eeb55
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265366"
---
# <a name="reportroot-getoffice365groupsactivitystorage"></a><span data-ttu-id="e3a44-103">reportRoot: getOffice365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="e3a44-103">reportRoot: getOffice365GroupsActivityStorage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3a44-104">すべてのグループ メールボックスとグループ サイトで使用されているストレージの合計を取得します。</span><span class="sxs-lookup"><span data-stu-id="e3a44-104">Get the total storage used across all group mailboxes and group sites.</span></span>

> <span data-ttu-id="e3a44-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Office 365 グループ](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3a44-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="e3a44-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e3a44-106">Permissions</span></span>

<span data-ttu-id="e3a44-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3a44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e3a44-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e3a44-109">Permission type</span></span>                        | <span data-ttu-id="e3a44-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e3a44-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e3a44-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="e3a44-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3a44-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3a44-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e3a44-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e3a44-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3a44-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3a44-114">Not supported.</span></span>                           |
| <span data-ttu-id="e3a44-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e3a44-115">Application</span></span>                            | <span data-ttu-id="e3a44-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3a44-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e3a44-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e3a44-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="e3a44-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="e3a44-118">Function parameters</span></span>

<span data-ttu-id="e3a44-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="e3a44-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e3a44-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e3a44-120">Parameter</span></span> | <span data-ttu-id="e3a44-121">型</span><span class="sxs-lookup"><span data-stu-id="e3a44-121">Type</span></span>   | <span data-ttu-id="e3a44-122">説明</span><span class="sxs-lookup"><span data-stu-id="e3a44-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e3a44-123">period</span><span class="sxs-lookup"><span data-stu-id="e3a44-123">period</span></span>    | <span data-ttu-id="e3a44-124">文字列</span><span class="sxs-lookup"><span data-stu-id="e3a44-124">string</span></span> | <span data-ttu-id="e3a44-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="e3a44-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e3a44-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="e3a44-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e3a44-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="e3a44-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e3a44-128">必須。</span><span class="sxs-lookup"><span data-stu-id="e3a44-128">Required.</span></span> |

<span data-ttu-id="e3a44-129">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e3a44-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e3a44-130">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="e3a44-130">The default output type is text/csv.</span></span> <span data-ttu-id="e3a44-131">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="e3a44-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3a44-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3a44-132">Request headers</span></span>

| <span data-ttu-id="e3a44-133">名前</span><span class="sxs-lookup"><span data-stu-id="e3a44-133">Name</span></span>          | <span data-ttu-id="e3a44-134">説明</span><span class="sxs-lookup"><span data-stu-id="e3a44-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e3a44-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3a44-135">Authorization</span></span> | <span data-ttu-id="e3a44-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e3a44-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e3a44-138">応答</span><span class="sxs-lookup"><span data-stu-id="e3a44-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e3a44-139">CSV</span><span class="sxs-lookup"><span data-stu-id="e3a44-139">CSV</span></span>

<span data-ttu-id="e3a44-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="e3a44-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e3a44-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="e3a44-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e3a44-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="e3a44-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e3a44-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="e3a44-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e3a44-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="e3a44-144">Report Refresh Date</span></span>
- <span data-ttu-id="e3a44-145">使用済みメールボックス ストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="e3a44-145">Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="e3a44-146">使用済みサイト ストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="e3a44-146">Site Storage Used (Byte)</span></span>
- <span data-ttu-id="e3a44-147">レポート日付</span><span class="sxs-lookup"><span data-stu-id="e3a44-147">Report Date</span></span>
- <span data-ttu-id="e3a44-148">レポート期間</span><span class="sxs-lookup"><span data-stu-id="e3a44-148">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="e3a44-149">JSON</span><span class="sxs-lookup"><span data-stu-id="e3a44-149">JSON</span></span>

<span data-ttu-id="e3a44-150">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e3a44-150">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3a44-151">例</span><span class="sxs-lookup"><span data-stu-id="e3a44-151">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e3a44-152">CSV</span><span class="sxs-lookup"><span data-stu-id="e3a44-152">CSV</span></span>

<span data-ttu-id="e3a44-153">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e3a44-153">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e3a44-154">要求</span><span class="sxs-lookup"><span data-stu-id="e3a44-154">Request</span></span>

<span data-ttu-id="e3a44-155">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e3a44-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitystorage_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityStorage(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="e3a44-156">応答</span><span class="sxs-lookup"><span data-stu-id="e3a44-156">Response</span></span>

<span data-ttu-id="e3a44-157">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e3a44-157">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e3a44-158">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="e3a44-158">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e3a44-159">C#</span><span class="sxs-lookup"><span data-stu-id="e3a44-159">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivitystorage_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e3a44-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="e3a44-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivitystorage_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e3a44-161">目的-C</span><span class="sxs-lookup"><span data-stu-id="e3a44-161">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivitystorage_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="e3a44-162">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="e3a44-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mailbox Storage Used (Byte),Site Storage Used (Byte),Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="e3a44-163">JSON</span><span class="sxs-lookup"><span data-stu-id="e3a44-163">JSON</span></span>

<span data-ttu-id="e3a44-164">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="e3a44-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e3a44-165">要求</span><span class="sxs-lookup"><span data-stu-id="e3a44-165">Request</span></span>

<span data-ttu-id="e3a44-166">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e3a44-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitystorage_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityStorage(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="e3a44-167">応答</span><span class="sxs-lookup"><span data-stu-id="e3a44-167">Response</span></span>

<span data-ttu-id="e3a44-168">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e3a44-168">The following is an example of the response.</span></span>

> <span data-ttu-id="e3a44-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e3a44-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityStorage"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityStorage)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "mailboxStorageUsedInBytes": 523143237898, 
      "siteStorageUsedInBytes": 31124384, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e3a44-171">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="e3a44-171">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e3a44-172">C#</span><span class="sxs-lookup"><span data-stu-id="e3a44-172">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivitystorage_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e3a44-173">Javascript</span><span class="sxs-lookup"><span data-stu-id="e3a44-173">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivitystorage_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e3a44-174">目的-C</span><span class="sxs-lookup"><span data-stu-id="e3a44-174">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivitystorage_json-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitystorage.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitystorage.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitystorage.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitystorage.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitystorage.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
