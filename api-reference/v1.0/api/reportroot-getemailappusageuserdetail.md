---
title: 'reportRoot: getEmailAppUsageUserDetail'
description: メール アプリの各バージョンでユーザーが実行したアクティビティの詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: bde1a3de90796dda65fc9d227fe0432df2ded47c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449422"
---
# <a name="reportroot-getemailappusageuserdetail"></a><span data-ttu-id="b7f25-103">reportRoot: getEmailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="b7f25-103">reportRoot: getEmailAppUsageUserDetail</span></span>

<span data-ttu-id="b7f25-104">メール アプリの各バージョンでユーザーが実行したアクティビティの詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="b7f25-104">Get details about which activities users performed on the various email apps.</span></span>

> <span data-ttu-id="b7f25-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メール アプリの使用状況](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b7f25-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="b7f25-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b7f25-106">Permissions</span></span>

<span data-ttu-id="b7f25-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b7f25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b7f25-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b7f25-109">Permission type</span></span>                        | <span data-ttu-id="b7f25-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b7f25-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b7f25-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="b7f25-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b7f25-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7f25-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b7f25-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b7f25-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7f25-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7f25-114">Not supported.</span></span>                           |
| <span data-ttu-id="b7f25-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b7f25-115">Application</span></span>                            | <span data-ttu-id="b7f25-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7f25-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b7f25-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b7f25-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b7f25-118">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b7f25-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "samples" } --> 

```http
GET /reports/getEmailAppUsageUserDetail(period='{period_value}')
GET /reports/getEmailAppUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="b7f25-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="b7f25-119">Function parameters</span></span>

<span data-ttu-id="b7f25-120">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="b7f25-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="b7f25-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b7f25-121">Parameter</span></span> | <span data-ttu-id="b7f25-122">型</span><span class="sxs-lookup"><span data-stu-id="b7f25-122">Type</span></span>   | <span data-ttu-id="b7f25-123">説明</span><span class="sxs-lookup"><span data-stu-id="b7f25-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b7f25-124">period</span><span class="sxs-lookup"><span data-stu-id="b7f25-124">period</span></span>    | <span data-ttu-id="b7f25-125">文字列</span><span class="sxs-lookup"><span data-stu-id="b7f25-125">string</span></span> | <span data-ttu-id="b7f25-126">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="b7f25-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b7f25-127">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="b7f25-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b7f25-128">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="b7f25-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="b7f25-129">date</span><span class="sxs-lookup"><span data-stu-id="b7f25-129">date</span></span>      | <span data-ttu-id="b7f25-130">日付</span><span class="sxs-lookup"><span data-stu-id="b7f25-130">Date</span></span>   | <span data-ttu-id="b7f25-131">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="b7f25-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="b7f25-132">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="b7f25-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="b7f25-133">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="b7f25-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="b7f25-134">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b7f25-134">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b7f25-135">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b7f25-135">Request headers</span></span>

| <span data-ttu-id="b7f25-136">名前</span><span class="sxs-lookup"><span data-stu-id="b7f25-136">Name</span></span>          | <span data-ttu-id="b7f25-137">説明</span><span class="sxs-lookup"><span data-stu-id="b7f25-137">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="b7f25-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7f25-138">Authorization</span></span> | <span data-ttu-id="b7f25-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b7f25-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="b7f25-141">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="b7f25-141">If-None-Match</span></span> | <span data-ttu-id="b7f25-142">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="b7f25-142">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="b7f25-143">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b7f25-143">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="b7f25-144">応答</span><span class="sxs-lookup"><span data-stu-id="b7f25-144">Response</span></span>

<span data-ttu-id="b7f25-145">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="b7f25-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b7f25-146">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="b7f25-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b7f25-147">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="b7f25-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b7f25-148">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="b7f25-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b7f25-149">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="b7f25-149">Report Refresh Date</span></span>
- <span data-ttu-id="b7f25-150">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="b7f25-150">User Principal Name</span></span>
- <span data-ttu-id="b7f25-151">表示名</span><span class="sxs-lookup"><span data-stu-id="b7f25-151">Display Name</span></span>
- <span data-ttu-id="b7f25-152">削除済み</span><span class="sxs-lookup"><span data-stu-id="b7f25-152">Is Deleted</span></span>
- <span data-ttu-id="b7f25-153">削除日</span><span class="sxs-lookup"><span data-stu-id="b7f25-153">Deleted Date</span></span>
- <span data-ttu-id="b7f25-154">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="b7f25-154">Last Activity Date</span></span>
- <span data-ttu-id="b7f25-155">Mail For Mac</span><span class="sxs-lookup"><span data-stu-id="b7f25-155">Mail For Mac</span></span>
- <span data-ttu-id="b7f25-156">Outlook For Mac</span><span class="sxs-lookup"><span data-stu-id="b7f25-156">Outlook For Mac</span></span>
- <span data-ttu-id="b7f25-157">Outlook For Windows</span><span class="sxs-lookup"><span data-stu-id="b7f25-157">Outlook For Windows</span></span>
- <span data-ttu-id="b7f25-158">Outlook For Mobile</span><span class="sxs-lookup"><span data-stu-id="b7f25-158">Outlook For Mobile</span></span>
- <span data-ttu-id="b7f25-159">Other For Mobile</span><span class="sxs-lookup"><span data-stu-id="b7f25-159">Other For Mobile</span></span>
- <span data-ttu-id="b7f25-160">Outlook For Web</span><span class="sxs-lookup"><span data-stu-id="b7f25-160">Outlook For Web</span></span>
- <span data-ttu-id="b7f25-161">POP3 アプリ</span><span class="sxs-lookup"><span data-stu-id="b7f25-161">POP3 App</span></span>
- <span data-ttu-id="b7f25-162">IMAP4 アプリ</span><span class="sxs-lookup"><span data-stu-id="b7f25-162">IMAP4 App</span></span>
- <span data-ttu-id="b7f25-163">SMTP アプリ</span><span class="sxs-lookup"><span data-stu-id="b7f25-163">SMTP App</span></span>
- <span data-ttu-id="b7f25-164">レポート期間</span><span class="sxs-lookup"><span data-stu-id="b7f25-164">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="b7f25-165">例</span><span class="sxs-lookup"><span data-stu-id="b7f25-165">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b7f25-166">要求</span><span class="sxs-lookup"><span data-stu-id="b7f25-166">Request</span></span>

<span data-ttu-id="b7f25-167">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b7f25-167">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailappusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b7f25-168">C#</span><span class="sxs-lookup"><span data-stu-id="b7f25-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b7f25-169">Javascript</span><span class="sxs-lookup"><span data-stu-id="b7f25-169">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b7f25-170">目的-C</span><span class="sxs-lookup"><span data-stu-id="b7f25-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b7f25-171">応答</span><span class="sxs-lookup"><span data-stu-id="b7f25-171">Response</span></span>

<span data-ttu-id="b7f25-172">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b7f25-172">The following is an example of the response.</span></span>

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

<span data-ttu-id="b7f25-173">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="b7f25-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
