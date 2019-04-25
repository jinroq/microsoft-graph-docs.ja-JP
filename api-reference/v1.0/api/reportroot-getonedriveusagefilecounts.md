---
title: 'reportRoot: getOneDriveUsageFileCounts'
description: すべてのサイトのファイル合計数と、アクティブ ファイルの数を取得します。 ファイルは一定期間中に保存、同期、変更、共有されるとアクティブとみなされます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: ddc7bb25a746630320a93ecf546a7299900f09c6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525559"
---
# <a name="reportroot-getonedriveusagefilecounts"></a><span data-ttu-id="5695e-104">reportRoot: getOneDriveUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="5695e-104">reportRoot: getOneDriveUsageFileCounts</span></span>

<span data-ttu-id="5695e-105">すべてのサイトのファイル合計数と、アクティブ ファイルの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="5695e-105">Get the total number of files across all sites and how many are active files.</span></span> <span data-ttu-id="5695e-106">ファイルは一定期間中に保存、同期、変更、共有されるとアクティブとみなされます。</span><span class="sxs-lookup"><span data-stu-id="5695e-106">A file is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="5695e-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business の使用状況](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5695e-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="5695e-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5695e-108">Permissions</span></span>

<span data-ttu-id="5695e-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5695e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5695e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5695e-111">Permission type</span></span>                        | <span data-ttu-id="5695e-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5695e-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5695e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5695e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="5695e-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5695e-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5695e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5695e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5695e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5695e-116">Not supported.</span></span>                           |
| <span data-ttu-id="5695e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5695e-117">Application</span></span>                            | <span data-ttu-id="5695e-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5695e-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5695e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5695e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="5695e-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="5695e-120">Function parameters</span></span>

<span data-ttu-id="5695e-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="5695e-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5695e-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="5695e-122">Parameter</span></span> | <span data-ttu-id="5695e-123">型</span><span class="sxs-lookup"><span data-stu-id="5695e-123">Type</span></span>   | <span data-ttu-id="5695e-124">説明</span><span class="sxs-lookup"><span data-stu-id="5695e-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5695e-125">period</span><span class="sxs-lookup"><span data-stu-id="5695e-125">period</span></span>    | <span data-ttu-id="5695e-126">文字列</span><span class="sxs-lookup"><span data-stu-id="5695e-126">string</span></span> | <span data-ttu-id="5695e-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="5695e-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5695e-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="5695e-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5695e-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="5695e-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5695e-130">必須。</span><span class="sxs-lookup"><span data-stu-id="5695e-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="5695e-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5695e-131">Request headers</span></span>

| <span data-ttu-id="5695e-132">名前</span><span class="sxs-lookup"><span data-stu-id="5695e-132">Name</span></span>          | <span data-ttu-id="5695e-133">説明</span><span class="sxs-lookup"><span data-stu-id="5695e-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="5695e-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="5695e-134">Authorization</span></span> | <span data-ttu-id="5695e-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5695e-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="5695e-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="5695e-137">If-None-Match</span></span> | <span data-ttu-id="5695e-138">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="5695e-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="5695e-139">省略可能。</span><span class="sxs-lookup"><span data-stu-id="5695e-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="5695e-140">応答</span><span class="sxs-lookup"><span data-stu-id="5695e-140">Response</span></span>

<span data-ttu-id="5695e-141">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="5695e-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5695e-142">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="5695e-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5695e-143">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="5695e-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5695e-144">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="5695e-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5695e-145">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="5695e-145">Report Refresh Date</span></span>
- <span data-ttu-id="5695e-146">サイトの種類</span><span class="sxs-lookup"><span data-stu-id="5695e-146">Site Type</span></span>
- <span data-ttu-id="5695e-147">合計</span><span class="sxs-lookup"><span data-stu-id="5695e-147">Total</span></span>
- <span data-ttu-id="5695e-148">アクティブ</span><span class="sxs-lookup"><span data-stu-id="5695e-148">Active</span></span>
- <span data-ttu-id="5695e-149">レポート日付</span><span class="sxs-lookup"><span data-stu-id="5695e-149">Report Date</span></span>
- <span data-ttu-id="5695e-150">レポート期間</span><span class="sxs-lookup"><span data-stu-id="5695e-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="5695e-151">例</span><span class="sxs-lookup"><span data-stu-id="5695e-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5695e-152">要求</span><span class="sxs-lookup"><span data-stu-id="5695e-152">Request</span></span>

<span data-ttu-id="5695e-153">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5695e-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveusagefilecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageFileCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="5695e-154">応答</span><span class="sxs-lookup"><span data-stu-id="5695e-154">Response</span></span>

<span data-ttu-id="5695e-155">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5695e-155">The following is an example of the response.</span></span>

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

<span data-ttu-id="5695e-156">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="5695e-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```
