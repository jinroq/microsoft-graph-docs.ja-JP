---
title: 'reportRoot: getYammerGroupsActivityCounts'
description: グループ内で投稿、読み取り、および「いいね!」を付けた Yammer メッセージの数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d1509747798507d10588f05ebeb4d9b5efec2b97
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565864"
---
# <a name="reportroot-getyammergroupsactivitycounts"></a><span data-ttu-id="21dbb-103">reportRoot: getYammerGroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="21dbb-103">reportRoot: getYammerGroupsActivityCounts</span></span>

<span data-ttu-id="21dbb-104">グループ内で投稿、読み取り、および「いいね!」を付けた Yammer メッセージの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="21dbb-104">Get the number of Yammer messages posted, read, and liked in groups.</span></span>

> <span data-ttu-id="21dbb-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer グループ アクティビティ](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="21dbb-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="21dbb-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="21dbb-106">Permissions</span></span>

<span data-ttu-id="21dbb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="21dbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="21dbb-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="21dbb-109">Permission type</span></span>                        | <span data-ttu-id="21dbb-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="21dbb-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="21dbb-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="21dbb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="21dbb-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="21dbb-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="21dbb-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="21dbb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21dbb-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="21dbb-114">Not supported.</span></span>                           |
| <span data-ttu-id="21dbb-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="21dbb-115">Application</span></span>                            | <span data-ttu-id="21dbb-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="21dbb-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="21dbb-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="21dbb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="21dbb-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="21dbb-118">Function parameters</span></span>

<span data-ttu-id="21dbb-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="21dbb-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="21dbb-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="21dbb-120">Parameter</span></span> | <span data-ttu-id="21dbb-121">型</span><span class="sxs-lookup"><span data-stu-id="21dbb-121">Type</span></span>   | <span data-ttu-id="21dbb-122">説明</span><span class="sxs-lookup"><span data-stu-id="21dbb-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="21dbb-123">period</span><span class="sxs-lookup"><span data-stu-id="21dbb-123">period</span></span>    | <span data-ttu-id="21dbb-124">文字列</span><span class="sxs-lookup"><span data-stu-id="21dbb-124">string</span></span> | <span data-ttu-id="21dbb-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="21dbb-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="21dbb-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="21dbb-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="21dbb-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="21dbb-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="21dbb-128">必須。</span><span class="sxs-lookup"><span data-stu-id="21dbb-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="21dbb-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="21dbb-129">Request headers</span></span>

| <span data-ttu-id="21dbb-130">名前</span><span class="sxs-lookup"><span data-stu-id="21dbb-130">Name</span></span>          | <span data-ttu-id="21dbb-131">説明</span><span class="sxs-lookup"><span data-stu-id="21dbb-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="21dbb-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="21dbb-132">Authorization</span></span> | <span data-ttu-id="21dbb-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="21dbb-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="21dbb-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="21dbb-135">If-None-Match</span></span> | <span data-ttu-id="21dbb-136">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="21dbb-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="21dbb-137">省略可能。</span><span class="sxs-lookup"><span data-stu-id="21dbb-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="21dbb-138">応答</span><span class="sxs-lookup"><span data-stu-id="21dbb-138">Response</span></span>

<span data-ttu-id="21dbb-139">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="21dbb-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="21dbb-140">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="21dbb-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="21dbb-141">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="21dbb-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="21dbb-142">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="21dbb-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="21dbb-143">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="21dbb-143">Report Refresh Date</span></span>
- <span data-ttu-id="21dbb-144">いいね!</span><span class="sxs-lookup"><span data-stu-id="21dbb-144">Liked</span></span>
- <span data-ttu-id="21dbb-145">投稿</span><span class="sxs-lookup"><span data-stu-id="21dbb-145">Posted</span></span>
- <span data-ttu-id="21dbb-146">読み取り</span><span class="sxs-lookup"><span data-stu-id="21dbb-146">Read</span></span>
- <span data-ttu-id="21dbb-147">レポート日付</span><span class="sxs-lookup"><span data-stu-id="21dbb-147">Report Date</span></span>
- <span data-ttu-id="21dbb-148">レポート期間</span><span class="sxs-lookup"><span data-stu-id="21dbb-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="21dbb-149">例</span><span class="sxs-lookup"><span data-stu-id="21dbb-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="21dbb-150">要求</span><span class="sxs-lookup"><span data-stu-id="21dbb-150">Request</span></span>

<span data-ttu-id="21dbb-151">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="21dbb-151">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="21dbb-152">応答</span><span class="sxs-lookup"><span data-stu-id="21dbb-152">Response</span></span>

<span data-ttu-id="21dbb-153">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="21dbb-153">The following is an example of the response.</span></span>

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

<span data-ttu-id="21dbb-154">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="21dbb-154">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
```
