---
title: 'reportRoot: getEmailAppUsageUserCounts'
description: 任意のメール アプリを使用して Exchange Online に接続されている、それぞれ別個のユーザー数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e987c82b94159bcecd19638f4c8e1d56e538c3cb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449429"
---
# <a name="reportroot-getemailappusageusercounts"></a><span data-ttu-id="892a0-103">reportRoot: getEmailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="892a0-103">reportRoot: getEmailAppUsageUserCounts</span></span>

<span data-ttu-id="892a0-104">任意のメール アプリを使用して Exchange Online に接続されている、それぞれ別個のユーザー数を取得します。</span><span class="sxs-lookup"><span data-stu-id="892a0-104">Get the count of unique users that connected to Exchange Online using any email app.</span></span>

> <span data-ttu-id="892a0-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メール アプリの使用状況](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="892a0-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="892a0-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="892a0-106">Permissions</span></span>

<span data-ttu-id="892a0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="892a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="892a0-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="892a0-109">Permission type</span></span>                        | <span data-ttu-id="892a0-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="892a0-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="892a0-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="892a0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="892a0-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="892a0-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="892a0-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="892a0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="892a0-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="892a0-114">Not supported.</span></span>                           |
| <span data-ttu-id="892a0-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="892a0-115">Application</span></span>                            | <span data-ttu-id="892a0-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="892a0-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="892a0-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="892a0-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="892a0-118">プロトコル</span><span class="sxs-lookup"><span data-stu-id="892a0-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="892a0-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="892a0-119">Function parameters</span></span>

<span data-ttu-id="892a0-120">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="892a0-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="892a0-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="892a0-121">Parameter</span></span> | <span data-ttu-id="892a0-122">型</span><span class="sxs-lookup"><span data-stu-id="892a0-122">Type</span></span>   | <span data-ttu-id="892a0-123">説明</span><span class="sxs-lookup"><span data-stu-id="892a0-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="892a0-124">period</span><span class="sxs-lookup"><span data-stu-id="892a0-124">period</span></span>    | <span data-ttu-id="892a0-125">文字列</span><span class="sxs-lookup"><span data-stu-id="892a0-125">string</span></span> | <span data-ttu-id="892a0-126">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="892a0-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="892a0-127">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="892a0-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="892a0-128">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="892a0-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="892a0-129">必須。</span><span class="sxs-lookup"><span data-stu-id="892a0-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="892a0-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="892a0-130">Request headers</span></span>

| <span data-ttu-id="892a0-131">名前</span><span class="sxs-lookup"><span data-stu-id="892a0-131">Name</span></span>          | <span data-ttu-id="892a0-132">説明</span><span class="sxs-lookup"><span data-stu-id="892a0-132">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="892a0-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="892a0-133">Authorization</span></span> | <span data-ttu-id="892a0-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="892a0-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="892a0-136">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="892a0-136">If-None-Match</span></span> | <span data-ttu-id="892a0-137">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="892a0-137">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="892a0-138">省略可能。</span><span class="sxs-lookup"><span data-stu-id="892a0-138">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="892a0-139">応答</span><span class="sxs-lookup"><span data-stu-id="892a0-139">Response</span></span>

<span data-ttu-id="892a0-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="892a0-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="892a0-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="892a0-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="892a0-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="892a0-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="892a0-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="892a0-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="892a0-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="892a0-144">Report Refresh Date</span></span>
- <span data-ttu-id="892a0-145">Mail For Mac</span><span class="sxs-lookup"><span data-stu-id="892a0-145">Mail For Mac</span></span>
- <span data-ttu-id="892a0-146">Outlook For Mac</span><span class="sxs-lookup"><span data-stu-id="892a0-146">Outlook For Mac</span></span>
- <span data-ttu-id="892a0-147">Outlook For Windows</span><span class="sxs-lookup"><span data-stu-id="892a0-147">Outlook For Windows</span></span>
- <span data-ttu-id="892a0-148">Outlook For Mobile</span><span class="sxs-lookup"><span data-stu-id="892a0-148">Outlook For Mobile</span></span>
- <span data-ttu-id="892a0-149">Other For Mobile</span><span class="sxs-lookup"><span data-stu-id="892a0-149">Other For Mobile</span></span>
- <span data-ttu-id="892a0-150">Outlook For Web</span><span class="sxs-lookup"><span data-stu-id="892a0-150">Outlook For Web</span></span>
- <span data-ttu-id="892a0-151">POP3 アプリ</span><span class="sxs-lookup"><span data-stu-id="892a0-151">POP3 App</span></span>
- <span data-ttu-id="892a0-152">IMAP4 アプリ</span><span class="sxs-lookup"><span data-stu-id="892a0-152">IMAP4 App</span></span>
- <span data-ttu-id="892a0-153">SMTP アプリ</span><span class="sxs-lookup"><span data-stu-id="892a0-153">SMTP App</span></span>
- <span data-ttu-id="892a0-154">レポート日付</span><span class="sxs-lookup"><span data-stu-id="892a0-154">Report Date</span></span>
- <span data-ttu-id="892a0-155">レポート期間</span><span class="sxs-lookup"><span data-stu-id="892a0-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="892a0-156">例</span><span class="sxs-lookup"><span data-stu-id="892a0-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="892a0-157">要求</span><span class="sxs-lookup"><span data-stu-id="892a0-157">Request</span></span>

<span data-ttu-id="892a0-158">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="892a0-158">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailappusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="892a0-159">C#</span><span class="sxs-lookup"><span data-stu-id="892a0-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="892a0-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="892a0-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="892a0-161">目的-C</span><span class="sxs-lookup"><span data-stu-id="892a0-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="892a0-162">応答</span><span class="sxs-lookup"><span data-stu-id="892a0-162">Response</span></span>

<span data-ttu-id="892a0-163">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="892a0-163">The following is an example of the response.</span></span>

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

<span data-ttu-id="892a0-164">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="892a0-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Date,Report Period
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
