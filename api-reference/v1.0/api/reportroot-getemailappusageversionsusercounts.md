---
title: 'reportRoot: getEmailAppUsageVersionsUserCounts'
description: Outlook デスクトップ版ごとの、それぞれ別個のユーザー数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: c45e4cc0fb23919d9b772f35bb2853a384b0cd74
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327292"
---
# <a name="reportroot-getemailappusageversionsusercounts"></a><span data-ttu-id="4a867-103">reportRoot: getEmailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="4a867-103">reportRoot: getEmailAppUsageVersionsUserCounts</span></span>

<span data-ttu-id="4a867-104">Outlook デスクトップ版ごとの、それぞれ別個のユーザー数を取得します。</span><span class="sxs-lookup"><span data-stu-id="4a867-104">Get the count of unique users by Outlook desktop version.</span></span>

> <span data-ttu-id="4a867-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メール アプリの使用状況](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4a867-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="4a867-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4a867-106">Permissions</span></span>

<span data-ttu-id="4a867-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4a867-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4a867-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4a867-109">Permission type</span></span>                        | <span data-ttu-id="4a867-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4a867-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4a867-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="4a867-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4a867-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a867-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4a867-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4a867-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a867-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a867-114">Not supported.</span></span>                           |
| <span data-ttu-id="4a867-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4a867-115">Application</span></span>                            | <span data-ttu-id="4a867-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a867-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4a867-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4a867-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageVersionsUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4a867-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="4a867-118">Function parameters</span></span>

<span data-ttu-id="4a867-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="4a867-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4a867-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="4a867-120">Parameter</span></span> | <span data-ttu-id="4a867-121">型</span><span class="sxs-lookup"><span data-stu-id="4a867-121">Type</span></span>   | <span data-ttu-id="4a867-122">説明</span><span class="sxs-lookup"><span data-stu-id="4a867-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4a867-123">period</span><span class="sxs-lookup"><span data-stu-id="4a867-123">period</span></span>    | <span data-ttu-id="4a867-124">文字列</span><span class="sxs-lookup"><span data-stu-id="4a867-124">string</span></span> | <span data-ttu-id="4a867-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="4a867-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4a867-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="4a867-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4a867-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="4a867-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4a867-128">必須。</span><span class="sxs-lookup"><span data-stu-id="4a867-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="4a867-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4a867-129">Request headers</span></span>

| <span data-ttu-id="4a867-130">名前</span><span class="sxs-lookup"><span data-stu-id="4a867-130">Name</span></span>          | <span data-ttu-id="4a867-131">説明</span><span class="sxs-lookup"><span data-stu-id="4a867-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="4a867-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a867-132">Authorization</span></span> | <span data-ttu-id="4a867-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4a867-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="4a867-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="4a867-135">If-None-Match</span></span> | <span data-ttu-id="4a867-136">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="4a867-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="4a867-137">省略可能。</span><span class="sxs-lookup"><span data-stu-id="4a867-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="4a867-138">応答</span><span class="sxs-lookup"><span data-stu-id="4a867-138">Response</span></span>

<span data-ttu-id="4a867-139">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="4a867-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4a867-140">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="4a867-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4a867-141">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="4a867-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4a867-142">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="4a867-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4a867-143">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="4a867-143">Report Refresh Date</span></span>
- <span data-ttu-id="4a867-144">Outlook 2016</span><span class="sxs-lookup"><span data-stu-id="4a867-144">Outlook 2016</span></span>
- <span data-ttu-id="4a867-145">Outlook 2013</span><span class="sxs-lookup"><span data-stu-id="4a867-145">Outlook 2013</span></span>
- <span data-ttu-id="4a867-146">Outlook 2010</span><span class="sxs-lookup"><span data-stu-id="4a867-146">Outlook 2010</span></span>
- <span data-ttu-id="4a867-147">Outlook 2007</span><span class="sxs-lookup"><span data-stu-id="4a867-147">Outlook 2007</span></span>
- <span data-ttu-id="4a867-148">未定義</span><span class="sxs-lookup"><span data-stu-id="4a867-148">Undetermined</span></span>
- <span data-ttu-id="4a867-149">レポート期間</span><span class="sxs-lookup"><span data-stu-id="4a867-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="4a867-150">例</span><span class="sxs-lookup"><span data-stu-id="4a867-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4a867-151">要求</span><span class="sxs-lookup"><span data-stu-id="4a867-151">Request</span></span>

<span data-ttu-id="4a867-152">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4a867-152">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4a867-153">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4a867-153">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailappusageversionsusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageVersionsUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4a867-154">C#</span><span class="sxs-lookup"><span data-stu-id="4a867-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageversionsusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4a867-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a867-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageversionsusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4a867-156">目的-C</span><span class="sxs-lookup"><span data-stu-id="4a867-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageversionsusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4a867-157">Java</span><span class="sxs-lookup"><span data-stu-id="4a867-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getemailappusageversionsusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4a867-158">応答</span><span class="sxs-lookup"><span data-stu-id="4a867-158">Response</span></span>

<span data-ttu-id="4a867-159">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4a867-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="4a867-160">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="4a867-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Outlook 2016,Outlook 2013,Outlook 2010,Outlook 2007,Undetermined,Report Period
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
