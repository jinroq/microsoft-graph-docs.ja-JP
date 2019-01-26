---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserCounts'
description: Skype for Business アプリを使用して接続した組織内のユーザー数について、使用傾向を取得します。 組織内で Skype for Business クライアント アプリをインストールし、使用したデバイスの種類 (Windows、Windows スマートフォン、Android スマートフォン、iPhone、iPad) の詳細も取得できます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 980e83838833e2fc7c16218417eb84df4949cc83
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572088"
---
# <a name="reportroot-getskypeforbusinessdeviceusageusercounts"></a><span data-ttu-id="57920-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="57920-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span></span>

<span data-ttu-id="57920-105">Skype for Business アプリを使用して接続した組織内のユーザー数について、使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="57920-105">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="57920-106">組織内で Skype for Business クライアント アプリをインストールし、使用したデバイスの種類 (Windows、Windows スマートフォン、Android スマートフォン、iPhone、iPad) の詳細も取得できます。</span><span class="sxs-lookup"><span data-stu-id="57920-106">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span>

> <span data-ttu-id="57920-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: 使用している Skype for Business クライアント](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="57920-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="57920-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="57920-108">Permissions</span></span>

<span data-ttu-id="57920-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="57920-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="57920-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="57920-111">Permission type</span></span>                        | <span data-ttu-id="57920-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="57920-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="57920-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="57920-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="57920-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="57920-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="57920-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="57920-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57920-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57920-116">Not supported.</span></span>                           |
| <span data-ttu-id="57920-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="57920-117">Application</span></span>                            | <span data-ttu-id="57920-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="57920-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="57920-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="57920-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="57920-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="57920-120">Function parameters</span></span>

<span data-ttu-id="57920-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="57920-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="57920-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="57920-122">Parameter</span></span> | <span data-ttu-id="57920-123">型</span><span class="sxs-lookup"><span data-stu-id="57920-123">Type</span></span>   | <span data-ttu-id="57920-124">説明</span><span class="sxs-lookup"><span data-stu-id="57920-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="57920-125">period</span><span class="sxs-lookup"><span data-stu-id="57920-125">period</span></span>    | <span data-ttu-id="57920-126">文字列</span><span class="sxs-lookup"><span data-stu-id="57920-126">string</span></span> | <span data-ttu-id="57920-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="57920-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="57920-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="57920-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="57920-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="57920-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="57920-130">必須。</span><span class="sxs-lookup"><span data-stu-id="57920-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="57920-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="57920-131">Request headers</span></span>

| <span data-ttu-id="57920-132">名前</span><span class="sxs-lookup"><span data-stu-id="57920-132">Name</span></span>          | <span data-ttu-id="57920-133">説明</span><span class="sxs-lookup"><span data-stu-id="57920-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="57920-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="57920-134">Authorization</span></span> | <span data-ttu-id="57920-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="57920-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="57920-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="57920-137">If-None-Match</span></span> | <span data-ttu-id="57920-138">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="57920-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="57920-139">省略可能。</span><span class="sxs-lookup"><span data-stu-id="57920-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="57920-140">応答</span><span class="sxs-lookup"><span data-stu-id="57920-140">Response</span></span>

<span data-ttu-id="57920-141">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="57920-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="57920-142">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="57920-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="57920-143">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="57920-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="57920-144">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="57920-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="57920-145">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="57920-145">Report Refresh Date</span></span>
- <span data-ttu-id="57920-146">Windows</span><span class="sxs-lookup"><span data-stu-id="57920-146">Windows</span></span>
- <span data-ttu-id="57920-147">Windows スマートフォン</span><span class="sxs-lookup"><span data-stu-id="57920-147">Windows Phone</span></span>
- <span data-ttu-id="57920-148">Android スマートフォン</span><span class="sxs-lookup"><span data-stu-id="57920-148">Android Phone</span></span>
- <span data-ttu-id="57920-149">iPhone</span><span class="sxs-lookup"><span data-stu-id="57920-149">iPhone</span></span>
- <span data-ttu-id="57920-150">iPad</span><span class="sxs-lookup"><span data-stu-id="57920-150">iPad</span></span>
- <span data-ttu-id="57920-151">レポート日付</span><span class="sxs-lookup"><span data-stu-id="57920-151">Report Date</span></span>
- <span data-ttu-id="57920-152">レポート期間</span><span class="sxs-lookup"><span data-stu-id="57920-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="57920-153">例</span><span class="sxs-lookup"><span data-stu-id="57920-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="57920-154">要求</span><span class="sxs-lookup"><span data-stu-id="57920-154">Request</span></span>

<span data-ttu-id="57920-155">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="57920-155">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="57920-156">応答</span><span class="sxs-lookup"><span data-stu-id="57920-156">Response</span></span>

<span data-ttu-id="57920-157">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="57920-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="57920-158">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="57920-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Date,Report Period
```
