---
title: 'reportRoot: getSharePointActivityPages'
description: ユーザーがアクセスしたそれぞれ別個のページ数を取得します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 9ac10f5896ea9b913e8816514a64993716c2fae9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526803"
---
# <a name="reportroot-getsharepointactivitypages"></a><span data-ttu-id="9a9e6-103">reportRoot: getSharePointActivityPages</span><span class="sxs-lookup"><span data-stu-id="9a9e6-103">reportRoot: getSharePointActivityPages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a9e6-104">ユーザーがアクセスしたそれぞれ別個のページ数を取得します。</span><span class="sxs-lookup"><span data-stu-id="9a9e6-104">Get the number of unique pages visited by users.</span></span>

> <span data-ttu-id="9a9e6-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint アクティビティ](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a9e6-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="9a9e6-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9a9e6-106">Permissions</span></span>

<span data-ttu-id="9a9e6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a9e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9a9e6-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9a9e6-109">Permission type</span></span>                        | <span data-ttu-id="9a9e6-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9a9e6-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9a9e6-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="9a9e6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9a9e6-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a9e6-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9a9e6-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9a9e6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a9e6-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a9e6-114">Not supported.</span></span>                           |
| <span data-ttu-id="9a9e6-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9a9e6-115">Application</span></span>                            | <span data-ttu-id="9a9e6-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a9e6-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="9a9e6-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9a9e6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityPages(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="9a9e6-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="9a9e6-118">Function parameters</span></span>

<span data-ttu-id="9a9e6-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="9a9e6-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="9a9e6-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="9a9e6-120">Parameter</span></span> | <span data-ttu-id="9a9e6-121">型</span><span class="sxs-lookup"><span data-stu-id="9a9e6-121">Type</span></span>   | <span data-ttu-id="9a9e6-122">説明</span><span class="sxs-lookup"><span data-stu-id="9a9e6-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9a9e6-123">period</span><span class="sxs-lookup"><span data-stu-id="9a9e6-123">period</span></span>    | <span data-ttu-id="9a9e6-124">文字列</span><span class="sxs-lookup"><span data-stu-id="9a9e6-124">string</span></span> | <span data-ttu-id="9a9e6-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="9a9e6-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9a9e6-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="9a9e6-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9a9e6-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="9a9e6-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="9a9e6-128">必須。</span><span class="sxs-lookup"><span data-stu-id="9a9e6-128">Required.</span></span> |

<span data-ttu-id="9a9e6-129">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="9a9e6-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="9a9e6-130">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="9a9e6-130">The default output type is text/csv.</span></span> <span data-ttu-id="9a9e6-131">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="9a9e6-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a9e6-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a9e6-132">Request headers</span></span>

| <span data-ttu-id="9a9e6-133">名前</span><span class="sxs-lookup"><span data-stu-id="9a9e6-133">Name</span></span>          | <span data-ttu-id="9a9e6-134">説明</span><span class="sxs-lookup"><span data-stu-id="9a9e6-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="9a9e6-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a9e6-135">Authorization</span></span> | <span data-ttu-id="9a9e6-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9a9e6-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="9a9e6-138">応答</span><span class="sxs-lookup"><span data-stu-id="9a9e6-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="9a9e6-139">CSV</span><span class="sxs-lookup"><span data-stu-id="9a9e6-139">CSV</span></span>

<span data-ttu-id="9a9e6-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="9a9e6-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9a9e6-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="9a9e6-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9a9e6-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="9a9e6-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9a9e6-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="9a9e6-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9a9e6-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="9a9e6-144">Report Refresh Date</span></span>
- <span data-ttu-id="9a9e6-145">アクセスしたページ数</span><span class="sxs-lookup"><span data-stu-id="9a9e6-145">Visited Page Count</span></span>
- <span data-ttu-id="9a9e6-146">レポート日付</span><span class="sxs-lookup"><span data-stu-id="9a9e6-146">Report Date</span></span>
- <span data-ttu-id="9a9e6-147">レポート期間</span><span class="sxs-lookup"><span data-stu-id="9a9e6-147">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="9a9e6-148">JSON</span><span class="sxs-lookup"><span data-stu-id="9a9e6-148">JSON</span></span>

<span data-ttu-id="9a9e6-149">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[sharePointActivityPages](../resources/sharepointactivitypages.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="9a9e6-149">If successful, this method returns a `200 OK` response code and a **[sharePointActivityPages](../resources/sharepointactivitypages.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a9e6-150">例</span><span class="sxs-lookup"><span data-stu-id="9a9e6-150">Example</span></span>

### <a name="csv"></a><span data-ttu-id="9a9e6-151">CSV</span><span class="sxs-lookup"><span data-stu-id="9a9e6-151">CSV</span></span>

<span data-ttu-id="9a9e6-152">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="9a9e6-152">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="9a9e6-153">要求</span><span class="sxs-lookup"><span data-stu-id="9a9e6-153">Request</span></span>

<span data-ttu-id="9a9e6-154">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9a9e6-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivitypages_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityPages(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="9a9e6-155">応答</span><span class="sxs-lookup"><span data-stu-id="9a9e6-155">Response</span></span>

<span data-ttu-id="9a9e6-156">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9a9e6-156">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="9a9e6-157">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="9a9e6-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page Count,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="9a9e6-158">JSON</span><span class="sxs-lookup"><span data-stu-id="9a9e6-158">JSON</span></span>

<span data-ttu-id="9a9e6-159">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="9a9e6-159">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="9a9e6-160">要求</span><span class="sxs-lookup"><span data-stu-id="9a9e6-160">Request</span></span>

<span data-ttu-id="9a9e6-161">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9a9e6-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivitypages_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityPages(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="9a9e6-162">応答</span><span class="sxs-lookup"><span data-stu-id="9a9e6-162">Response</span></span>

<span data-ttu-id="9a9e6-163">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9a9e6-163">The following is an example of the response.</span></span>

> <span data-ttu-id="9a9e6-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9a9e6-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointActivityPages"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointActivityPages)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "visitedPageCount": 195, 
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
    "Error: /api-reference/beta/api/reportroot-getsharepointactivitypages.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
