---
title: 'reportRoot: getSharePointActivityUserCounts'
description: アクティブ ユーザーの数の傾向を取得します。 ユーザーが一定期間中にファイル アクティビティ (保存、同期、変更、共有) を実行するか、またはページにアクセスすると、そのユーザーはアクティブとみなされます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c64a87e51bd3f3ee140aa5e125f38be3c3594a80
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273354"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="8f2f4-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="8f2f4-104">reportRoot: getSharePointActivityUserCounts</span></span>

<span data-ttu-id="8f2f4-105">アクティブ ユーザーの数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="8f2f4-105">Get the trend in the number of active users.</span></span> <span data-ttu-id="8f2f4-106">ユーザーが一定期間中にファイル アクティビティ (保存、同期、変更、共有) を実行するか、またはページにアクセスすると、そのユーザーはアクティブとみなされます。</span><span class="sxs-lookup"><span data-stu-id="8f2f4-106">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="8f2f4-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint アクティビティ](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8f2f4-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="8f2f4-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8f2f4-108">Permissions</span></span>

<span data-ttu-id="8f2f4-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8f2f4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8f2f4-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8f2f4-111">Permission type</span></span>                        | <span data-ttu-id="8f2f4-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8f2f4-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8f2f4-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="8f2f4-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8f2f4-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f2f4-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8f2f4-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8f2f4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f2f4-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8f2f4-116">Not supported.</span></span>                           |
| <span data-ttu-id="8f2f4-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8f2f4-117">Application</span></span>                            | <span data-ttu-id="8f2f4-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f2f4-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8f2f4-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8f2f4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="8f2f4-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="8f2f4-120">Function parameters</span></span>

<span data-ttu-id="8f2f4-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="8f2f4-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="8f2f4-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="8f2f4-122">Parameter</span></span> | <span data-ttu-id="8f2f4-123">型</span><span class="sxs-lookup"><span data-stu-id="8f2f4-123">Type</span></span>   | <span data-ttu-id="8f2f4-124">説明</span><span class="sxs-lookup"><span data-stu-id="8f2f4-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8f2f4-125">period</span><span class="sxs-lookup"><span data-stu-id="8f2f4-125">period</span></span>    | <span data-ttu-id="8f2f4-126">文字列</span><span class="sxs-lookup"><span data-stu-id="8f2f4-126">string</span></span> | <span data-ttu-id="8f2f4-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="8f2f4-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8f2f4-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="8f2f4-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8f2f4-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="8f2f4-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="8f2f4-130">必須。</span><span class="sxs-lookup"><span data-stu-id="8f2f4-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="8f2f4-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8f2f4-131">Request headers</span></span>

| <span data-ttu-id="8f2f4-132">名前</span><span class="sxs-lookup"><span data-stu-id="8f2f4-132">Name</span></span>          | <span data-ttu-id="8f2f4-133">説明</span><span class="sxs-lookup"><span data-stu-id="8f2f4-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="8f2f4-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f2f4-134">Authorization</span></span> | <span data-ttu-id="8f2f4-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8f2f4-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="8f2f4-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="8f2f4-137">If-None-Match</span></span> | <span data-ttu-id="8f2f4-138">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="8f2f4-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="8f2f4-139">省略可能。</span><span class="sxs-lookup"><span data-stu-id="8f2f4-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="8f2f4-140">応答</span><span class="sxs-lookup"><span data-stu-id="8f2f4-140">Response</span></span>

<span data-ttu-id="8f2f4-141">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="8f2f4-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8f2f4-142">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="8f2f4-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8f2f4-143">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="8f2f4-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8f2f4-144">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="8f2f4-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8f2f4-145">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="8f2f4-145">Report Refresh Date</span></span>
- <span data-ttu-id="8f2f4-146">アクセスしたページ</span><span class="sxs-lookup"><span data-stu-id="8f2f4-146">Visited Page</span></span>
- <span data-ttu-id="8f2f4-147">表示済みまたは編集済み</span><span class="sxs-lookup"><span data-stu-id="8f2f4-147">Viewed Or Edited</span></span>
- <span data-ttu-id="8f2f4-148">同期済み</span><span class="sxs-lookup"><span data-stu-id="8f2f4-148">Synced</span></span>
- <span data-ttu-id="8f2f4-149">社内で共有済み</span><span class="sxs-lookup"><span data-stu-id="8f2f4-149">Shared Internally</span></span>
- <span data-ttu-id="8f2f4-150">外部で共有済み</span><span class="sxs-lookup"><span data-stu-id="8f2f4-150">Shared Externally</span></span>
- <span data-ttu-id="8f2f4-151">レポート日付</span><span class="sxs-lookup"><span data-stu-id="8f2f4-151">Report Date</span></span>
- <span data-ttu-id="8f2f4-152">レポート期間</span><span class="sxs-lookup"><span data-stu-id="8f2f4-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="8f2f4-153">例</span><span class="sxs-lookup"><span data-stu-id="8f2f4-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8f2f4-154">要求</span><span class="sxs-lookup"><span data-stu-id="8f2f4-154">Request</span></span>

<span data-ttu-id="8f2f4-155">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8f2f4-155">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="8f2f4-156">応答</span><span class="sxs-lookup"><span data-stu-id="8f2f4-156">Response</span></span>

<span data-ttu-id="8f2f4-157">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8f2f4-157">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8f2f4-158">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="8f2f4-158">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8f2f4-159">C#</span><span class="sxs-lookup"><span data-stu-id="8f2f4-159">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointactivityusercounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f2f4-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="8f2f4-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointactivityusercounts-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8f2f4-161">目的-C</span><span class="sxs-lookup"><span data-stu-id="8f2f4-161">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointactivityusercounts-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="8f2f4-162">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="8f2f4-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getsharepointactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getsharepointactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getsharepointactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
