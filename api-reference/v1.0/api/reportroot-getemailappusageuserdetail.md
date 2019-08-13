---
title: 'reportRoot: getEmailAppUsageUserDetail'
description: メール アプリの各バージョンでユーザーが実行したアクティビティの詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 82b199177248dbfd459b4963b130e38d91f5e466
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327322"
---
# <a name="reportroot-getemailappusageuserdetail"></a><span data-ttu-id="11707-103">reportRoot: getEmailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="11707-103">reportRoot: getEmailAppUsageUserDetail</span></span>

<span data-ttu-id="11707-104">メール アプリの各バージョンでユーザーが実行したアクティビティの詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="11707-104">Get details about which activities users performed on the various email apps.</span></span>

> <span data-ttu-id="11707-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メール アプリの使用状況](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="11707-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="11707-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="11707-106">Permissions</span></span>

<span data-ttu-id="11707-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="11707-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="11707-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="11707-109">Permission type</span></span>                        | <span data-ttu-id="11707-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="11707-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="11707-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="11707-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="11707-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="11707-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="11707-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="11707-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11707-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11707-114">Not supported.</span></span>                           |
| <span data-ttu-id="11707-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="11707-115">Application</span></span>                            | <span data-ttu-id="11707-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="11707-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="11707-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="11707-117">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getEmailAppUsageUserDetail(period='{period_value}')
GET /reports/getEmailAppUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="11707-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="11707-118">Function parameters</span></span>

<span data-ttu-id="11707-119">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="11707-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="11707-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="11707-120">Parameter</span></span> | <span data-ttu-id="11707-121">型</span><span class="sxs-lookup"><span data-stu-id="11707-121">Type</span></span>   | <span data-ttu-id="11707-122">説明</span><span class="sxs-lookup"><span data-stu-id="11707-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="11707-123">period</span><span class="sxs-lookup"><span data-stu-id="11707-123">period</span></span>    | <span data-ttu-id="11707-124">文字列</span><span class="sxs-lookup"><span data-stu-id="11707-124">string</span></span> | <span data-ttu-id="11707-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="11707-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="11707-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="11707-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="11707-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="11707-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="11707-128">date</span><span class="sxs-lookup"><span data-stu-id="11707-128">date</span></span>      | <span data-ttu-id="11707-129">日付</span><span class="sxs-lookup"><span data-stu-id="11707-129">Date</span></span>   | <span data-ttu-id="11707-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="11707-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="11707-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="11707-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="11707-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="11707-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="11707-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="11707-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="11707-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="11707-134">Request headers</span></span>

| <span data-ttu-id="11707-135">名前</span><span class="sxs-lookup"><span data-stu-id="11707-135">Name</span></span>          | <span data-ttu-id="11707-136">説明</span><span class="sxs-lookup"><span data-stu-id="11707-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="11707-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="11707-137">Authorization</span></span> | <span data-ttu-id="11707-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="11707-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="11707-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="11707-140">If-None-Match</span></span> | <span data-ttu-id="11707-141">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="11707-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="11707-142">省略可能。</span><span class="sxs-lookup"><span data-stu-id="11707-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="11707-143">応答</span><span class="sxs-lookup"><span data-stu-id="11707-143">Response</span></span>

<span data-ttu-id="11707-144">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="11707-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="11707-145">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="11707-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="11707-146">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="11707-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="11707-147">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="11707-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="11707-148">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="11707-148">Report Refresh Date</span></span>
- <span data-ttu-id="11707-149">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="11707-149">User Principal Name</span></span>
- <span data-ttu-id="11707-150">表示名</span><span class="sxs-lookup"><span data-stu-id="11707-150">Display Name</span></span>
- <span data-ttu-id="11707-151">削除済み</span><span class="sxs-lookup"><span data-stu-id="11707-151">Is Deleted</span></span>
- <span data-ttu-id="11707-152">削除日</span><span class="sxs-lookup"><span data-stu-id="11707-152">Deleted Date</span></span>
- <span data-ttu-id="11707-153">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="11707-153">Last Activity Date</span></span>
- <span data-ttu-id="11707-154">Mail For Mac</span><span class="sxs-lookup"><span data-stu-id="11707-154">Mail For Mac</span></span>
- <span data-ttu-id="11707-155">Outlook For Mac</span><span class="sxs-lookup"><span data-stu-id="11707-155">Outlook For Mac</span></span>
- <span data-ttu-id="11707-156">Outlook For Windows</span><span class="sxs-lookup"><span data-stu-id="11707-156">Outlook For Windows</span></span>
- <span data-ttu-id="11707-157">Outlook For Mobile</span><span class="sxs-lookup"><span data-stu-id="11707-157">Outlook For Mobile</span></span>
- <span data-ttu-id="11707-158">Other For Mobile</span><span class="sxs-lookup"><span data-stu-id="11707-158">Other For Mobile</span></span>
- <span data-ttu-id="11707-159">Outlook For Web</span><span class="sxs-lookup"><span data-stu-id="11707-159">Outlook For Web</span></span>
- <span data-ttu-id="11707-160">POP3 アプリ</span><span class="sxs-lookup"><span data-stu-id="11707-160">POP3 App</span></span>
- <span data-ttu-id="11707-161">IMAP4 アプリ</span><span class="sxs-lookup"><span data-stu-id="11707-161">IMAP4 App</span></span>
- <span data-ttu-id="11707-162">SMTP アプリ</span><span class="sxs-lookup"><span data-stu-id="11707-162">SMTP App</span></span>
- <span data-ttu-id="11707-163">レポート期間</span><span class="sxs-lookup"><span data-stu-id="11707-163">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="11707-164">例</span><span class="sxs-lookup"><span data-stu-id="11707-164">Example</span></span>

#### <a name="request"></a><span data-ttu-id="11707-165">要求</span><span class="sxs-lookup"><span data-stu-id="11707-165">Request</span></span>

<span data-ttu-id="11707-166">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="11707-166">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="11707-167">プロトコル</span><span class="sxs-lookup"><span data-stu-id="11707-167">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailappusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="11707-168">C#</span><span class="sxs-lookup"><span data-stu-id="11707-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="11707-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11707-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="11707-170">目的-C</span><span class="sxs-lookup"><span data-stu-id="11707-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="11707-171">Java</span><span class="sxs-lookup"><span data-stu-id="11707-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getemailappusageuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="11707-172">応答</span><span class="sxs-lookup"><span data-stu-id="11707-172">Response</span></span>

<span data-ttu-id="11707-173">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="11707-173">The following is an example of the response.</span></span>

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

<span data-ttu-id="11707-174">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="11707-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Period
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
