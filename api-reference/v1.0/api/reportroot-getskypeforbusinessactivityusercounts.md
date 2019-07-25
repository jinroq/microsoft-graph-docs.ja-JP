---
title: 'reportRoot: getSkypeForBusinessActivityUserCounts'
description: Skype for Business を介して組織内で行われた会議セッションにおける、それぞれ別個の開催ユーザー数と参加ユーザー数の傾向を取得します。 レポートには、ピア ツー ピア セッションの数も含まれます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 6e73319028d48d5e50f7f46de8ffbca64e923427
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892537"
---
# <a name="reportroot-getskypeforbusinessactivityusercounts"></a><span data-ttu-id="34736-104">reportRoot: getSkypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="34736-104">reportRoot: getSkypeForBusinessActivityUserCounts</span></span>

<span data-ttu-id="34736-105">Skype for Business を介して組織内で行われた会議セッションにおける、それぞれ別個の開催ユーザー数と参加ユーザー数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="34736-105">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="34736-106">レポートには、ピア ツー ピア セッションの数も含まれます。</span><span class="sxs-lookup"><span data-stu-id="34736-106">The report also includes the number of peer-to-peer sessions.</span></span>

> <span data-ttu-id="34736-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business アクティビティ](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="34736-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="34736-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="34736-108">Permissions</span></span>

<span data-ttu-id="34736-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="34736-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="34736-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="34736-111">Permission type</span></span>                        | <span data-ttu-id="34736-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="34736-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="34736-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="34736-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="34736-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="34736-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="34736-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="34736-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34736-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34736-116">Not supported.</span></span>                           |
| <span data-ttu-id="34736-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="34736-117">Application</span></span>                            | <span data-ttu-id="34736-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="34736-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="34736-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="34736-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="34736-120">プロトコル</span><span class="sxs-lookup"><span data-stu-id="34736-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="34736-121">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="34736-121">Function parameters</span></span>

<span data-ttu-id="34736-122">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="34736-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="34736-123">パラメーター</span><span class="sxs-lookup"><span data-stu-id="34736-123">Parameter</span></span> | <span data-ttu-id="34736-124">型</span><span class="sxs-lookup"><span data-stu-id="34736-124">Type</span></span>   | <span data-ttu-id="34736-125">説明</span><span class="sxs-lookup"><span data-stu-id="34736-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="34736-126">period</span><span class="sxs-lookup"><span data-stu-id="34736-126">period</span></span>    | <span data-ttu-id="34736-127">文字列</span><span class="sxs-lookup"><span data-stu-id="34736-127">string</span></span> | <span data-ttu-id="34736-128">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="34736-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="34736-129">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="34736-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="34736-130">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="34736-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="34736-131">必須。</span><span class="sxs-lookup"><span data-stu-id="34736-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="34736-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="34736-132">Request headers</span></span>

| <span data-ttu-id="34736-133">名前</span><span class="sxs-lookup"><span data-stu-id="34736-133">Name</span></span>          | <span data-ttu-id="34736-134">説明</span><span class="sxs-lookup"><span data-stu-id="34736-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="34736-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="34736-135">Authorization</span></span> | <span data-ttu-id="34736-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="34736-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="34736-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="34736-138">If-None-Match</span></span> | <span data-ttu-id="34736-139">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="34736-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="34736-140">省略可能。</span><span class="sxs-lookup"><span data-stu-id="34736-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="34736-141">応答</span><span class="sxs-lookup"><span data-stu-id="34736-141">Response</span></span>

<span data-ttu-id="34736-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="34736-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="34736-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="34736-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="34736-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="34736-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="34736-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="34736-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="34736-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="34736-146">Report Refresh Date</span></span>
- <span data-ttu-id="34736-147">レポート日付</span><span class="sxs-lookup"><span data-stu-id="34736-147">Report Date</span></span>
- <span data-ttu-id="34736-148">レポート期間</span><span class="sxs-lookup"><span data-stu-id="34736-148">Report Period</span></span>
- <span data-ttu-id="34736-149">ピアツーピア</span><span class="sxs-lookup"><span data-stu-id="34736-149">Peer-to-peer</span></span>
- <span data-ttu-id="34736-150">開催</span><span class="sxs-lookup"><span data-stu-id="34736-150">Organized</span></span>
- <span data-ttu-id="34736-151">参加</span><span class="sxs-lookup"><span data-stu-id="34736-151">Participated</span></span>

## <a name="example"></a><span data-ttu-id="34736-152">例</span><span class="sxs-lookup"><span data-stu-id="34736-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="34736-153">要求</span><span class="sxs-lookup"><span data-stu-id="34736-153">Request</span></span>

<span data-ttu-id="34736-154">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="34736-154">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessactivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessActivityUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="34736-155">C#</span><span class="sxs-lookup"><span data-stu-id="34736-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessactivityusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="34736-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="34736-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessactivityusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="34736-157">目的-C</span><span class="sxs-lookup"><span data-stu-id="34736-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessactivityusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="34736-158">Java</span><span class="sxs-lookup"><span data-stu-id="34736-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessactivityusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="34736-159">応答</span><span class="sxs-lookup"><span data-stu-id="34736-159">Response</span></span>

<span data-ttu-id="34736-160">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="34736-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="34736-161">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="34736-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Peer-to-peer,Organized,Participated
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
