---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: アクティビティの種類ごとに、Microsoft Teams ユーザーの数を取得します。 アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話、または会議の数です。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 56bcf617e7e32ae2cae62f54f24d0f5bd82c4808
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278107"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="442cc-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="442cc-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

<span data-ttu-id="442cc-105">アクティビティの種類ごとに、Microsoft Teams ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="442cc-105">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="442cc-106">アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話、または会議の数です。</span><span class="sxs-lookup"><span data-stu-id="442cc-106">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="442cc-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="442cc-107">Permissions</span></span>

<span data-ttu-id="442cc-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="442cc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="442cc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="442cc-110">Permission type</span></span>                        | <span data-ttu-id="442cc-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="442cc-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="442cc-112">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="442cc-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="442cc-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="442cc-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="442cc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="442cc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="442cc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="442cc-115">Not supported.</span></span>                           |
| <span data-ttu-id="442cc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="442cc-116">Application</span></span>                            | <span data-ttu-id="442cc-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="442cc-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="442cc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="442cc-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="442cc-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="442cc-119">Function parameters</span></span>

<span data-ttu-id="442cc-120">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="442cc-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="442cc-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="442cc-121">Parameter</span></span> | <span data-ttu-id="442cc-122">型</span><span class="sxs-lookup"><span data-stu-id="442cc-122">Type</span></span>   | <span data-ttu-id="442cc-123">説明</span><span class="sxs-lookup"><span data-stu-id="442cc-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="442cc-124">period</span><span class="sxs-lookup"><span data-stu-id="442cc-124">period</span></span>    | <span data-ttu-id="442cc-125">文字列</span><span class="sxs-lookup"><span data-stu-id="442cc-125">string</span></span> | <span data-ttu-id="442cc-126">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="442cc-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="442cc-127">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="442cc-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="442cc-128">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="442cc-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="442cc-129">必須。</span><span class="sxs-lookup"><span data-stu-id="442cc-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="442cc-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="442cc-130">Request headers</span></span>

| <span data-ttu-id="442cc-131">名前</span><span class="sxs-lookup"><span data-stu-id="442cc-131">Name</span></span>          | <span data-ttu-id="442cc-132">説明</span><span class="sxs-lookup"><span data-stu-id="442cc-132">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="442cc-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="442cc-133">Authorization</span></span> | <span data-ttu-id="442cc-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="442cc-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="442cc-136">応答</span><span class="sxs-lookup"><span data-stu-id="442cc-136">Response</span></span>

<span data-ttu-id="442cc-137">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="442cc-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="442cc-138">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="442cc-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="442cc-139">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="442cc-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="442cc-140">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="442cc-140">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="442cc-141">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="442cc-141">Report Refresh Date</span></span>
- <span data-ttu-id="442cc-142">レポート日付</span><span class="sxs-lookup"><span data-stu-id="442cc-142">Report Date</span></span>
- <span data-ttu-id="442cc-143">チーム チャット メッセージ</span><span class="sxs-lookup"><span data-stu-id="442cc-143">Team Chat Messages</span></span>
- <span data-ttu-id="442cc-144">非公開チャット メッセージ</span><span class="sxs-lookup"><span data-stu-id="442cc-144">Private Chat Messages</span></span>
- <span data-ttu-id="442cc-145">通話</span><span class="sxs-lookup"><span data-stu-id="442cc-145">Calls</span></span>
- <span data-ttu-id="442cc-146">会議</span><span class="sxs-lookup"><span data-stu-id="442cc-146">Meetings</span></span>
- <span data-ttu-id="442cc-147">その他のアクション</span><span class="sxs-lookup"><span data-stu-id="442cc-147">Other Actions</span></span>
- <span data-ttu-id="442cc-148">レポート期間</span><span class="sxs-lookup"><span data-stu-id="442cc-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="442cc-149">例</span><span class="sxs-lookup"><span data-stu-id="442cc-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="442cc-150">要求</span><span class="sxs-lookup"><span data-stu-id="442cc-150">Request</span></span>

<span data-ttu-id="442cc-151">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="442cc-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="442cc-152">応答</span><span class="sxs-lookup"><span data-stu-id="442cc-152">Response</span></span>

<span data-ttu-id="442cc-153">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="442cc-153">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="442cc-154">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="442cc-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="442cc-155">C#</span><span class="sxs-lookup"><span data-stu-id="442cc-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivityusercounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="442cc-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="442cc-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivityusercounts-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="442cc-157">目的-C</span><span class="sxs-lookup"><span data-stu-id="442cc-157">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivityusercounts-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="442cc-158">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="442cc-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Other Actions,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getteamsuseractivityusercounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getteamsuseractivityusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getteamsuseractivityusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
