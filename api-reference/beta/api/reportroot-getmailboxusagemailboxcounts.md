---
title: 'reportRoot: getMailboxUsageMailboxCounts'
description: 組織内のユーザー メールボックスの合計数と、レポート期間中の各日にアクティブなメールボックス数を取得します。 メールボックスは、ユーザーが何らかの電子メールを送信するか、読んだ場合にアクティブとみなされます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e181141ce1058489a6bbb254923bbde3110e2bfc
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331688"
---
# <a name="reportroot-getmailboxusagemailboxcounts"></a><span data-ttu-id="a2853-104">reportRoot: getMailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="a2853-104">reportRoot: getMailboxUsageMailboxCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2853-105">組織内のユーザー メールボックスの合計数と、レポート期間中の各日にアクティブなメールボックス数を取得します。</span><span class="sxs-lookup"><span data-stu-id="a2853-105">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="a2853-106">メールボックスは、ユーザーが何らかの電子メールを送信するか、読んだ場合にアクティブとみなされます。</span><span class="sxs-lookup"><span data-stu-id="a2853-106">A mailbox is considered active if the user sent or read any email.</span></span>

> <span data-ttu-id="a2853-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メールボックスの使用状況](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2853-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="a2853-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a2853-108">Permissions</span></span>

<span data-ttu-id="a2853-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2853-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a2853-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a2853-111">Permission type</span></span>                        | <span data-ttu-id="a2853-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a2853-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a2853-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="a2853-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="a2853-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2853-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a2853-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a2853-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2853-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2853-116">Not supported.</span></span>                           |
| <span data-ttu-id="a2853-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a2853-117">Application</span></span>                            | <span data-ttu-id="a2853-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2853-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a2853-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a2853-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a2853-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="a2853-120">Function parameters</span></span>

<span data-ttu-id="a2853-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="a2853-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a2853-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="a2853-122">Parameter</span></span> | <span data-ttu-id="a2853-123">型</span><span class="sxs-lookup"><span data-stu-id="a2853-123">Type</span></span>   | <span data-ttu-id="a2853-124">説明</span><span class="sxs-lookup"><span data-stu-id="a2853-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a2853-125">period</span><span class="sxs-lookup"><span data-stu-id="a2853-125">period</span></span>    | <span data-ttu-id="a2853-126">文字列</span><span class="sxs-lookup"><span data-stu-id="a2853-126">string</span></span> | <span data-ttu-id="a2853-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="a2853-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a2853-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="a2853-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a2853-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="a2853-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a2853-130">必須。</span><span class="sxs-lookup"><span data-stu-id="a2853-130">Required.</span></span> |

<span data-ttu-id="a2853-131">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a2853-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a2853-132">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="a2853-132">The default output type is text/csv.</span></span> <span data-ttu-id="a2853-133">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="a2853-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2853-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2853-134">Request headers</span></span>

| <span data-ttu-id="a2853-135">名前</span><span class="sxs-lookup"><span data-stu-id="a2853-135">Name</span></span>          | <span data-ttu-id="a2853-136">説明</span><span class="sxs-lookup"><span data-stu-id="a2853-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a2853-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2853-137">Authorization</span></span> | <span data-ttu-id="a2853-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a2853-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a2853-140">応答</span><span class="sxs-lookup"><span data-stu-id="a2853-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a2853-141">CSV</span><span class="sxs-lookup"><span data-stu-id="a2853-141">CSV</span></span>

<span data-ttu-id="a2853-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="a2853-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a2853-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="a2853-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a2853-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="a2853-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a2853-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="a2853-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a2853-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="a2853-146">Report Refresh Date</span></span>
- <span data-ttu-id="a2853-147">合計</span><span class="sxs-lookup"><span data-stu-id="a2853-147">Total</span></span>
- <span data-ttu-id="a2853-148">アクティブ</span><span class="sxs-lookup"><span data-stu-id="a2853-148">Active</span></span>
- <span data-ttu-id="a2853-149">レポート日付</span><span class="sxs-lookup"><span data-stu-id="a2853-149">Report Date</span></span>
- <span data-ttu-id="a2853-150">レポート期間</span><span class="sxs-lookup"><span data-stu-id="a2853-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="a2853-151">JSON</span><span class="sxs-lookup"><span data-stu-id="a2853-151">JSON</span></span>

<span data-ttu-id="a2853-152">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a2853-152">If successful, this method returns a `200 OK` response code and a **[mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2853-153">例</span><span class="sxs-lookup"><span data-stu-id="a2853-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a2853-154">CSV</span><span class="sxs-lookup"><span data-stu-id="a2853-154">CSV</span></span>

<span data-ttu-id="a2853-155">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a2853-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a2853-156">要求</span><span class="sxs-lookup"><span data-stu-id="a2853-156">Request</span></span>

<span data-ttu-id="a2853-157">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a2853-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagemailboxcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageMailboxCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="a2853-158">応答</span><span class="sxs-lookup"><span data-stu-id="a2853-158">Response</span></span>

<span data-ttu-id="a2853-159">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a2853-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a2853-160">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="a2853-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="a2853-161">JSON</span><span class="sxs-lookup"><span data-stu-id="a2853-161">JSON</span></span>

<span data-ttu-id="a2853-162">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="a2853-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a2853-163">要求</span><span class="sxs-lookup"><span data-stu-id="a2853-163">Request</span></span>

<span data-ttu-id="a2853-164">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a2853-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagemailboxcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageMailboxCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="a2853-165">応答</span><span class="sxs-lookup"><span data-stu-id="a2853-165">Response</span></span>

<span data-ttu-id="a2853-166">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a2853-166">The following is an example of the response.</span></span>

> <span data-ttu-id="a2853-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a2853-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxUsageMailboxCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 232

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.mailboxUsageMailboxCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "total": 202, 
      "active": 198, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
