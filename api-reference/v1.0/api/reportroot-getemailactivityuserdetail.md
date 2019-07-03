---
title: 'reportRoot: getEmailActivityUserDetail'
description: ユーザーが実行した電子メール アクティビティに関する詳細を取得します。
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 7738e797ec625e49278705292358f8cbffe69823
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449443"
---
# <a name="reportroot-getemailactivityuserdetail"></a><span data-ttu-id="55e4d-103">reportRoot: getEmailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="55e4d-103">reportRoot: getEmailActivityUserDetail</span></span>

<span data-ttu-id="55e4d-104">ユーザーが実行した電子メール アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="55e4d-104">Get details about email activity users have performed.</span></span>

> <span data-ttu-id="55e4d-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: 電子メール アクティビティ](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="55e4d-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="55e4d-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="55e4d-106">Permissions</span></span>

<span data-ttu-id="55e4d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="55e4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="55e4d-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="55e4d-109">Permission type</span></span>                        | <span data-ttu-id="55e4d-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="55e4d-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="55e4d-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="55e4d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="55e4d-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="55e4d-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="55e4d-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="55e4d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55e4d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="55e4d-114">Not supported.</span></span>                           |
| <span data-ttu-id="55e4d-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="55e4d-115">Application</span></span>                            | <span data-ttu-id="55e4d-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="55e4d-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="55e4d-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="55e4d-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="55e4d-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="55e4d-118">--Http</span></span>](#tab/http)
<!-- { "blockType": "samples" } --> 

```http
GET /reports/getEmailActivityUserDetail(period='{period_value}')
GET /reports/getEmailActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="55e4d-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="55e4d-119">Function parameters</span></span>

<span data-ttu-id="55e4d-120">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="55e4d-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="55e4d-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="55e4d-121">Parameter</span></span> | <span data-ttu-id="55e4d-122">型</span><span class="sxs-lookup"><span data-stu-id="55e4d-122">Type</span></span>   | <span data-ttu-id="55e4d-123">説明</span><span class="sxs-lookup"><span data-stu-id="55e4d-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="55e4d-124">period</span><span class="sxs-lookup"><span data-stu-id="55e4d-124">period</span></span>    | <span data-ttu-id="55e4d-125">文字列</span><span class="sxs-lookup"><span data-stu-id="55e4d-125">string</span></span> | <span data-ttu-id="55e4d-126">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="55e4d-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="55e4d-127">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="55e4d-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="55e4d-128">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="55e4d-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="55e4d-129">date</span><span class="sxs-lookup"><span data-stu-id="55e4d-129">date</span></span>      | <span data-ttu-id="55e4d-130">日付</span><span class="sxs-lookup"><span data-stu-id="55e4d-130">Date</span></span>   | <span data-ttu-id="55e4d-131">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="55e4d-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="55e4d-132">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="55e4d-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="55e4d-133">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="55e4d-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="55e4d-134">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="55e4d-134">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="55e4d-135">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="55e4d-135">Request headers</span></span>

| <span data-ttu-id="55e4d-136">名前</span><span class="sxs-lookup"><span data-stu-id="55e4d-136">Name</span></span>          | <span data-ttu-id="55e4d-137">説明</span><span class="sxs-lookup"><span data-stu-id="55e4d-137">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="55e4d-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="55e4d-138">Authorization</span></span> | <span data-ttu-id="55e4d-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="55e4d-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="55e4d-141">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="55e4d-141">If-None-Match</span></span> | <span data-ttu-id="55e4d-142">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="55e4d-142">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="55e4d-143">省略可能。</span><span class="sxs-lookup"><span data-stu-id="55e4d-143">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="55e4d-144">応答</span><span class="sxs-lookup"><span data-stu-id="55e4d-144">Response</span></span>

<span data-ttu-id="55e4d-145">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="55e4d-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="55e4d-146">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="55e4d-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="55e4d-147">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="55e4d-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="55e4d-148">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="55e4d-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="55e4d-149">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="55e4d-149">Report Refresh Date</span></span>
- <span data-ttu-id="55e4d-150">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="55e4d-150">User Principal Name</span></span>
- <span data-ttu-id="55e4d-151">表示名</span><span class="sxs-lookup"><span data-stu-id="55e4d-151">Display Name</span></span>
- <span data-ttu-id="55e4d-152">削除済み</span><span class="sxs-lookup"><span data-stu-id="55e4d-152">Is Deleted</span></span>
- <span data-ttu-id="55e4d-153">削除日</span><span class="sxs-lookup"><span data-stu-id="55e4d-153">Deleted Date</span></span>
- <span data-ttu-id="55e4d-154">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="55e4d-154">Last Activity Date</span></span>
- <span data-ttu-id="55e4d-155">送信数</span><span class="sxs-lookup"><span data-stu-id="55e4d-155">Send Count</span></span>
- <span data-ttu-id="55e4d-156">受信数</span><span class="sxs-lookup"><span data-stu-id="55e4d-156">Receive Count</span></span>
- <span data-ttu-id="55e4d-157">読み取り数</span><span class="sxs-lookup"><span data-stu-id="55e4d-157">Read Count</span></span>
- <span data-ttu-id="55e4d-158">割り当て済み製品</span><span class="sxs-lookup"><span data-stu-id="55e4d-158">Assigned Products</span></span>
- <span data-ttu-id="55e4d-159">レポート期間</span><span class="sxs-lookup"><span data-stu-id="55e4d-159">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="55e4d-160">例</span><span class="sxs-lookup"><span data-stu-id="55e4d-160">Example</span></span>

#### <a name="request"></a><span data-ttu-id="55e4d-161">要求</span><span class="sxs-lookup"><span data-stu-id="55e4d-161">Request</span></span>

<span data-ttu-id="55e4d-162">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="55e4d-162">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailActivityUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="55e4d-163">C#</span><span class="sxs-lookup"><span data-stu-id="55e4d-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailactivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="55e4d-164">Javascript</span><span class="sxs-lookup"><span data-stu-id="55e4d-164">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailactivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="55e4d-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55e4d-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailactivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="55e4d-166">応答</span><span class="sxs-lookup"><span data-stu-id="55e4d-166">Response</span></span>

<span data-ttu-id="55e4d-167">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="55e4d-167">The following is an example of the response.</span></span>

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

<span data-ttu-id="55e4d-168">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="55e4d-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Send Count,Receive Count,Read Count,Assigned Products,Report Period
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
