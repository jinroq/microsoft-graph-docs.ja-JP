---
title: 'reportRoot: getSkypeForBusinessParticipantActivityUserCounts'
description: 組織からユーザーが参加したそれぞれ別個のユーザーの数と会議セッションの種類について、使用傾向を取得します。 会議セッションの種類には、IM、オーディオ/ビデオ、アプリケーション共有、Web、サードパーティへのダイヤルイン/ダイヤルアウトなどがあります。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 9568de36d57a4474a6de03d3566c768d32ddea01
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892293"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityusercounts"></a><span data-ttu-id="b5e71-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="b5e71-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span></span>

<span data-ttu-id="b5e71-105">組織からユーザーが参加したそれぞれ別個のユーザーの数と会議セッションの種類について、使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="b5e71-105">Get usage trends on the number of unique users and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="b5e71-106">会議セッションの種類には、IM、オーディオ/ビデオ、アプリケーション共有、Web、サードパーティへのダイヤルイン/ダイヤルアウトなどがあります。</span><span class="sxs-lookup"><span data-stu-id="b5e71-106">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span>

> <span data-ttu-id="b5e71-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business 電話会議の参加者のアクティビティ](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b5e71-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="b5e71-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b5e71-108">Permissions</span></span>

<span data-ttu-id="b5e71-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b5e71-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b5e71-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b5e71-111">Permission type</span></span>                        | <span data-ttu-id="b5e71-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b5e71-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b5e71-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="b5e71-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b5e71-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5e71-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b5e71-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b5e71-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5e71-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b5e71-116">Not supported.</span></span>                           |
| <span data-ttu-id="b5e71-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b5e71-117">Application</span></span>                            | <span data-ttu-id="b5e71-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5e71-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b5e71-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b5e71-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b5e71-120">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b5e71-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="b5e71-121">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="b5e71-121">Function parameters</span></span>

<span data-ttu-id="b5e71-122">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="b5e71-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b5e71-123">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b5e71-123">Parameter</span></span> | <span data-ttu-id="b5e71-124">型</span><span class="sxs-lookup"><span data-stu-id="b5e71-124">Type</span></span>   | <span data-ttu-id="b5e71-125">説明</span><span class="sxs-lookup"><span data-stu-id="b5e71-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b5e71-126">period</span><span class="sxs-lookup"><span data-stu-id="b5e71-126">period</span></span>    | <span data-ttu-id="b5e71-127">文字列</span><span class="sxs-lookup"><span data-stu-id="b5e71-127">string</span></span> | <span data-ttu-id="b5e71-128">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="b5e71-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b5e71-129">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="b5e71-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b5e71-130">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="b5e71-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b5e71-131">必須。</span><span class="sxs-lookup"><span data-stu-id="b5e71-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="b5e71-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b5e71-132">Request headers</span></span>

| <span data-ttu-id="b5e71-133">名前</span><span class="sxs-lookup"><span data-stu-id="b5e71-133">Name</span></span>          | <span data-ttu-id="b5e71-134">説明</span><span class="sxs-lookup"><span data-stu-id="b5e71-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="b5e71-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5e71-135">Authorization</span></span> | <span data-ttu-id="b5e71-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b5e71-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="b5e71-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="b5e71-138">If-None-Match</span></span> | <span data-ttu-id="b5e71-139">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="b5e71-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="b5e71-140">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b5e71-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="b5e71-141">応答</span><span class="sxs-lookup"><span data-stu-id="b5e71-141">Response</span></span>

<span data-ttu-id="b5e71-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="b5e71-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b5e71-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="b5e71-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b5e71-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="b5e71-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b5e71-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="b5e71-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b5e71-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="b5e71-146">Report Refresh Date</span></span>
- <span data-ttu-id="b5e71-147">レポート日付</span><span class="sxs-lookup"><span data-stu-id="b5e71-147">Report Date</span></span>
- <span data-ttu-id="b5e71-148">レポート期間</span><span class="sxs-lookup"><span data-stu-id="b5e71-148">Report Period</span></span>
- <span data-ttu-id="b5e71-149">IM</span><span class="sxs-lookup"><span data-stu-id="b5e71-149">IM</span></span>
- <span data-ttu-id="b5e71-150">オーディオ/ビデオ</span><span class="sxs-lookup"><span data-stu-id="b5e71-150">Audio/Video</span></span>
- <span data-ttu-id="b5e71-151">アプリ共有</span><span class="sxs-lookup"><span data-stu-id="b5e71-151">App Sharing</span></span>
- <span data-ttu-id="b5e71-152">Web</span><span class="sxs-lookup"><span data-stu-id="b5e71-152">Web</span></span>
- <span data-ttu-id="b5e71-153">サード パーティのダイヤルイン/アウト</span><span class="sxs-lookup"><span data-stu-id="b5e71-153">Dial-in/out 3rd Party</span></span>

## <a name="example"></a><span data-ttu-id="b5e71-154">例</span><span class="sxs-lookup"><span data-stu-id="b5e71-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b5e71-155">要求</span><span class="sxs-lookup"><span data-stu-id="b5e71-155">Request</span></span>

<span data-ttu-id="b5e71-156">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b5e71-156">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessparticipantactivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b5e71-157">C#</span><span class="sxs-lookup"><span data-stu-id="b5e71-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessparticipantactivityusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b5e71-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="b5e71-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessparticipantactivityusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b5e71-159">目的-C</span><span class="sxs-lookup"><span data-stu-id="b5e71-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessparticipantactivityusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b5e71-160">Java</span><span class="sxs-lookup"><span data-stu-id="b5e71-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessparticipantactivityusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b5e71-161">応答</span><span class="sxs-lookup"><span data-stu-id="b5e71-161">Response</span></span>

<span data-ttu-id="b5e71-162">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b5e71-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="b5e71-163">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="b5e71-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
  ]
}-->
