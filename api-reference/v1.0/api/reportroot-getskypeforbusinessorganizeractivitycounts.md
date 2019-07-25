---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityCounts'
description: 組織内のユーザーが開催、企画した電話会議セッションの数と種類に関する使用状況の傾向を取得します。 会議セッションの種類には、IM、オーディオ/ビデオ、アプリケーション共有、Web、サード パーティへのダイヤルイン/ダイヤルアウト、Microsoft へのダイヤルイン/ダイヤルアウトなどがあります。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 9f57d6e21ca60855c58fd16bacf8a8fd0b38d9c7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892366"
---
# <a name="reportroot-getskypeforbusinessorganizeractivitycounts"></a><span data-ttu-id="f9a05-104">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="f9a05-104">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span></span>

<span data-ttu-id="f9a05-105">組織内のユーザーが開催、企画した電話会議セッションの数と種類に関する使用状況の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="f9a05-105">Get usage trends on the number and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="f9a05-106">会議セッションの種類には、IM、オーディオ/ビデオ、アプリケーション共有、Web、サード パーティへのダイヤルイン/ダイヤルアウト、Microsoft へのダイヤルイン/ダイヤルアウトなどがあります。</span><span class="sxs-lookup"><span data-stu-id="f9a05-106">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and Dial-in/out Microsoft.</span></span>

> <span data-ttu-id="f9a05-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business 電話会議の開催者のアクティビティ](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f9a05-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="f9a05-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f9a05-108">Permissions</span></span>

<span data-ttu-id="f9a05-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f9a05-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f9a05-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f9a05-111">Permission type</span></span>                        | <span data-ttu-id="f9a05-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f9a05-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f9a05-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="f9a05-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f9a05-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f9a05-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f9a05-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f9a05-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9a05-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9a05-116">Not supported.</span></span>                           |
| <span data-ttu-id="f9a05-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f9a05-117">Application</span></span>                            | <span data-ttu-id="f9a05-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f9a05-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f9a05-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f9a05-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f9a05-120">プロトコル</span><span class="sxs-lookup"><span data-stu-id="f9a05-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f9a05-121">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="f9a05-121">Function parameters</span></span>

<span data-ttu-id="f9a05-122">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="f9a05-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f9a05-123">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f9a05-123">Parameter</span></span> | <span data-ttu-id="f9a05-124">型</span><span class="sxs-lookup"><span data-stu-id="f9a05-124">Type</span></span>   | <span data-ttu-id="f9a05-125">説明</span><span class="sxs-lookup"><span data-stu-id="f9a05-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f9a05-126">period</span><span class="sxs-lookup"><span data-stu-id="f9a05-126">period</span></span>    | <span data-ttu-id="f9a05-127">文字列</span><span class="sxs-lookup"><span data-stu-id="f9a05-127">string</span></span> | <span data-ttu-id="f9a05-128">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="f9a05-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f9a05-129">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="f9a05-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f9a05-130">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="f9a05-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f9a05-131">必須。</span><span class="sxs-lookup"><span data-stu-id="f9a05-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f9a05-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f9a05-132">Request headers</span></span>

| <span data-ttu-id="f9a05-133">名前</span><span class="sxs-lookup"><span data-stu-id="f9a05-133">Name</span></span>          | <span data-ttu-id="f9a05-134">説明</span><span class="sxs-lookup"><span data-stu-id="f9a05-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="f9a05-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9a05-135">Authorization</span></span> | <span data-ttu-id="f9a05-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f9a05-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="f9a05-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="f9a05-138">If-None-Match</span></span> | <span data-ttu-id="f9a05-139">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="f9a05-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="f9a05-140">省略可能。</span><span class="sxs-lookup"><span data-stu-id="f9a05-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="f9a05-141">応答</span><span class="sxs-lookup"><span data-stu-id="f9a05-141">Response</span></span>

<span data-ttu-id="f9a05-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="f9a05-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f9a05-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="f9a05-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f9a05-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="f9a05-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f9a05-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="f9a05-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f9a05-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="f9a05-146">Report Refresh Date</span></span>
- <span data-ttu-id="f9a05-147">レポート日付</span><span class="sxs-lookup"><span data-stu-id="f9a05-147">Report Date</span></span>
- <span data-ttu-id="f9a05-148">レポート期間</span><span class="sxs-lookup"><span data-stu-id="f9a05-148">Report Period</span></span>
- <span data-ttu-id="f9a05-149">IM</span><span class="sxs-lookup"><span data-stu-id="f9a05-149">IM</span></span>
- <span data-ttu-id="f9a05-150">オーディオ/ビデオ</span><span class="sxs-lookup"><span data-stu-id="f9a05-150">Audio/Video</span></span>
- <span data-ttu-id="f9a05-151">アプリ共有</span><span class="sxs-lookup"><span data-stu-id="f9a05-151">App Sharing</span></span>
- <span data-ttu-id="f9a05-152">Web</span><span class="sxs-lookup"><span data-stu-id="f9a05-152">Web</span></span>
- <span data-ttu-id="f9a05-153">サード パーティのダイヤルイン/アウト</span><span class="sxs-lookup"><span data-stu-id="f9a05-153">Dial-in/out 3rd Party</span></span>
- <span data-ttu-id="f9a05-154">Microsoft へのダイヤルイン/アウト</span><span class="sxs-lookup"><span data-stu-id="f9a05-154">Dial-in/out Microsoft</span></span>

## <a name="example"></a><span data-ttu-id="f9a05-155">例</span><span class="sxs-lookup"><span data-stu-id="f9a05-155">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f9a05-156">要求</span><span class="sxs-lookup"><span data-stu-id="f9a05-156">Request</span></span>

<span data-ttu-id="f9a05-157">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f9a05-157">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessorganizeractivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessOrganizerActivityCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f9a05-158">C#</span><span class="sxs-lookup"><span data-stu-id="f9a05-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessorganizeractivitycounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f9a05-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="f9a05-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessorganizeractivitycounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f9a05-160">目的-C</span><span class="sxs-lookup"><span data-stu-id="f9a05-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessorganizeractivitycounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f9a05-161">Java</span><span class="sxs-lookup"><span data-stu-id="f9a05-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessorganizeractivitycounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f9a05-162">応答</span><span class="sxs-lookup"><span data-stu-id="f9a05-162">Response</span></span>

<span data-ttu-id="f9a05-163">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f9a05-163">The following is an example of the response.</span></span>

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

<span data-ttu-id="f9a05-164">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="f9a05-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party,Dial-in/out Microsoft
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
