---
title: 'reportRoot: getOffice365GroupsActivityGroupCounts'
description: グループの日次合計数と、そのうちのアクティブなグループの数を、電子メールでの会話、Yammer の投稿、SharePoint ファイルのアクティビティに基づいて取得します。
localization_priority: Normal
ms.openlocfilehash: 58d6bf33e5ab90693bb469da2fedce05b723f4f7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842869"
---
# <a name="reportroot-getoffice365groupsactivitygroupcounts"></a><span data-ttu-id="8da63-103">reportRoot: getOffice365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="8da63-103">reportRoot: getOffice365GroupsActivityGroupCounts</span></span>

<span data-ttu-id="8da63-104">グループの日次合計数と、そのうちのアクティブなグループの数を、電子メールでの会話、Yammer の投稿、SharePoint ファイルのアクティビティに基づいて取得します。</span><span class="sxs-lookup"><span data-stu-id="8da63-104">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span>

> <span data-ttu-id="8da63-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Office 365 グループ](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8da63-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="8da63-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8da63-106">Permissions</span></span>

<span data-ttu-id="8da63-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8da63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8da63-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8da63-109">Permission type</span></span>                        | <span data-ttu-id="8da63-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8da63-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8da63-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="8da63-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8da63-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8da63-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8da63-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8da63-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8da63-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8da63-114">Not supported.</span></span>                           |
| <span data-ttu-id="8da63-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8da63-115">Application</span></span>                            | <span data-ttu-id="8da63-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8da63-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8da63-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8da63-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityGroupCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="8da63-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="8da63-118">Function parameters</span></span>

<span data-ttu-id="8da63-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="8da63-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="8da63-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="8da63-120">Parameter</span></span> | <span data-ttu-id="8da63-121">Type</span><span class="sxs-lookup"><span data-stu-id="8da63-121">Type</span></span>   | <span data-ttu-id="8da63-122">説明</span><span class="sxs-lookup"><span data-stu-id="8da63-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8da63-123">period</span><span class="sxs-lookup"><span data-stu-id="8da63-123">period</span></span>    | <span data-ttu-id="8da63-124">文字列</span><span class="sxs-lookup"><span data-stu-id="8da63-124">string</span></span> | <span data-ttu-id="8da63-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="8da63-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8da63-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="8da63-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8da63-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="8da63-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="8da63-128">必須。</span><span class="sxs-lookup"><span data-stu-id="8da63-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="8da63-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8da63-129">Request headers</span></span>

| <span data-ttu-id="8da63-130">名前</span><span class="sxs-lookup"><span data-stu-id="8da63-130">Name</span></span>          | <span data-ttu-id="8da63-131">説明</span><span class="sxs-lookup"><span data-stu-id="8da63-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="8da63-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="8da63-132">Authorization</span></span> | <span data-ttu-id="8da63-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8da63-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="8da63-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="8da63-135">If-None-Match</span></span> | <span data-ttu-id="8da63-136">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="8da63-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="8da63-137">省略可能。</span><span class="sxs-lookup"><span data-stu-id="8da63-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="8da63-138">応答</span><span class="sxs-lookup"><span data-stu-id="8da63-138">Response</span></span>

<span data-ttu-id="8da63-139">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="8da63-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8da63-140">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="8da63-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8da63-141">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="8da63-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8da63-142">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="8da63-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8da63-143">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="8da63-143">Report Refresh Date</span></span>
- <span data-ttu-id="8da63-144">合計</span><span class="sxs-lookup"><span data-stu-id="8da63-144">Total</span></span>
- <span data-ttu-id="8da63-145">アクティブ</span><span class="sxs-lookup"><span data-stu-id="8da63-145">Active</span></span>
- <span data-ttu-id="8da63-146">レポート日付</span><span class="sxs-lookup"><span data-stu-id="8da63-146">Report Date</span></span>
- <span data-ttu-id="8da63-147">レポート期間</span><span class="sxs-lookup"><span data-stu-id="8da63-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="8da63-148">例</span><span class="sxs-lookup"><span data-stu-id="8da63-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8da63-149">要求</span><span class="sxs-lookup"><span data-stu-id="8da63-149">Request</span></span>

<span data-ttu-id="8da63-150">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8da63-150">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivitygroupcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityGroupCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="8da63-151">応答</span><span class="sxs-lookup"><span data-stu-id="8da63-151">Response</span></span>

<span data-ttu-id="8da63-152">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8da63-152">The following is an example of the response.</span></span>

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

<span data-ttu-id="8da63-153">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="8da63-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
```
