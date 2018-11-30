---
title: 'reportRoot: getTeamsUserActivityCounts'
description: アクティビティの種類ごとに、Microsoft Teams アクティビティの数を取得します。 アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話および会議です。
ms.openlocfilehash: 58d0ddd884fed70e9fc5cbdd1c3d97c8a5463ccc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023811"
---
# <a name="reportroot-getteamsuseractivitycounts"></a><span data-ttu-id="356a3-104">reportRoot: getTeamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="356a3-104">reportRoot: getTeamsUserActivityCounts</span></span>

<span data-ttu-id="356a3-105">アクティビティの種類ごとに、Microsoft Teams アクティビティの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="356a3-105">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="356a3-106">アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話および会議です。</span><span class="sxs-lookup"><span data-stu-id="356a3-106">The activity types are team chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="356a3-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="356a3-107">Permissions</span></span>

<span data-ttu-id="356a3-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="356a3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="356a3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="356a3-110">Permission type</span></span>                        | <span data-ttu-id="356a3-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="356a3-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="356a3-112">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="356a3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="356a3-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="356a3-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="356a3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="356a3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="356a3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="356a3-115">Not supported.</span></span>                           |
| <span data-ttu-id="356a3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="356a3-116">Application</span></span>                            | <span data-ttu-id="356a3-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="356a3-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="356a3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="356a3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="356a3-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="356a3-119">Function parameters</span></span>

<span data-ttu-id="356a3-120">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="356a3-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="356a3-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="356a3-121">Parameter</span></span> | <span data-ttu-id="356a3-122">型</span><span class="sxs-lookup"><span data-stu-id="356a3-122">Type</span></span>   | <span data-ttu-id="356a3-123">説明</span><span class="sxs-lookup"><span data-stu-id="356a3-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="356a3-124">period</span><span class="sxs-lookup"><span data-stu-id="356a3-124">period</span></span>    | <span data-ttu-id="356a3-125">文字列</span><span class="sxs-lookup"><span data-stu-id="356a3-125">string</span></span> | <span data-ttu-id="356a3-126">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="356a3-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="356a3-127">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="356a3-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="356a3-128">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="356a3-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="356a3-129">必須。</span><span class="sxs-lookup"><span data-stu-id="356a3-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="356a3-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="356a3-130">Request headers</span></span>

| <span data-ttu-id="356a3-131">名前</span><span class="sxs-lookup"><span data-stu-id="356a3-131">Name</span></span>          | <span data-ttu-id="356a3-132">説明</span><span class="sxs-lookup"><span data-stu-id="356a3-132">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="356a3-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="356a3-133">Authorization</span></span> | <span data-ttu-id="356a3-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="356a3-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="356a3-136">応答</span><span class="sxs-lookup"><span data-stu-id="356a3-136">Response</span></span>

<span data-ttu-id="356a3-137">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="356a3-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="356a3-138">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="356a3-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="356a3-139">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="356a3-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="356a3-140">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="356a3-140">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="356a3-141">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="356a3-141">Report Refresh Date</span></span>
- <span data-ttu-id="356a3-142">レポート日付</span><span class="sxs-lookup"><span data-stu-id="356a3-142">Report Date</span></span>
- <span data-ttu-id="356a3-143">チーム チャット メッセージ</span><span class="sxs-lookup"><span data-stu-id="356a3-143">Team Chat Messages</span></span>
- <span data-ttu-id="356a3-144">非公開チャット メッセージ</span><span class="sxs-lookup"><span data-stu-id="356a3-144">Private Chat Messages</span></span>
- <span data-ttu-id="356a3-145">通話</span><span class="sxs-lookup"><span data-stu-id="356a3-145">Calls</span></span>
- <span data-ttu-id="356a3-146">会議</span><span class="sxs-lookup"><span data-stu-id="356a3-146">Meetings</span></span>
- <span data-ttu-id="356a3-147">レポート期間</span><span class="sxs-lookup"><span data-stu-id="356a3-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="356a3-148">例</span><span class="sxs-lookup"><span data-stu-id="356a3-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="356a3-149">要求</span><span class="sxs-lookup"><span data-stu-id="356a3-149">Request</span></span>

<span data-ttu-id="356a3-150">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="356a3-150">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="356a3-151">応答</span><span class="sxs-lookup"><span data-stu-id="356a3-151">Response</span></span>

<span data-ttu-id="356a3-152">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="356a3-152">The following is an example of the response.</span></span>

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
<span data-ttu-id="356a3-153">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="356a3-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Report Period
```