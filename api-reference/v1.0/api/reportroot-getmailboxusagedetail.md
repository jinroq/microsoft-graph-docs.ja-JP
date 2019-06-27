---
title: 'reportRoot: getMailboxUsageDetail'
description: メールボックスの使用状況に関する詳細を取得します。
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c7b29395486962d8387ffb438465c6f63adf9042
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268797"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="db89e-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="db89e-103">reportRoot: getMailboxUsageDetail</span></span>

<span data-ttu-id="db89e-104">メールボックスの使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="db89e-104">Get details about mailbox usage.</span></span>

> <span data-ttu-id="db89e-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メールボックスの使用状況](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="db89e-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="db89e-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="db89e-106">Permissions</span></span>

<span data-ttu-id="db89e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="db89e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="db89e-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="db89e-109">Permission type</span></span>                        | <span data-ttu-id="db89e-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="db89e-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="db89e-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="db89e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="db89e-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="db89e-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="db89e-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="db89e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db89e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="db89e-114">Not supported.</span></span>                           |
| <span data-ttu-id="db89e-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="db89e-115">Application</span></span>                            | <span data-ttu-id="db89e-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="db89e-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="db89e-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="db89e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="db89e-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="db89e-118">Function parameters</span></span>

<span data-ttu-id="db89e-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="db89e-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="db89e-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="db89e-120">Parameter</span></span> | <span data-ttu-id="db89e-121">型</span><span class="sxs-lookup"><span data-stu-id="db89e-121">Type</span></span>   | <span data-ttu-id="db89e-122">説明</span><span class="sxs-lookup"><span data-stu-id="db89e-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="db89e-123">period</span><span class="sxs-lookup"><span data-stu-id="db89e-123">period</span></span>    | <span data-ttu-id="db89e-124">文字列</span><span class="sxs-lookup"><span data-stu-id="db89e-124">string</span></span> | <span data-ttu-id="db89e-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="db89e-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="db89e-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="db89e-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="db89e-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="db89e-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="db89e-128">必須。</span><span class="sxs-lookup"><span data-stu-id="db89e-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="db89e-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="db89e-129">Request headers</span></span>

| <span data-ttu-id="db89e-130">名前</span><span class="sxs-lookup"><span data-stu-id="db89e-130">Name</span></span>          | <span data-ttu-id="db89e-131">説明</span><span class="sxs-lookup"><span data-stu-id="db89e-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="db89e-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="db89e-132">Authorization</span></span> | <span data-ttu-id="db89e-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="db89e-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="db89e-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="db89e-135">If-None-Match</span></span> | <span data-ttu-id="db89e-136">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="db89e-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="db89e-137">省略可能。</span><span class="sxs-lookup"><span data-stu-id="db89e-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="db89e-138">応答</span><span class="sxs-lookup"><span data-stu-id="db89e-138">Response</span></span>

<span data-ttu-id="db89e-139">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="db89e-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="db89e-140">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="db89e-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="db89e-141">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="db89e-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="db89e-142">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="db89e-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="db89e-143">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="db89e-143">Report Refresh Date</span></span>
- <span data-ttu-id="db89e-144">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="db89e-144">User Principal Name</span></span>
- <span data-ttu-id="db89e-145">表示名</span><span class="sxs-lookup"><span data-stu-id="db89e-145">Display Name</span></span>
- <span data-ttu-id="db89e-146">削除済み</span><span class="sxs-lookup"><span data-stu-id="db89e-146">Is Deleted</span></span>
- <span data-ttu-id="db89e-147">削除日</span><span class="sxs-lookup"><span data-stu-id="db89e-147">Deleted Date</span></span>
- <span data-ttu-id="db89e-148">作成日</span><span class="sxs-lookup"><span data-stu-id="db89e-148">Created Date</span></span>
- <span data-ttu-id="db89e-149">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="db89e-149">Last Activity Date</span></span>
- <span data-ttu-id="db89e-150">アイテム数</span><span class="sxs-lookup"><span data-stu-id="db89e-150">Item Count</span></span>
- <span data-ttu-id="db89e-151">使用済みストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="db89e-151">Storage Used (Byte)</span></span>
- <span data-ttu-id="db89e-152">警告表示クォータ (バイト)</span><span class="sxs-lookup"><span data-stu-id="db89e-152">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="db89e-153">送信禁止クォータ (バイト)</span><span class="sxs-lookup"><span data-stu-id="db89e-153">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="db89e-154">送受信禁止クォータ (バイト)</span><span class="sxs-lookup"><span data-stu-id="db89e-154">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="db89e-155">レポート期間</span><span class="sxs-lookup"><span data-stu-id="db89e-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="db89e-156">例</span><span class="sxs-lookup"><span data-stu-id="db89e-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="db89e-157">要求</span><span class="sxs-lookup"><span data-stu-id="db89e-157">Request</span></span>

<span data-ttu-id="db89e-158">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="db89e-158">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="db89e-159">応答</span><span class="sxs-lookup"><span data-stu-id="db89e-159">Response</span></span>

<span data-ttu-id="db89e-160">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="db89e-160">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="db89e-161">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="db89e-161">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="db89e-162">C#</span><span class="sxs-lookup"><span data-stu-id="db89e-162">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusageuserdetail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db89e-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="db89e-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusageuserdetail-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="db89e-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db89e-164">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusageuserdetail-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="db89e-165">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="db89e-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Created Date,Last Activity Date,Item Count,Storage Used (Byte),Issue Warning Quota (Byte),Prohibit Send Quota (Byte),Prohibit Send/Receive Quota (Byte),Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getmailboxusagedetail.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getmailboxusagedetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getmailboxusagedetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
