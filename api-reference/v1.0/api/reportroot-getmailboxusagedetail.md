---
title: 'reportRoot: getMailboxUsageDetail'
description: メールボックスの使用状況に関する詳細を取得します。
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0ec06a813d0e7080c9b3b4f2ae8565bca9031e4a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448564"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="648e6-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="648e6-103">reportRoot: getMailboxUsageDetail</span></span>

<span data-ttu-id="648e6-104">メールボックスの使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="648e6-104">Get details about mailbox usage.</span></span>

> <span data-ttu-id="648e6-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メールボックスの使用状況](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="648e6-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="648e6-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="648e6-106">Permissions</span></span>

<span data-ttu-id="648e6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="648e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="648e6-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="648e6-109">Permission type</span></span>                        | <span data-ttu-id="648e6-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="648e6-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="648e6-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="648e6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="648e6-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="648e6-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="648e6-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="648e6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="648e6-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="648e6-114">Not supported.</span></span>                           |
| <span data-ttu-id="648e6-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="648e6-115">Application</span></span>                            | <span data-ttu-id="648e6-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="648e6-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="648e6-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="648e6-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="648e6-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="648e6-118">--Http</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="648e6-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="648e6-119">Function parameters</span></span>

<span data-ttu-id="648e6-120">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="648e6-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="648e6-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="648e6-121">Parameter</span></span> | <span data-ttu-id="648e6-122">型</span><span class="sxs-lookup"><span data-stu-id="648e6-122">Type</span></span>   | <span data-ttu-id="648e6-123">説明</span><span class="sxs-lookup"><span data-stu-id="648e6-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="648e6-124">period</span><span class="sxs-lookup"><span data-stu-id="648e6-124">period</span></span>    | <span data-ttu-id="648e6-125">文字列</span><span class="sxs-lookup"><span data-stu-id="648e6-125">string</span></span> | <span data-ttu-id="648e6-126">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="648e6-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="648e6-127">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="648e6-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="648e6-128">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="648e6-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="648e6-129">必須。</span><span class="sxs-lookup"><span data-stu-id="648e6-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="648e6-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="648e6-130">Request headers</span></span>

| <span data-ttu-id="648e6-131">名前</span><span class="sxs-lookup"><span data-stu-id="648e6-131">Name</span></span>          | <span data-ttu-id="648e6-132">説明</span><span class="sxs-lookup"><span data-stu-id="648e6-132">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="648e6-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="648e6-133">Authorization</span></span> | <span data-ttu-id="648e6-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="648e6-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="648e6-136">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="648e6-136">If-None-Match</span></span> | <span data-ttu-id="648e6-137">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="648e6-137">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="648e6-138">省略可能。</span><span class="sxs-lookup"><span data-stu-id="648e6-138">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="648e6-139">応答</span><span class="sxs-lookup"><span data-stu-id="648e6-139">Response</span></span>

<span data-ttu-id="648e6-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="648e6-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="648e6-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="648e6-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="648e6-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="648e6-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="648e6-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="648e6-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="648e6-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="648e6-144">Report Refresh Date</span></span>
- <span data-ttu-id="648e6-145">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="648e6-145">User Principal Name</span></span>
- <span data-ttu-id="648e6-146">表示名</span><span class="sxs-lookup"><span data-stu-id="648e6-146">Display Name</span></span>
- <span data-ttu-id="648e6-147">削除済み</span><span class="sxs-lookup"><span data-stu-id="648e6-147">Is Deleted</span></span>
- <span data-ttu-id="648e6-148">削除日</span><span class="sxs-lookup"><span data-stu-id="648e6-148">Deleted Date</span></span>
- <span data-ttu-id="648e6-149">作成日</span><span class="sxs-lookup"><span data-stu-id="648e6-149">Created Date</span></span>
- <span data-ttu-id="648e6-150">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="648e6-150">Last Activity Date</span></span>
- <span data-ttu-id="648e6-151">アイテム数</span><span class="sxs-lookup"><span data-stu-id="648e6-151">Item Count</span></span>
- <span data-ttu-id="648e6-152">使用済みストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="648e6-152">Storage Used (Byte)</span></span>
- <span data-ttu-id="648e6-153">警告表示クォータ (バイト)</span><span class="sxs-lookup"><span data-stu-id="648e6-153">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="648e6-154">送信禁止クォータ (バイト)</span><span class="sxs-lookup"><span data-stu-id="648e6-154">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="648e6-155">送受信禁止クォータ (バイト)</span><span class="sxs-lookup"><span data-stu-id="648e6-155">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="648e6-156">レポート期間</span><span class="sxs-lookup"><span data-stu-id="648e6-156">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="648e6-157">例</span><span class="sxs-lookup"><span data-stu-id="648e6-157">Example</span></span>

#### <a name="request"></a><span data-ttu-id="648e6-158">要求</span><span class="sxs-lookup"><span data-stu-id="648e6-158">Request</span></span>

<span data-ttu-id="648e6-159">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="648e6-159">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="648e6-160">C#</span><span class="sxs-lookup"><span data-stu-id="648e6-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="648e6-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="648e6-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="648e6-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="648e6-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="648e6-163">応答</span><span class="sxs-lookup"><span data-stu-id="648e6-163">Response</span></span>

<span data-ttu-id="648e6-164">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="648e6-164">The following is an example of the response.</span></span>

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

<span data-ttu-id="648e6-165">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="648e6-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
  ]
}-->
