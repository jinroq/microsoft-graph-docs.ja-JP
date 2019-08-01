---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserCounts'
description: Skype for Business アプリを使用して接続した組織内のユーザー数について、使用傾向を取得します。 組織内で Skype for Business クライアント アプリをインストールし、使用したデバイスの種類 (Windows、Windows スマートフォン、Android スマートフォン、iPhone、iPad) の詳細も取得できます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 30c77dbd2332f2d1a6e027d7583380795d5c47b8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021747"
---
# <a name="reportroot-getskypeforbusinessdeviceusageusercounts"></a><span data-ttu-id="fbd93-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="fbd93-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span></span>

<span data-ttu-id="fbd93-105">Skype for Business アプリを使用して接続した組織内のユーザー数について、使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="fbd93-105">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="fbd93-106">組織内で Skype for Business クライアント アプリをインストールし、使用したデバイスの種類 (Windows、Windows スマートフォン、Android スマートフォン、iPhone、iPad) の詳細も取得できます。</span><span class="sxs-lookup"><span data-stu-id="fbd93-106">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span>

> <span data-ttu-id="fbd93-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: 使用している Skype for Business クライアント](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fbd93-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="fbd93-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fbd93-108">Permissions</span></span>

<span data-ttu-id="fbd93-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fbd93-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fbd93-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fbd93-111">Permission type</span></span>                        | <span data-ttu-id="fbd93-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fbd93-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="fbd93-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="fbd93-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="fbd93-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbd93-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="fbd93-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fbd93-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fbd93-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fbd93-116">Not supported.</span></span>                           |
| <span data-ttu-id="fbd93-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fbd93-117">Application</span></span>                            | <span data-ttu-id="fbd93-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbd93-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="fbd93-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fbd93-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fbd93-120">プロトコル</span><span class="sxs-lookup"><span data-stu-id="fbd93-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="fbd93-121">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="fbd93-121">Function parameters</span></span>

<span data-ttu-id="fbd93-122">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="fbd93-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="fbd93-123">パラメーター</span><span class="sxs-lookup"><span data-stu-id="fbd93-123">Parameter</span></span> | <span data-ttu-id="fbd93-124">型</span><span class="sxs-lookup"><span data-stu-id="fbd93-124">Type</span></span>   | <span data-ttu-id="fbd93-125">説明</span><span class="sxs-lookup"><span data-stu-id="fbd93-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="fbd93-126">period</span><span class="sxs-lookup"><span data-stu-id="fbd93-126">period</span></span>    | <span data-ttu-id="fbd93-127">文字列</span><span class="sxs-lookup"><span data-stu-id="fbd93-127">string</span></span> | <span data-ttu-id="fbd93-128">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="fbd93-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="fbd93-129">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="fbd93-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="fbd93-130">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="fbd93-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="fbd93-131">必須。</span><span class="sxs-lookup"><span data-stu-id="fbd93-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="fbd93-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fbd93-132">Request headers</span></span>

| <span data-ttu-id="fbd93-133">名前</span><span class="sxs-lookup"><span data-stu-id="fbd93-133">Name</span></span>          | <span data-ttu-id="fbd93-134">説明</span><span class="sxs-lookup"><span data-stu-id="fbd93-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="fbd93-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbd93-135">Authorization</span></span> | <span data-ttu-id="fbd93-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fbd93-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="fbd93-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="fbd93-138">If-None-Match</span></span> | <span data-ttu-id="fbd93-139">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="fbd93-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="fbd93-140">省略可能。</span><span class="sxs-lookup"><span data-stu-id="fbd93-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="fbd93-141">応答</span><span class="sxs-lookup"><span data-stu-id="fbd93-141">Response</span></span>

<span data-ttu-id="fbd93-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="fbd93-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="fbd93-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="fbd93-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="fbd93-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="fbd93-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="fbd93-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="fbd93-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="fbd93-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="fbd93-146">Report Refresh Date</span></span>
- <span data-ttu-id="fbd93-147">Windows</span><span class="sxs-lookup"><span data-stu-id="fbd93-147">Windows</span></span>
- <span data-ttu-id="fbd93-148">Windows スマートフォン</span><span class="sxs-lookup"><span data-stu-id="fbd93-148">Windows Phone</span></span>
- <span data-ttu-id="fbd93-149">Android スマートフォン</span><span class="sxs-lookup"><span data-stu-id="fbd93-149">Android Phone</span></span>
- <span data-ttu-id="fbd93-150">iPhone</span><span class="sxs-lookup"><span data-stu-id="fbd93-150">iPhone</span></span>
- <span data-ttu-id="fbd93-151">iPad</span><span class="sxs-lookup"><span data-stu-id="fbd93-151">iPad</span></span>
- <span data-ttu-id="fbd93-152">レポート日付</span><span class="sxs-lookup"><span data-stu-id="fbd93-152">Report Date</span></span>
- <span data-ttu-id="fbd93-153">レポート期間</span><span class="sxs-lookup"><span data-stu-id="fbd93-153">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="fbd93-154">例</span><span class="sxs-lookup"><span data-stu-id="fbd93-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="fbd93-155">要求</span><span class="sxs-lookup"><span data-stu-id="fbd93-155">Request</span></span>

<span data-ttu-id="fbd93-156">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fbd93-156">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fbd93-157">C#</span><span class="sxs-lookup"><span data-stu-id="fbd93-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusageusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fbd93-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="fbd93-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusageusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fbd93-159">目的-C</span><span class="sxs-lookup"><span data-stu-id="fbd93-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusageusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fbd93-160">Java</span><span class="sxs-lookup"><span data-stu-id="fbd93-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessdeviceusageusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fbd93-161">応答</span><span class="sxs-lookup"><span data-stu-id="fbd93-161">Response</span></span>

<span data-ttu-id="fbd93-162">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fbd93-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="fbd93-163">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="fbd93-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Date,Report Period
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
