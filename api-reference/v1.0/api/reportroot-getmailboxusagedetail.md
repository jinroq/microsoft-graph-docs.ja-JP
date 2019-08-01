---
title: 'reportRoot: getMailboxUsageDetail'
description: メールボックスの使用状況に関する詳細を取得します。
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: fb297d3be564a585a5346961aa6e39169cf61b92
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025135"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="378c7-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="378c7-103">reportRoot: getMailboxUsageDetail</span></span>

<span data-ttu-id="378c7-104">メールボックスの使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="378c7-104">Get details about mailbox usage.</span></span>

> <span data-ttu-id="378c7-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メールボックスの使用状況](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="378c7-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="378c7-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="378c7-106">Permissions</span></span>

<span data-ttu-id="378c7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="378c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="378c7-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="378c7-109">Permission type</span></span>                        | <span data-ttu-id="378c7-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="378c7-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="378c7-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="378c7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="378c7-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="378c7-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="378c7-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="378c7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="378c7-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="378c7-114">Not supported.</span></span>                           |
| <span data-ttu-id="378c7-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="378c7-115">Application</span></span>                            | <span data-ttu-id="378c7-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="378c7-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="378c7-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="378c7-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="378c7-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="378c7-118">--Http</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="378c7-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="378c7-119">Function parameters</span></span>

<span data-ttu-id="378c7-120">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="378c7-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="378c7-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="378c7-121">Parameter</span></span> | <span data-ttu-id="378c7-122">型</span><span class="sxs-lookup"><span data-stu-id="378c7-122">Type</span></span>   | <span data-ttu-id="378c7-123">説明</span><span class="sxs-lookup"><span data-stu-id="378c7-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="378c7-124">period</span><span class="sxs-lookup"><span data-stu-id="378c7-124">period</span></span>    | <span data-ttu-id="378c7-125">文字列</span><span class="sxs-lookup"><span data-stu-id="378c7-125">string</span></span> | <span data-ttu-id="378c7-126">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="378c7-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="378c7-127">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="378c7-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="378c7-128">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="378c7-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="378c7-129">必須。</span><span class="sxs-lookup"><span data-stu-id="378c7-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="378c7-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="378c7-130">Request headers</span></span>

| <span data-ttu-id="378c7-131">名前</span><span class="sxs-lookup"><span data-stu-id="378c7-131">Name</span></span>          | <span data-ttu-id="378c7-132">説明</span><span class="sxs-lookup"><span data-stu-id="378c7-132">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="378c7-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="378c7-133">Authorization</span></span> | <span data-ttu-id="378c7-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="378c7-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="378c7-136">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="378c7-136">If-None-Match</span></span> | <span data-ttu-id="378c7-137">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="378c7-137">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="378c7-138">省略可能。</span><span class="sxs-lookup"><span data-stu-id="378c7-138">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="378c7-139">応答</span><span class="sxs-lookup"><span data-stu-id="378c7-139">Response</span></span>

<span data-ttu-id="378c7-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="378c7-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="378c7-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="378c7-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="378c7-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="378c7-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="378c7-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="378c7-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="378c7-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="378c7-144">Report Refresh Date</span></span>
- <span data-ttu-id="378c7-145">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="378c7-145">User Principal Name</span></span>
- <span data-ttu-id="378c7-146">表示名</span><span class="sxs-lookup"><span data-stu-id="378c7-146">Display Name</span></span>
- <span data-ttu-id="378c7-147">削除済み</span><span class="sxs-lookup"><span data-stu-id="378c7-147">Is Deleted</span></span>
- <span data-ttu-id="378c7-148">削除日</span><span class="sxs-lookup"><span data-stu-id="378c7-148">Deleted Date</span></span>
- <span data-ttu-id="378c7-149">作成日</span><span class="sxs-lookup"><span data-stu-id="378c7-149">Created Date</span></span>
- <span data-ttu-id="378c7-150">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="378c7-150">Last Activity Date</span></span>
- <span data-ttu-id="378c7-151">アイテム数</span><span class="sxs-lookup"><span data-stu-id="378c7-151">Item Count</span></span>
- <span data-ttu-id="378c7-152">使用済みストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="378c7-152">Storage Used (Byte)</span></span>
- <span data-ttu-id="378c7-153">警告表示クォータ (バイト)</span><span class="sxs-lookup"><span data-stu-id="378c7-153">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="378c7-154">送信禁止クォータ (バイト)</span><span class="sxs-lookup"><span data-stu-id="378c7-154">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="378c7-155">送受信禁止クォータ (バイト)</span><span class="sxs-lookup"><span data-stu-id="378c7-155">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="378c7-156">レポート期間</span><span class="sxs-lookup"><span data-stu-id="378c7-156">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="378c7-157">例</span><span class="sxs-lookup"><span data-stu-id="378c7-157">Example</span></span>

#### <a name="request"></a><span data-ttu-id="378c7-158">要求</span><span class="sxs-lookup"><span data-stu-id="378c7-158">Request</span></span>

<span data-ttu-id="378c7-159">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="378c7-159">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="378c7-160">C#</span><span class="sxs-lookup"><span data-stu-id="378c7-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="378c7-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="378c7-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="378c7-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="378c7-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="378c7-163">Java</span><span class="sxs-lookup"><span data-stu-id="378c7-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusageuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="378c7-164">応答</span><span class="sxs-lookup"><span data-stu-id="378c7-164">Response</span></span>

<span data-ttu-id="378c7-165">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="378c7-165">The following is an example of the response.</span></span>

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

<span data-ttu-id="378c7-166">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="378c7-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
