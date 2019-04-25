---
title: 'reportRoot: getYammerActivityUserCounts'
description: Yammer メッセージを投稿、読み取り、および「いいね!」を付けた一意のユーザーの数の傾向を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: fa2648990bacd69e8d4597d33c7b10c5a388bba2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537911"
---
# <a name="reportroot-getyammeractivityusercounts"></a><span data-ttu-id="e9880-103">reportRoot: getYammerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="e9880-103">reportRoot: getYammerActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9880-104">Yammer メッセージを投稿、読み取り、および「いいね!」を付けた一意のユーザーの数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="e9880-104">Get the trends on the number of unique users who posted, read, and liked Yammer messages.</span></span>

> <span data-ttu-id="e9880-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer アクティビティ](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e9880-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="e9880-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e9880-106">Permissions</span></span>

<span data-ttu-id="e9880-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e9880-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e9880-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e9880-109">Permission type</span></span>                        | <span data-ttu-id="e9880-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e9880-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e9880-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e9880-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e9880-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9880-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e9880-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e9880-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9880-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e9880-114">Not supported.</span></span>                           |
| <span data-ttu-id="e9880-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e9880-115">Application</span></span>                            | <span data-ttu-id="e9880-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9880-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e9880-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e9880-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="e9880-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="e9880-118">Function parameters</span></span>

<span data-ttu-id="e9880-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="e9880-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e9880-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e9880-120">Parameter</span></span> | <span data-ttu-id="e9880-121">型</span><span class="sxs-lookup"><span data-stu-id="e9880-121">Type</span></span>   | <span data-ttu-id="e9880-122">説明</span><span class="sxs-lookup"><span data-stu-id="e9880-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e9880-123">period</span><span class="sxs-lookup"><span data-stu-id="e9880-123">period</span></span>    | <span data-ttu-id="e9880-124">文字列</span><span class="sxs-lookup"><span data-stu-id="e9880-124">string</span></span> | <span data-ttu-id="e9880-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="e9880-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e9880-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="e9880-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e9880-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="e9880-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e9880-128">必須。</span><span class="sxs-lookup"><span data-stu-id="e9880-128">Required.</span></span> |

<span data-ttu-id="e9880-129">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e9880-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e9880-130">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="e9880-130">The default output type is text/csv.</span></span> <span data-ttu-id="e9880-131">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="e9880-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9880-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e9880-132">Request headers</span></span>

| <span data-ttu-id="e9880-133">名前</span><span class="sxs-lookup"><span data-stu-id="e9880-133">Name</span></span>          | <span data-ttu-id="e9880-134">説明</span><span class="sxs-lookup"><span data-stu-id="e9880-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e9880-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9880-135">Authorization</span></span> | <span data-ttu-id="e9880-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e9880-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e9880-138">応答</span><span class="sxs-lookup"><span data-stu-id="e9880-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e9880-139">CSV</span><span class="sxs-lookup"><span data-stu-id="e9880-139">CSV</span></span>

<span data-ttu-id="e9880-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="e9880-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e9880-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="e9880-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e9880-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="e9880-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e9880-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="e9880-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e9880-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="e9880-144">Report Refresh Date</span></span>
- <span data-ttu-id="e9880-145">いいね!</span><span class="sxs-lookup"><span data-stu-id="e9880-145">Liked</span></span>
- <span data-ttu-id="e9880-146">投稿</span><span class="sxs-lookup"><span data-stu-id="e9880-146">Posted</span></span>
- <span data-ttu-id="e9880-147">読み取り</span><span class="sxs-lookup"><span data-stu-id="e9880-147">Read</span></span>
- <span data-ttu-id="e9880-148">レポート日付</span><span class="sxs-lookup"><span data-stu-id="e9880-148">Report Date</span></span>
- <span data-ttu-id="e9880-149">レポート期間</span><span class="sxs-lookup"><span data-stu-id="e9880-149">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="e9880-150">JSON</span><span class="sxs-lookup"><span data-stu-id="e9880-150">JSON</span></span>

<span data-ttu-id="e9880-151">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[yammerActivitySummary](../resources/yammeractivitysummary.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e9880-151">If successful, this method returns a `200 OK` response code and a **[yammerActivitySummary](../resources/yammeractivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9880-152">例</span><span class="sxs-lookup"><span data-stu-id="e9880-152">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e9880-153">CSV</span><span class="sxs-lookup"><span data-stu-id="e9880-153">CSV</span></span>

<span data-ttu-id="e9880-154">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e9880-154">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e9880-155">要求</span><span class="sxs-lookup"><span data-stu-id="e9880-155">Request</span></span>

<span data-ttu-id="e9880-156">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e9880-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="e9880-157">応答</span><span class="sxs-lookup"><span data-stu-id="e9880-157">Response</span></span>

<span data-ttu-id="e9880-158">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e9880-158">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="e9880-159">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="e9880-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="e9880-160">JSON</span><span class="sxs-lookup"><span data-stu-id="e9880-160">JSON</span></span>

<span data-ttu-id="e9880-161">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="e9880-161">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e9880-162">要求</span><span class="sxs-lookup"><span data-stu-id="e9880-162">Request</span></span>

<span data-ttu-id="e9880-163">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e9880-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="e9880-164">応答</span><span class="sxs-lookup"><span data-stu-id="e9880-164">Response</span></span>

<span data-ttu-id="e9880-165">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e9880-165">The following is an example of the response.</span></span>

> <span data-ttu-id="e9880-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e9880-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 236

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "liked": 40, 
      "posted": 54, 
      "read": 28, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getyammeractivityusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
