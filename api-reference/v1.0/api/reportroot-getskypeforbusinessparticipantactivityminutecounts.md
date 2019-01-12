---
title: 'reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts'
description: 組織からユーザーが参加した会議セッションの長さ (分) と種類について、使用傾向を取得します。 会議セッションの種類には、オーディオ/ビデオがあります。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 230807a0494ad52a1b93113e88abcf9302d24754
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920605"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityminutecounts"></a><span data-ttu-id="ea85f-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="ea85f-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span></span>

<span data-ttu-id="ea85f-105">組織からユーザーが参加した会議セッションの長さ (分) と種類について、使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="ea85f-105">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="ea85f-106">会議セッションの種類には、オーディオ/ビデオがあります。</span><span class="sxs-lookup"><span data-stu-id="ea85f-106">Types of conference sessions include audio/video.</span></span>

> <span data-ttu-id="ea85f-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business 電話会議の参加者のアクティビティ](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ea85f-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="ea85f-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ea85f-108">Permissions</span></span>

<span data-ttu-id="ea85f-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ea85f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ea85f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ea85f-111">Permission type</span></span>                        | <span data-ttu-id="ea85f-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ea85f-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ea85f-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="ea85f-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ea85f-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea85f-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ea85f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ea85f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea85f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ea85f-116">Not supported.</span></span>                           |
| <span data-ttu-id="ea85f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ea85f-117">Application</span></span>                            | <span data-ttu-id="ea85f-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea85f-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ea85f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ea85f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ea85f-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="ea85f-120">Function parameters</span></span>

<span data-ttu-id="ea85f-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="ea85f-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ea85f-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ea85f-122">Parameter</span></span> | <span data-ttu-id="ea85f-123">型</span><span class="sxs-lookup"><span data-stu-id="ea85f-123">Type</span></span>   | <span data-ttu-id="ea85f-124">説明</span><span class="sxs-lookup"><span data-stu-id="ea85f-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ea85f-125">period</span><span class="sxs-lookup"><span data-stu-id="ea85f-125">period</span></span>    | <span data-ttu-id="ea85f-126">文字列</span><span class="sxs-lookup"><span data-stu-id="ea85f-126">string</span></span> | <span data-ttu-id="ea85f-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="ea85f-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ea85f-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="ea85f-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ea85f-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="ea85f-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ea85f-130">必須。</span><span class="sxs-lookup"><span data-stu-id="ea85f-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="ea85f-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ea85f-131">Request headers</span></span>

| <span data-ttu-id="ea85f-132">名前</span><span class="sxs-lookup"><span data-stu-id="ea85f-132">Name</span></span>          | <span data-ttu-id="ea85f-133">説明</span><span class="sxs-lookup"><span data-stu-id="ea85f-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="ea85f-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea85f-134">Authorization</span></span> | <span data-ttu-id="ea85f-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ea85f-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="ea85f-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="ea85f-137">If-None-Match</span></span> | <span data-ttu-id="ea85f-138">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="ea85f-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="ea85f-139">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ea85f-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="ea85f-140">応答</span><span class="sxs-lookup"><span data-stu-id="ea85f-140">Response</span></span>

<span data-ttu-id="ea85f-141">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="ea85f-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ea85f-142">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="ea85f-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ea85f-143">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="ea85f-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ea85f-144">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="ea85f-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ea85f-145">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="ea85f-145">Report Refresh Date</span></span>
- <span data-ttu-id="ea85f-146">レポート日付</span><span class="sxs-lookup"><span data-stu-id="ea85f-146">Report Date</span></span>
- <span data-ttu-id="ea85f-147">レポート期間</span><span class="sxs-lookup"><span data-stu-id="ea85f-147">Report Period</span></span>
- <span data-ttu-id="ea85f-148">オーディオ/ビデオ</span><span class="sxs-lookup"><span data-stu-id="ea85f-148">Audio/Video</span></span>

## <a name="example"></a><span data-ttu-id="ea85f-149">例</span><span class="sxs-lookup"><span data-stu-id="ea85f-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ea85f-150">要求</span><span class="sxs-lookup"><span data-stu-id="ea85f-150">Request</span></span>

<span data-ttu-id="ea85f-151">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ea85f-151">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessparticipantactivityminutecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="ea85f-152">応答</span><span class="sxs-lookup"><span data-stu-id="ea85f-152">Response</span></span>

<span data-ttu-id="ea85f-153">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ea85f-153">The following is an example of the response.</span></span>

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

<span data-ttu-id="ea85f-154">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="ea85f-154">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video
```
