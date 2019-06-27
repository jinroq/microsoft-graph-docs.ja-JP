---
title: 'reportRoot: getMailboxUsageMailboxCounts'
description: 組織内のユーザー メールボックスの合計数と、レポート期間中の各日にアクティブなメールボックス数を取得します。 メールボックスは、ユーザーが何らかの電子メールを送信するか、読んだ場合にアクティブとみなされます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: bc8e8ca23a8653cd47165faa78cdeb3975ee98ee
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268790"
---
# <a name="reportroot-getmailboxusagemailboxcounts"></a><span data-ttu-id="745b7-104">reportRoot: getMailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="745b7-104">reportRoot: getMailboxUsageMailboxCounts</span></span>

<span data-ttu-id="745b7-105">組織内のユーザー メールボックスの合計数と、レポート期間中の各日にアクティブなメールボックス数を取得します。</span><span class="sxs-lookup"><span data-stu-id="745b7-105">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="745b7-106">メールボックスは、ユーザーが何らかの電子メールを送信するか、読んだ場合にアクティブとみなされます。</span><span class="sxs-lookup"><span data-stu-id="745b7-106">A mailbox is considered active if the user sent or read any email.</span></span>

> <span data-ttu-id="745b7-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メールボックスの使用状況](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="745b7-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="745b7-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="745b7-108">Permissions</span></span>

<span data-ttu-id="745b7-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="745b7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="745b7-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="745b7-111">Permission type</span></span>                        | <span data-ttu-id="745b7-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="745b7-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="745b7-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="745b7-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="745b7-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="745b7-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="745b7-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="745b7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="745b7-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="745b7-116">Not supported.</span></span>                           |
| <span data-ttu-id="745b7-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="745b7-117">Application</span></span>                            | <span data-ttu-id="745b7-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="745b7-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="745b7-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="745b7-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="745b7-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="745b7-120">Function parameters</span></span>

<span data-ttu-id="745b7-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="745b7-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="745b7-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="745b7-122">Parameter</span></span> | <span data-ttu-id="745b7-123">型</span><span class="sxs-lookup"><span data-stu-id="745b7-123">Type</span></span>   | <span data-ttu-id="745b7-124">説明</span><span class="sxs-lookup"><span data-stu-id="745b7-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="745b7-125">period</span><span class="sxs-lookup"><span data-stu-id="745b7-125">period</span></span>    | <span data-ttu-id="745b7-126">文字列</span><span class="sxs-lookup"><span data-stu-id="745b7-126">string</span></span> | <span data-ttu-id="745b7-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="745b7-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="745b7-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="745b7-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="745b7-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="745b7-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="745b7-130">必須。</span><span class="sxs-lookup"><span data-stu-id="745b7-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="745b7-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="745b7-131">Request headers</span></span>

| <span data-ttu-id="745b7-132">名前</span><span class="sxs-lookup"><span data-stu-id="745b7-132">Name</span></span>          | <span data-ttu-id="745b7-133">説明</span><span class="sxs-lookup"><span data-stu-id="745b7-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="745b7-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="745b7-134">Authorization</span></span> | <span data-ttu-id="745b7-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="745b7-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="745b7-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="745b7-137">If-None-Match</span></span> | <span data-ttu-id="745b7-138">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="745b7-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="745b7-139">省略可能。</span><span class="sxs-lookup"><span data-stu-id="745b7-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="745b7-140">応答</span><span class="sxs-lookup"><span data-stu-id="745b7-140">Response</span></span>

<span data-ttu-id="745b7-141">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="745b7-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="745b7-142">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="745b7-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="745b7-143">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="745b7-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="745b7-144">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="745b7-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="745b7-145">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="745b7-145">Report Refresh Date</span></span>
- <span data-ttu-id="745b7-146">合計</span><span class="sxs-lookup"><span data-stu-id="745b7-146">Total</span></span>
- <span data-ttu-id="745b7-147">アクティブ</span><span class="sxs-lookup"><span data-stu-id="745b7-147">Active</span></span>
- <span data-ttu-id="745b7-148">レポート日付</span><span class="sxs-lookup"><span data-stu-id="745b7-148">Report Date</span></span>
- <span data-ttu-id="745b7-149">レポート期間</span><span class="sxs-lookup"><span data-stu-id="745b7-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="745b7-150">例</span><span class="sxs-lookup"><span data-stu-id="745b7-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="745b7-151">要求</span><span class="sxs-lookup"><span data-stu-id="745b7-151">Request</span></span>

<span data-ttu-id="745b7-152">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="745b7-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusagemailboxcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageMailboxCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="745b7-153">応答</span><span class="sxs-lookup"><span data-stu-id="745b7-153">Response</span></span>

<span data-ttu-id="745b7-154">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="745b7-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="745b7-155">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="745b7-155">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="745b7-156">C#</span><span class="sxs-lookup"><span data-stu-id="745b7-156">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusagemailboxcounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="745b7-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="745b7-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusagemailboxcounts-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="745b7-158">目的-C</span><span class="sxs-lookup"><span data-stu-id="745b7-158">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusagemailboxcounts-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="745b7-159">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="745b7-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getmailboxusagemailboxcounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getmailboxusagemailboxcounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getmailboxusagemailboxcounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
