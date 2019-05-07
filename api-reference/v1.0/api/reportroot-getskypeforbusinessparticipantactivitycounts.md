---
title: 'reportRoot: getSkypeForBusinessParticipantActivityCounts'
description: 組織からユーザーが参加した会議セッションの数と種類について、使用傾向を取得します。 会議セッションの種類には、IM、オーディオ/ビデオ、アプリケーション共有、Web、サードパーティへのダイヤルイン/ダイヤルアウトなどがあります。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a69d20258622dd68e219b99d437f8f446af0d756
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33604173"
---
# <a name="reportroot-getskypeforbusinessparticipantactivitycounts"></a><span data-ttu-id="ce3cd-104">reportRoot: getSkypeForBusinessParticipantActivityCounts</span><span class="sxs-lookup"><span data-stu-id="ce3cd-104">reportRoot: getSkypeForBusinessParticipantActivityCounts</span></span>

<span data-ttu-id="ce3cd-105">組織からユーザーが参加した会議セッションの数と種類について、使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="ce3cd-105">Get usage trends on the number and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="ce3cd-106">会議セッションの種類には、IM、オーディオ/ビデオ、アプリケーション共有、Web、サードパーティへのダイヤルイン/ダイヤルアウトなどがあります。</span><span class="sxs-lookup"><span data-stu-id="ce3cd-106">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span>

> <span data-ttu-id="ce3cd-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business 電話会議の参加者のアクティビティ](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce3cd-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="ce3cd-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ce3cd-108">Permissions</span></span>

<span data-ttu-id="ce3cd-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce3cd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ce3cd-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ce3cd-111">Permission type</span></span>                        | <span data-ttu-id="ce3cd-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ce3cd-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ce3cd-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="ce3cd-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ce3cd-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce3cd-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ce3cd-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ce3cd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce3cd-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce3cd-116">Not supported.</span></span>                           |
| <span data-ttu-id="ce3cd-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ce3cd-117">Application</span></span>                            | <span data-ttu-id="ce3cd-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce3cd-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ce3cd-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ce3cd-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ce3cd-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="ce3cd-120">Function parameters</span></span>

<span data-ttu-id="ce3cd-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="ce3cd-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ce3cd-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ce3cd-122">Parameter</span></span> | <span data-ttu-id="ce3cd-123">型</span><span class="sxs-lookup"><span data-stu-id="ce3cd-123">Type</span></span>   | <span data-ttu-id="ce3cd-124">説明</span><span class="sxs-lookup"><span data-stu-id="ce3cd-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ce3cd-125">period</span><span class="sxs-lookup"><span data-stu-id="ce3cd-125">period</span></span>    | <span data-ttu-id="ce3cd-126">文字列</span><span class="sxs-lookup"><span data-stu-id="ce3cd-126">string</span></span> | <span data-ttu-id="ce3cd-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="ce3cd-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ce3cd-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="ce3cd-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ce3cd-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="ce3cd-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ce3cd-130">必須。</span><span class="sxs-lookup"><span data-stu-id="ce3cd-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="ce3cd-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce3cd-131">Request headers</span></span>

| <span data-ttu-id="ce3cd-132">名前</span><span class="sxs-lookup"><span data-stu-id="ce3cd-132">Name</span></span>          | <span data-ttu-id="ce3cd-133">説明</span><span class="sxs-lookup"><span data-stu-id="ce3cd-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="ce3cd-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce3cd-134">Authorization</span></span> | <span data-ttu-id="ce3cd-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ce3cd-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="ce3cd-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="ce3cd-137">If-None-Match</span></span> | <span data-ttu-id="ce3cd-138">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="ce3cd-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="ce3cd-139">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ce3cd-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="ce3cd-140">応答</span><span class="sxs-lookup"><span data-stu-id="ce3cd-140">Response</span></span>

<span data-ttu-id="ce3cd-141">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="ce3cd-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ce3cd-142">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="ce3cd-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ce3cd-143">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="ce3cd-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ce3cd-144">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="ce3cd-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ce3cd-145">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="ce3cd-145">Report Refresh Date</span></span>
- <span data-ttu-id="ce3cd-146">レポート日付</span><span class="sxs-lookup"><span data-stu-id="ce3cd-146">Report Date</span></span>
- <span data-ttu-id="ce3cd-147">レポート期間</span><span class="sxs-lookup"><span data-stu-id="ce3cd-147">Report Period</span></span>
- <span data-ttu-id="ce3cd-148">IM</span><span class="sxs-lookup"><span data-stu-id="ce3cd-148">IM</span></span>
- <span data-ttu-id="ce3cd-149">オーディオ/ビデオ</span><span class="sxs-lookup"><span data-stu-id="ce3cd-149">Audio/Video</span></span>
- <span data-ttu-id="ce3cd-150">アプリ共有</span><span class="sxs-lookup"><span data-stu-id="ce3cd-150">App Sharing</span></span>
- <span data-ttu-id="ce3cd-151">Web</span><span class="sxs-lookup"><span data-stu-id="ce3cd-151">Web</span></span>
- <span data-ttu-id="ce3cd-152">サード パーティのダイヤルイン/アウト</span><span class="sxs-lookup"><span data-stu-id="ce3cd-152">Dial-in/out 3rd Party</span></span>

## <a name="example"></a><span data-ttu-id="ce3cd-153">例</span><span class="sxs-lookup"><span data-stu-id="ce3cd-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ce3cd-154">要求</span><span class="sxs-lookup"><span data-stu-id="ce3cd-154">Request</span></span>

<span data-ttu-id="ce3cd-155">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ce3cd-155">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessparticipantactivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessParticipantActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="ce3cd-156">応答</span><span class="sxs-lookup"><span data-stu-id="ce3cd-156">Response</span></span>

<span data-ttu-id="ce3cd-157">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ce3cd-157">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ce3cd-158">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="ce3cd-158">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ce3cd-159">Visual</span><span class="sxs-lookup"><span data-stu-id="ce3cd-159">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessparticipantactivitycounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ce3cd-160">Java</span><span class="sxs-lookup"><span data-stu-id="ce3cd-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessparticipantactivitycounts-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="ce3cd-161">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="ce3cd-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party
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
    "Error: /api-reference/v1.0/api/reportroot-getskypeforbusinessparticipantactivitycounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getskypeforbusinessparticipantactivitycounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
