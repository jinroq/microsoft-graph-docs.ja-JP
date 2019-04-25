---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityUserCounts'
description: 一意のユーザー数と組織内のユーザーが開催、企画した電話会議セッションの数と種類に関する使用傾向を取得します。 会議セッションの種類には、IM、オーディオ/ビデオ、アプリケーション共有、Web、サード パーティへのダイヤルイン/ダイヤルアウト、Microsoft へのダイヤルイン/ダイヤルアウトなどがあります。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 513755bc878cbb3f9d80753e108448996759cda1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580884"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityusercounts"></a><span data-ttu-id="38dec-104">reportRoot: getSkypeForBusinessOrganizerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="38dec-104">reportRoot: getSkypeForBusinessOrganizerActivityUserCounts</span></span>

<span data-ttu-id="38dec-105">一意のユーザー数と組織内のユーザーが開催、企画した電話会議セッションの数と種類に関する使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="38dec-105">Get usage trends on the number of unique users and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="38dec-106">会議セッションの種類には、IM、オーディオ/ビデオ、アプリケーション共有、Web、サード パーティへのダイヤルイン/ダイヤルアウト、Microsoft へのダイヤルイン/ダイヤルアウトなどがあります。</span><span class="sxs-lookup"><span data-stu-id="38dec-106">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and dial-in/out Microsoft.</span></span>

> <span data-ttu-id="38dec-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business 電話会議の開催者のアクティビティ](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="38dec-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="38dec-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="38dec-108">Permissions</span></span>

<span data-ttu-id="38dec-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="38dec-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="38dec-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="38dec-111">Permission type</span></span>                        | <span data-ttu-id="38dec-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="38dec-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="38dec-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="38dec-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="38dec-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="38dec-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="38dec-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="38dec-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38dec-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="38dec-116">Not supported.</span></span>                           |
| <span data-ttu-id="38dec-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="38dec-117">Application</span></span>                            | <span data-ttu-id="38dec-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="38dec-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="38dec-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="38dec-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="38dec-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="38dec-120">Function parameters</span></span>

<span data-ttu-id="38dec-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="38dec-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="38dec-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="38dec-122">Parameter</span></span> | <span data-ttu-id="38dec-123">型</span><span class="sxs-lookup"><span data-stu-id="38dec-123">Type</span></span>   | <span data-ttu-id="38dec-124">説明</span><span class="sxs-lookup"><span data-stu-id="38dec-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="38dec-125">period</span><span class="sxs-lookup"><span data-stu-id="38dec-125">period</span></span>    | <span data-ttu-id="38dec-126">文字列</span><span class="sxs-lookup"><span data-stu-id="38dec-126">string</span></span> | <span data-ttu-id="38dec-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="38dec-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="38dec-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="38dec-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="38dec-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="38dec-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="38dec-130">必須。</span><span class="sxs-lookup"><span data-stu-id="38dec-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="38dec-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="38dec-131">Request headers</span></span>

| <span data-ttu-id="38dec-132">名前</span><span class="sxs-lookup"><span data-stu-id="38dec-132">Name</span></span>          | <span data-ttu-id="38dec-133">説明</span><span class="sxs-lookup"><span data-stu-id="38dec-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="38dec-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="38dec-134">Authorization</span></span> | <span data-ttu-id="38dec-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="38dec-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="38dec-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="38dec-137">If-None-Match</span></span> | <span data-ttu-id="38dec-138">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="38dec-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="38dec-139">省略可能。</span><span class="sxs-lookup"><span data-stu-id="38dec-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="38dec-140">応答</span><span class="sxs-lookup"><span data-stu-id="38dec-140">Response</span></span>

<span data-ttu-id="38dec-141">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="38dec-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="38dec-142">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="38dec-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="38dec-143">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="38dec-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="38dec-144">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="38dec-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="38dec-145">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="38dec-145">Report Refresh Date</span></span>
- <span data-ttu-id="38dec-146">レポート日付</span><span class="sxs-lookup"><span data-stu-id="38dec-146">Report Date</span></span>
- <span data-ttu-id="38dec-147">レポート期間</span><span class="sxs-lookup"><span data-stu-id="38dec-147">Report Period</span></span>
- <span data-ttu-id="38dec-148">IM</span><span class="sxs-lookup"><span data-stu-id="38dec-148">IM</span></span>
- <span data-ttu-id="38dec-149">オーディオ/ビデオ</span><span class="sxs-lookup"><span data-stu-id="38dec-149">Audio/Video</span></span>
- <span data-ttu-id="38dec-150">アプリ共有</span><span class="sxs-lookup"><span data-stu-id="38dec-150">App Sharing</span></span>
- <span data-ttu-id="38dec-151">Web</span><span class="sxs-lookup"><span data-stu-id="38dec-151">Web</span></span>
- <span data-ttu-id="38dec-152">サード パーティのダイヤルイン/アウト</span><span class="sxs-lookup"><span data-stu-id="38dec-152">Dial-in/out 3rd Party</span></span>
- <span data-ttu-id="38dec-153">Microsoft へのダイヤルイン/アウト</span><span class="sxs-lookup"><span data-stu-id="38dec-153">Dial-in/out Microsoft</span></span>

## <a name="example"></a><span data-ttu-id="38dec-154">例</span><span class="sxs-lookup"><span data-stu-id="38dec-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="38dec-155">要求</span><span class="sxs-lookup"><span data-stu-id="38dec-155">Request</span></span>

<span data-ttu-id="38dec-156">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="38dec-156">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessorganizeractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessOrganizerActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="38dec-157">応答</span><span class="sxs-lookup"><span data-stu-id="38dec-157">Response</span></span>

<span data-ttu-id="38dec-158">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="38dec-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="38dec-159">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="38dec-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party,Dial-in/out Microsoft
```
