---
title: 'reportRoot: getMailboxUsageQuotaStatusMailboxCounts'
description: 各クォータ カテゴリのユーザーのメールボックス数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: da947184ece4be0015829f19243753bd39695745
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574825"
---
# <a name="reportroot-getmailboxusagequotastatusmailboxcounts"></a><span data-ttu-id="f2e95-103">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="f2e95-103">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span></span>

<span data-ttu-id="f2e95-104">各クォータ カテゴリのユーザーのメールボックス数を取得します。</span><span class="sxs-lookup"><span data-stu-id="f2e95-104">Get the count of user mailboxes in each quota category.</span></span>

> <span data-ttu-id="f2e95-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メールボックスの使用状況](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f2e95-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="f2e95-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f2e95-106">Permissions</span></span>

<span data-ttu-id="f2e95-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f2e95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f2e95-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f2e95-109">Permission type</span></span>                        | <span data-ttu-id="f2e95-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f2e95-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f2e95-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="f2e95-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f2e95-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2e95-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f2e95-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f2e95-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2e95-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2e95-114">Not supported.</span></span>                           |
| <span data-ttu-id="f2e95-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f2e95-115">Application</span></span>                            | <span data-ttu-id="f2e95-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2e95-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f2e95-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f2e95-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageQuotaStatusMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f2e95-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="f2e95-118">Function parameters</span></span>

<span data-ttu-id="f2e95-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="f2e95-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f2e95-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f2e95-120">Parameter</span></span> | <span data-ttu-id="f2e95-121">型</span><span class="sxs-lookup"><span data-stu-id="f2e95-121">Type</span></span>   | <span data-ttu-id="f2e95-122">説明</span><span class="sxs-lookup"><span data-stu-id="f2e95-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f2e95-123">period</span><span class="sxs-lookup"><span data-stu-id="f2e95-123">period</span></span>    | <span data-ttu-id="f2e95-124">文字列</span><span class="sxs-lookup"><span data-stu-id="f2e95-124">string</span></span> | <span data-ttu-id="f2e95-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="f2e95-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f2e95-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="f2e95-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f2e95-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="f2e95-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f2e95-128">必須。</span><span class="sxs-lookup"><span data-stu-id="f2e95-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f2e95-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f2e95-129">Request headers</span></span>

| <span data-ttu-id="f2e95-130">名前</span><span class="sxs-lookup"><span data-stu-id="f2e95-130">Name</span></span>          | <span data-ttu-id="f2e95-131">説明</span><span class="sxs-lookup"><span data-stu-id="f2e95-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="f2e95-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2e95-132">Authorization</span></span> | <span data-ttu-id="f2e95-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f2e95-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="f2e95-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="f2e95-135">If-None-Match</span></span> | <span data-ttu-id="f2e95-136">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="f2e95-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="f2e95-137">省略可能。</span><span class="sxs-lookup"><span data-stu-id="f2e95-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="f2e95-138">応答</span><span class="sxs-lookup"><span data-stu-id="f2e95-138">Response</span></span>

<span data-ttu-id="f2e95-139">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="f2e95-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f2e95-140">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="f2e95-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f2e95-141">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="f2e95-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f2e95-142">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="f2e95-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f2e95-143">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="f2e95-143">Report Refresh Date</span></span>
- <span data-ttu-id="f2e95-144">制限下</span><span class="sxs-lookup"><span data-stu-id="f2e95-144">Under Limit</span></span>
- <span data-ttu-id="f2e95-145">警告を発行</span><span class="sxs-lookup"><span data-stu-id="f2e95-145">Warning Issued</span></span>
- <span data-ttu-id="f2e95-146">送信禁止</span><span class="sxs-lookup"><span data-stu-id="f2e95-146">Send Prohibited</span></span>
- <span data-ttu-id="f2e95-147">送受信禁止</span><span class="sxs-lookup"><span data-stu-id="f2e95-147">Send/Receive Prohibited</span></span>
- <span data-ttu-id="f2e95-148">中間</span><span class="sxs-lookup"><span data-stu-id="f2e95-148">Indeterminate</span></span>
- <span data-ttu-id="f2e95-149">レポート日付</span><span class="sxs-lookup"><span data-stu-id="f2e95-149">Report Date</span></span>
- <span data-ttu-id="f2e95-150">レポート期間</span><span class="sxs-lookup"><span data-stu-id="f2e95-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="f2e95-151">例</span><span class="sxs-lookup"><span data-stu-id="f2e95-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f2e95-152">要求</span><span class="sxs-lookup"><span data-stu-id="f2e95-152">Request</span></span>

<span data-ttu-id="f2e95-153">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f2e95-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusagequotastatusmailboxcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageQuotaStatusMailboxCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="f2e95-154">応答</span><span class="sxs-lookup"><span data-stu-id="f2e95-154">Response</span></span>

<span data-ttu-id="f2e95-155">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f2e95-155">The following is an example of the response.</span></span>

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

<span data-ttu-id="f2e95-156">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="f2e95-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Under Limit,Warning Issued,Send Prohibited,Send/Receive Prohibited,Indeterminate,Report Date,Report Period
```
