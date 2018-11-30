---
title: 'reportRoot: getSharePointActivityPages'
description: ユーザーがアクセスしたそれぞれ別個のページ数を取得します。
ms.openlocfilehash: b9e98eebccb82061d4a601068d4e953fb3f246b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067480"
---
# <a name="reportroot-getsharepointactivitypages"></a><span data-ttu-id="0fd04-103">reportRoot: getSharePointActivityPages</span><span class="sxs-lookup"><span data-stu-id="0fd04-103">reportRoot: getSharePointActivityPages</span></span>

> <span data-ttu-id="0fd04-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0fd04-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0fd04-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0fd04-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0fd04-106">ユーザーがアクセスしたそれぞれ別個のページ数を取得します。</span><span class="sxs-lookup"><span data-stu-id="0fd04-106">Get the number of unique pages visited by users.</span></span>

> <span data-ttu-id="0fd04-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint アクティビティ](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0fd04-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="0fd04-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0fd04-108">Permissions</span></span>

<span data-ttu-id="0fd04-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0fd04-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0fd04-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0fd04-111">Permission type</span></span>                        | <span data-ttu-id="0fd04-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0fd04-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0fd04-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="0fd04-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="0fd04-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0fd04-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0fd04-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0fd04-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fd04-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0fd04-116">Not supported.</span></span>                           |
| <span data-ttu-id="0fd04-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0fd04-117">Application</span></span>                            | <span data-ttu-id="0fd04-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0fd04-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0fd04-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0fd04-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityPages(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="0fd04-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="0fd04-120">Function parameters</span></span>

<span data-ttu-id="0fd04-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="0fd04-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="0fd04-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="0fd04-122">Parameter</span></span> | <span data-ttu-id="0fd04-123">型</span><span class="sxs-lookup"><span data-stu-id="0fd04-123">Type</span></span>   | <span data-ttu-id="0fd04-124">説明</span><span class="sxs-lookup"><span data-stu-id="0fd04-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0fd04-125">period</span><span class="sxs-lookup"><span data-stu-id="0fd04-125">period</span></span>    | <span data-ttu-id="0fd04-126">文字列</span><span class="sxs-lookup"><span data-stu-id="0fd04-126">string</span></span> | <span data-ttu-id="0fd04-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="0fd04-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0fd04-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="0fd04-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0fd04-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="0fd04-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="0fd04-130">必須。</span><span class="sxs-lookup"><span data-stu-id="0fd04-130">Required.</span></span> |

<span data-ttu-id="0fd04-131">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="0fd04-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="0fd04-132">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="0fd04-132">The default output type is text/csv.</span></span> <span data-ttu-id="0fd04-133">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="0fd04-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0fd04-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0fd04-134">Request headers</span></span>

| <span data-ttu-id="0fd04-135">名前</span><span class="sxs-lookup"><span data-stu-id="0fd04-135">Name</span></span>          | <span data-ttu-id="0fd04-136">説明</span><span class="sxs-lookup"><span data-stu-id="0fd04-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0fd04-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fd04-137">Authorization</span></span> | <span data-ttu-id="0fd04-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0fd04-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0fd04-140">応答</span><span class="sxs-lookup"><span data-stu-id="0fd04-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="0fd04-141">CSV</span><span class="sxs-lookup"><span data-stu-id="0fd04-141">CSV</span></span>

<span data-ttu-id="0fd04-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="0fd04-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0fd04-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="0fd04-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0fd04-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="0fd04-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0fd04-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="0fd04-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0fd04-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="0fd04-146">Report Refresh Date</span></span>
- <span data-ttu-id="0fd04-147">アクセスしたページ数</span><span class="sxs-lookup"><span data-stu-id="0fd04-147">Visited Page Count</span></span>
- <span data-ttu-id="0fd04-148">レポート日付</span><span class="sxs-lookup"><span data-stu-id="0fd04-148">Report Date</span></span>
- <span data-ttu-id="0fd04-149">レポート期間</span><span class="sxs-lookup"><span data-stu-id="0fd04-149">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="0fd04-150">JSON</span><span class="sxs-lookup"><span data-stu-id="0fd04-150">JSON</span></span>

<span data-ttu-id="0fd04-151">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[sharePointActivityPages](../resources/sharepointactivitypages.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="0fd04-151">If successful, this method returns a `200 OK` response code and a **[sharePointActivityPages](../resources/sharepointactivitypages.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fd04-152">使用例</span><span class="sxs-lookup"><span data-stu-id="0fd04-152">Example</span></span>

### <a name="csv"></a><span data-ttu-id="0fd04-153">CSV</span><span class="sxs-lookup"><span data-stu-id="0fd04-153">CSV</span></span>

<span data-ttu-id="0fd04-154">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="0fd04-154">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="0fd04-155">要求</span><span class="sxs-lookup"><span data-stu-id="0fd04-155">Request</span></span>

<span data-ttu-id="0fd04-156">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0fd04-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivitypages_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityPages(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="0fd04-157">応答</span><span class="sxs-lookup"><span data-stu-id="0fd04-157">Response</span></span>

<span data-ttu-id="0fd04-158">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0fd04-158">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="0fd04-159">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="0fd04-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="0fd04-160">JSON</span><span class="sxs-lookup"><span data-stu-id="0fd04-160">JSON</span></span>

<span data-ttu-id="0fd04-161">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="0fd04-161">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="0fd04-162">要求</span><span class="sxs-lookup"><span data-stu-id="0fd04-162">Request</span></span>

<span data-ttu-id="0fd04-163">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0fd04-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivitypages_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityPages(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="0fd04-164">応答</span><span class="sxs-lookup"><span data-stu-id="0fd04-164">Response</span></span>

<span data-ttu-id="0fd04-165">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0fd04-165">The following is an example of the response.</span></span>

> <span data-ttu-id="0fd04-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0fd04-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
