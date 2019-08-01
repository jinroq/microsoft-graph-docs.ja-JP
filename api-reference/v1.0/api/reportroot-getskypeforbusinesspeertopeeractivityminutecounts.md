---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts'
description: 組織内で実施されたピア ツー ピア セッションの長さ (分数) と種類についての使用傾向を取得します。 セッションの種類には、オーディオとビデオが含まれます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 379b41ff27b56a8087ed2eb520c4970090f2666a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021705"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityminutecounts"></a><span data-ttu-id="5cc42-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="5cc42-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span></span>

<span data-ttu-id="5cc42-105">組織内で実施されたピア ツー ピア セッションの長さ (分数) と種類についての使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="5cc42-105">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="5cc42-106">セッションの種類には、オーディオとビデオが含まれます。</span><span class="sxs-lookup"><span data-stu-id="5cc42-106">Types of sessions include audio and video.</span></span>

> <span data-ttu-id="5cc42-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business ピア ツー ピア アクティビティ](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5cc42-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="5cc42-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5cc42-108">Permissions</span></span>

<span data-ttu-id="5cc42-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5cc42-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5cc42-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5cc42-111">Permission type</span></span>                        | <span data-ttu-id="5cc42-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5cc42-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5cc42-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="5cc42-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="5cc42-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5cc42-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5cc42-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5cc42-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5cc42-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5cc42-116">Not supported.</span></span>                           |
| <span data-ttu-id="5cc42-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5cc42-117">Application</span></span>                            | <span data-ttu-id="5cc42-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5cc42-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5cc42-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5cc42-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5cc42-120">プロトコル</span><span class="sxs-lookup"><span data-stu-id="5cc42-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="5cc42-121">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="5cc42-121">Function parameters</span></span>

<span data-ttu-id="5cc42-122">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="5cc42-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5cc42-123">パラメーター</span><span class="sxs-lookup"><span data-stu-id="5cc42-123">Parameter</span></span> | <span data-ttu-id="5cc42-124">型</span><span class="sxs-lookup"><span data-stu-id="5cc42-124">Type</span></span>   | <span data-ttu-id="5cc42-125">説明</span><span class="sxs-lookup"><span data-stu-id="5cc42-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5cc42-126">period</span><span class="sxs-lookup"><span data-stu-id="5cc42-126">period</span></span>    | <span data-ttu-id="5cc42-127">文字列</span><span class="sxs-lookup"><span data-stu-id="5cc42-127">string</span></span> | <span data-ttu-id="5cc42-128">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="5cc42-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5cc42-129">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="5cc42-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5cc42-130">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="5cc42-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5cc42-131">必須。</span><span class="sxs-lookup"><span data-stu-id="5cc42-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="5cc42-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5cc42-132">Request headers</span></span>

| <span data-ttu-id="5cc42-133">名前</span><span class="sxs-lookup"><span data-stu-id="5cc42-133">Name</span></span>          | <span data-ttu-id="5cc42-134">説明</span><span class="sxs-lookup"><span data-stu-id="5cc42-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="5cc42-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="5cc42-135">Authorization</span></span> | <span data-ttu-id="5cc42-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5cc42-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="5cc42-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="5cc42-138">If-None-Match</span></span> | <span data-ttu-id="5cc42-139">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="5cc42-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="5cc42-140">省略可能。</span><span class="sxs-lookup"><span data-stu-id="5cc42-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="5cc42-141">応答</span><span class="sxs-lookup"><span data-stu-id="5cc42-141">Response</span></span>

<span data-ttu-id="5cc42-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="5cc42-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5cc42-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="5cc42-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5cc42-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="5cc42-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5cc42-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="5cc42-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5cc42-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="5cc42-146">Report Refresh Date</span></span>
- <span data-ttu-id="5cc42-147">レポート日付</span><span class="sxs-lookup"><span data-stu-id="5cc42-147">Report Date</span></span>
- <span data-ttu-id="5cc42-148">レポート期間</span><span class="sxs-lookup"><span data-stu-id="5cc42-148">Report Period</span></span>
- <span data-ttu-id="5cc42-149">オーディオ</span><span class="sxs-lookup"><span data-stu-id="5cc42-149">Audio</span></span>
- <span data-ttu-id="5cc42-150">ビデオ</span><span class="sxs-lookup"><span data-stu-id="5cc42-150">Video</span></span>

## <a name="example"></a><span data-ttu-id="5cc42-151">例</span><span class="sxs-lookup"><span data-stu-id="5cc42-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5cc42-152">要求</span><span class="sxs-lookup"><span data-stu-id="5cc42-152">Request</span></span>

<span data-ttu-id="5cc42-153">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5cc42-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5cc42-154">C#</span><span class="sxs-lookup"><span data-stu-id="5cc42-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5cc42-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="5cc42-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5cc42-156">目的-C</span><span class="sxs-lookup"><span data-stu-id="5cc42-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5cc42-157">Java</span><span class="sxs-lookup"><span data-stu-id="5cc42-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5cc42-158">応答</span><span class="sxs-lookup"><span data-stu-id="5cc42-158">Response</span></span>

<span data-ttu-id="5cc42-159">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5cc42-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="5cc42-160">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="5cc42-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio,Video
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
