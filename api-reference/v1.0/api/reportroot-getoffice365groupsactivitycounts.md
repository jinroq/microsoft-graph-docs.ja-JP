---
title: 'reportRoot: getOffice365GroupsActivityCounts'
description: グループ ワークロード全体のグループ活動の数を取得します。
localization_priority: Normal
ms.openlocfilehash: d63655d136acee1d5d911e8e7b437560826043cf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846173"
---
# <a name="reportroot-getoffice365groupsactivitycounts"></a><span data-ttu-id="ad8b5-103">reportRoot: getOffice365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="ad8b5-103">reportRoot: getOffice365GroupsActivityCounts</span></span>

<span data-ttu-id="ad8b5-104">グループ ワークロード全体のグループ活動の数を取得します。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-104">Get the number of group activities across group workloads.</span></span>

> <span data-ttu-id="ad8b5-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Office 365 グループ](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="ad8b5-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ad8b5-106">Permissions</span></span>

<span data-ttu-id="ad8b5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ad8b5-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ad8b5-109">Permission type</span></span>                        | <span data-ttu-id="ad8b5-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ad8b5-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ad8b5-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="ad8b5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ad8b5-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad8b5-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ad8b5-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ad8b5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad8b5-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-114">Not supported.</span></span>                           |
| <span data-ttu-id="ad8b5-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ad8b5-115">Application</span></span>                            | <span data-ttu-id="ad8b5-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad8b5-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ad8b5-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ad8b5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ad8b5-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="ad8b5-118">Function parameters</span></span>

<span data-ttu-id="ad8b5-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ad8b5-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ad8b5-120">Parameter</span></span> | <span data-ttu-id="ad8b5-121">Type</span><span class="sxs-lookup"><span data-stu-id="ad8b5-121">Type</span></span>   | <span data-ttu-id="ad8b5-122">説明</span><span class="sxs-lookup"><span data-stu-id="ad8b5-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ad8b5-123">period</span><span class="sxs-lookup"><span data-stu-id="ad8b5-123">period</span></span>    | <span data-ttu-id="ad8b5-124">文字列</span><span class="sxs-lookup"><span data-stu-id="ad8b5-124">string</span></span> | <span data-ttu-id="ad8b5-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ad8b5-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ad8b5-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ad8b5-128">必須。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="ad8b5-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad8b5-129">Request headers</span></span>

| <span data-ttu-id="ad8b5-130">名前</span><span class="sxs-lookup"><span data-stu-id="ad8b5-130">Name</span></span>          | <span data-ttu-id="ad8b5-131">説明</span><span class="sxs-lookup"><span data-stu-id="ad8b5-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="ad8b5-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad8b5-132">Authorization</span></span> | <span data-ttu-id="ad8b5-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="ad8b5-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="ad8b5-135">If-None-Match</span></span> | <span data-ttu-id="ad8b5-136">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="ad8b5-137">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="ad8b5-138">応答</span><span class="sxs-lookup"><span data-stu-id="ad8b5-138">Response</span></span>

<span data-ttu-id="ad8b5-139">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ad8b5-140">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ad8b5-141">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ad8b5-142">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ad8b5-143">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="ad8b5-143">Report Refresh Date</span></span>
- <span data-ttu-id="ad8b5-144">受信した Exchange の電子メール</span><span class="sxs-lookup"><span data-stu-id="ad8b5-144">Exchange Emails Received</span></span>
- <span data-ttu-id="ad8b5-145">投稿された Yammer メッセージ</span><span class="sxs-lookup"><span data-stu-id="ad8b5-145">Yammer Messages Posted</span></span>
- <span data-ttu-id="ad8b5-146">読み取られた Yammer メッセージ</span><span class="sxs-lookup"><span data-stu-id="ad8b5-146">Yammer Messages Read</span></span>
- <span data-ttu-id="ad8b5-147">「いいね!」された Yammer メッセージ</span><span class="sxs-lookup"><span data-stu-id="ad8b5-147">Yammer Messages Liked</span></span>
- <span data-ttu-id="ad8b5-148">レポート日付</span><span class="sxs-lookup"><span data-stu-id="ad8b5-148">Report Date</span></span>
- <span data-ttu-id="ad8b5-149">レポート期間</span><span class="sxs-lookup"><span data-stu-id="ad8b5-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="ad8b5-150">例</span><span class="sxs-lookup"><span data-stu-id="ad8b5-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ad8b5-151">要求</span><span class="sxs-lookup"><span data-stu-id="ad8b5-151">Request</span></span>

<span data-ttu-id="ad8b5-152">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="ad8b5-153">応答</span><span class="sxs-lookup"><span data-stu-id="ad8b5-153">Response</span></span>

<span data-ttu-id="ad8b5-154">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="ad8b5-155">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Emails Received,Yammer Messages Posted,Yammer Messages Read,Yammer Messages Liked,Report Date,Report Period
```
