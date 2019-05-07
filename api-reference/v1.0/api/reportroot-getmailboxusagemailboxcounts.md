---
title: 'reportRoot: getMailboxUsageMailboxCounts'
description: 組織内のユーザー メールボックスの合計数と、レポート期間中の各日にアクティブなメールボックス数を取得します。 メールボックスは、ユーザーが何らかの電子メールを送信するか、読んだ場合にアクティブとみなされます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 54b0c53737b5319bdfce776fc780b3168de4e8b1
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33607063"
---
# <a name="reportroot-getmailboxusagemailboxcounts"></a><span data-ttu-id="5e484-104">reportRoot: getMailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="5e484-104">reportRoot: getMailboxUsageMailboxCounts</span></span>

<span data-ttu-id="5e484-105">組織内のユーザー メールボックスの合計数と、レポート期間中の各日にアクティブなメールボックス数を取得します。</span><span class="sxs-lookup"><span data-stu-id="5e484-105">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="5e484-106">メールボックスは、ユーザーが何らかの電子メールを送信するか、読んだ場合にアクティブとみなされます。</span><span class="sxs-lookup"><span data-stu-id="5e484-106">A mailbox is considered active if the user sent or read any email.</span></span>

> <span data-ttu-id="5e484-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メールボックスの使用状況](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5e484-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="5e484-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5e484-108">Permissions</span></span>

<span data-ttu-id="5e484-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5e484-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5e484-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5e484-111">Permission type</span></span>                        | <span data-ttu-id="5e484-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5e484-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5e484-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="5e484-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="5e484-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e484-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5e484-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5e484-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e484-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5e484-116">Not supported.</span></span>                           |
| <span data-ttu-id="5e484-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5e484-117">Application</span></span>                            | <span data-ttu-id="5e484-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e484-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5e484-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5e484-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="5e484-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="5e484-120">Function parameters</span></span>

<span data-ttu-id="5e484-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="5e484-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5e484-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="5e484-122">Parameter</span></span> | <span data-ttu-id="5e484-123">型</span><span class="sxs-lookup"><span data-stu-id="5e484-123">Type</span></span>   | <span data-ttu-id="5e484-124">説明</span><span class="sxs-lookup"><span data-stu-id="5e484-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5e484-125">period</span><span class="sxs-lookup"><span data-stu-id="5e484-125">period</span></span>    | <span data-ttu-id="5e484-126">文字列</span><span class="sxs-lookup"><span data-stu-id="5e484-126">string</span></span> | <span data-ttu-id="5e484-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="5e484-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5e484-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="5e484-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5e484-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="5e484-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5e484-130">必須。</span><span class="sxs-lookup"><span data-stu-id="5e484-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="5e484-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5e484-131">Request headers</span></span>

| <span data-ttu-id="5e484-132">名前</span><span class="sxs-lookup"><span data-stu-id="5e484-132">Name</span></span>          | <span data-ttu-id="5e484-133">説明</span><span class="sxs-lookup"><span data-stu-id="5e484-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="5e484-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e484-134">Authorization</span></span> | <span data-ttu-id="5e484-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5e484-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="5e484-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="5e484-137">If-None-Match</span></span> | <span data-ttu-id="5e484-138">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="5e484-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="5e484-139">省略可能。</span><span class="sxs-lookup"><span data-stu-id="5e484-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="5e484-140">応答</span><span class="sxs-lookup"><span data-stu-id="5e484-140">Response</span></span>

<span data-ttu-id="5e484-141">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="5e484-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5e484-142">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="5e484-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5e484-143">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="5e484-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5e484-144">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="5e484-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5e484-145">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="5e484-145">Report Refresh Date</span></span>
- <span data-ttu-id="5e484-146">合計</span><span class="sxs-lookup"><span data-stu-id="5e484-146">Total</span></span>
- <span data-ttu-id="5e484-147">アクティブ</span><span class="sxs-lookup"><span data-stu-id="5e484-147">Active</span></span>
- <span data-ttu-id="5e484-148">レポート日付</span><span class="sxs-lookup"><span data-stu-id="5e484-148">Report Date</span></span>
- <span data-ttu-id="5e484-149">レポート期間</span><span class="sxs-lookup"><span data-stu-id="5e484-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="5e484-150">例</span><span class="sxs-lookup"><span data-stu-id="5e484-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5e484-151">要求</span><span class="sxs-lookup"><span data-stu-id="5e484-151">Request</span></span>

<span data-ttu-id="5e484-152">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5e484-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusagemailboxcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageMailboxCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="5e484-153">応答</span><span class="sxs-lookup"><span data-stu-id="5e484-153">Response</span></span>

<span data-ttu-id="5e484-154">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5e484-154">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5e484-155">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="5e484-155">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5e484-156">Visual</span><span class="sxs-lookup"><span data-stu-id="5e484-156">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusagemailboxcounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5e484-157">Java</span><span class="sxs-lookup"><span data-stu-id="5e484-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusagemailboxcounts-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="5e484-158">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="5e484-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
    "Error: /api-reference/v1.0/api/reportroot-getmailboxusagemailboxcounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getmailboxusagemailboxcounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
