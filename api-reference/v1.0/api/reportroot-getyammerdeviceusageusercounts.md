---
title: 'reportRoot: getYammerDeviceUsageUserCounts'
description: デバイスの種類別に日次ユーザーの数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 05a0bac1bc7f7b81521c82e35f1804fe267def91
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320291"
---
# <a name="reportroot-getyammerdeviceusageusercounts"></a><span data-ttu-id="2e852-103">reportRoot: getYammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="2e852-103">reportRoot: getYammerDeviceUsageUserCounts</span></span>

<span data-ttu-id="2e852-104">デバイスの種類別に日次ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="2e852-104">Get the number of daily users by device type.</span></span>

> <span data-ttu-id="2e852-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer デバイスの使用状況](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2e852-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="2e852-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2e852-106">Permissions</span></span>

<span data-ttu-id="2e852-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2e852-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2e852-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2e852-109">Permission type</span></span>                        | <span data-ttu-id="2e852-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2e852-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2e852-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="2e852-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2e852-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e852-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2e852-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2e852-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e852-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2e852-114">Not supported.</span></span>                           |
| <span data-ttu-id="2e852-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2e852-115">Application</span></span>                            | <span data-ttu-id="2e852-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e852-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2e852-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2e852-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="2e852-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="2e852-118">Function parameters</span></span>

<span data-ttu-id="2e852-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="2e852-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="2e852-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="2e852-120">Parameter</span></span> | <span data-ttu-id="2e852-121">型</span><span class="sxs-lookup"><span data-stu-id="2e852-121">Type</span></span>   | <span data-ttu-id="2e852-122">説明</span><span class="sxs-lookup"><span data-stu-id="2e852-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2e852-123">period</span><span class="sxs-lookup"><span data-stu-id="2e852-123">period</span></span>    | <span data-ttu-id="2e852-124">文字列</span><span class="sxs-lookup"><span data-stu-id="2e852-124">string</span></span> | <span data-ttu-id="2e852-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="2e852-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2e852-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="2e852-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2e852-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="2e852-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="2e852-128">必須。</span><span class="sxs-lookup"><span data-stu-id="2e852-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="2e852-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2e852-129">Request headers</span></span>

| <span data-ttu-id="2e852-130">名前</span><span class="sxs-lookup"><span data-stu-id="2e852-130">Name</span></span>          | <span data-ttu-id="2e852-131">説明</span><span class="sxs-lookup"><span data-stu-id="2e852-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="2e852-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e852-132">Authorization</span></span> | <span data-ttu-id="2e852-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2e852-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="2e852-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="2e852-135">If-None-Match</span></span> | <span data-ttu-id="2e852-136">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="2e852-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="2e852-137">省略可能。</span><span class="sxs-lookup"><span data-stu-id="2e852-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="2e852-138">応答</span><span class="sxs-lookup"><span data-stu-id="2e852-138">Response</span></span>

<span data-ttu-id="2e852-139">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="2e852-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2e852-140">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="2e852-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2e852-141">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="2e852-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2e852-142">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="2e852-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2e852-143">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="2e852-143">Report Refresh Date</span></span>
- <span data-ttu-id="2e852-144">Web</span><span class="sxs-lookup"><span data-stu-id="2e852-144">Web</span></span>
- <span data-ttu-id="2e852-145">Windows スマートフォン</span><span class="sxs-lookup"><span data-stu-id="2e852-145">Windows Phone</span></span>
- <span data-ttu-id="2e852-146">Android スマートフォン</span><span class="sxs-lookup"><span data-stu-id="2e852-146">Android Phone</span></span>
- <span data-ttu-id="2e852-147">iPhone</span><span class="sxs-lookup"><span data-stu-id="2e852-147">iPhone</span></span>
- <span data-ttu-id="2e852-148">iPad</span><span class="sxs-lookup"><span data-stu-id="2e852-148">iPad</span></span>
- <span data-ttu-id="2e852-149">その他</span><span class="sxs-lookup"><span data-stu-id="2e852-149">Other</span></span>
- <span data-ttu-id="2e852-150">レポート日付</span><span class="sxs-lookup"><span data-stu-id="2e852-150">Report Date</span></span>
- <span data-ttu-id="2e852-151">レポート期間</span><span class="sxs-lookup"><span data-stu-id="2e852-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="2e852-152">例</span><span class="sxs-lookup"><span data-stu-id="2e852-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2e852-153">要求</span><span class="sxs-lookup"><span data-stu-id="2e852-153">Request</span></span>

<span data-ttu-id="2e852-154">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2e852-154">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2e852-155">プロトコル</span><span class="sxs-lookup"><span data-stu-id="2e852-155">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2e852-156">C#</span><span class="sxs-lookup"><span data-stu-id="2e852-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammerdeviceusageusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2e852-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e852-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammerdeviceusageusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2e852-158">目的-C</span><span class="sxs-lookup"><span data-stu-id="2e852-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammerdeviceusageusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2e852-159">Java</span><span class="sxs-lookup"><span data-stu-id="2e852-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammerdeviceusageusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2e852-160">応答</span><span class="sxs-lookup"><span data-stu-id="2e852-160">Response</span></span>

<span data-ttu-id="2e852-161">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2e852-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="2e852-162">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="2e852-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Date,Report Period
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
