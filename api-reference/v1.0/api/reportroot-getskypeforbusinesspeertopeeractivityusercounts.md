---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts'
description: 組織内で実施されたピア ツー ピア セッションの一意のユーザー数と種類について、使用傾向を取得します。 ピア ツー ピア セッションでのセッションの種類には IM、オーディオ、ビデオ、アプリケーション共有、ファイル転送があります。
localization_priority: Normal
ms.openlocfilehash: 84402088f6b5557520e1a12888afa2060c01035c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821204"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityusercounts"></a><span data-ttu-id="eb079-104">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="eb079-104">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span></span>

<span data-ttu-id="eb079-105">組織内で実施されたピア ツー ピア セッションの一意のユーザー数と種類について、使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="eb079-105">Get usage trends on the number of unique users and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="eb079-106">ピア ツー ピア セッションでのセッションの種類には IM、オーディオ、ビデオ、アプリケーション共有、ファイル転送があります。</span><span class="sxs-lookup"><span data-stu-id="eb079-106">Types of sessions include IM, audio, video, application sharing, and file transfers in peer-to-peer sessions.</span></span>

> <span data-ttu-id="eb079-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business ピア ツー ピア アクティビティ](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eb079-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="eb079-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="eb079-108">Permissions</span></span>

<span data-ttu-id="eb079-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eb079-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eb079-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eb079-111">Permission type</span></span>                        | <span data-ttu-id="eb079-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="eb079-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="eb079-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="eb079-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="eb079-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb079-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="eb079-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eb079-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb079-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eb079-116">Not supported.</span></span>                           |
| <span data-ttu-id="eb079-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eb079-117">Application</span></span>                            | <span data-ttu-id="eb079-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb079-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="eb079-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eb079-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="eb079-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="eb079-120">Function parameters</span></span>

<span data-ttu-id="eb079-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="eb079-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="eb079-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="eb079-122">Parameter</span></span> | <span data-ttu-id="eb079-123">Type</span><span class="sxs-lookup"><span data-stu-id="eb079-123">Type</span></span>   | <span data-ttu-id="eb079-124">説明</span><span class="sxs-lookup"><span data-stu-id="eb079-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="eb079-125">period</span><span class="sxs-lookup"><span data-stu-id="eb079-125">period</span></span>    | <span data-ttu-id="eb079-126">文字列</span><span class="sxs-lookup"><span data-stu-id="eb079-126">string</span></span> | <span data-ttu-id="eb079-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="eb079-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="eb079-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="eb079-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="eb079-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="eb079-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="eb079-130">必須。</span><span class="sxs-lookup"><span data-stu-id="eb079-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="eb079-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eb079-131">Request headers</span></span>

| <span data-ttu-id="eb079-132">名前</span><span class="sxs-lookup"><span data-stu-id="eb079-132">Name</span></span>          | <span data-ttu-id="eb079-133">説明</span><span class="sxs-lookup"><span data-stu-id="eb079-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="eb079-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb079-134">Authorization</span></span> | <span data-ttu-id="eb079-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="eb079-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="eb079-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="eb079-137">If-None-Match</span></span> | <span data-ttu-id="eb079-138">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="eb079-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="eb079-139">省略可能。</span><span class="sxs-lookup"><span data-stu-id="eb079-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="eb079-140">応答</span><span class="sxs-lookup"><span data-stu-id="eb079-140">Response</span></span>

<span data-ttu-id="eb079-141">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="eb079-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="eb079-142">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="eb079-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="eb079-143">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="eb079-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="eb079-144">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="eb079-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="eb079-145">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="eb079-145">Report Refresh Date</span></span>
- <span data-ttu-id="eb079-146">レポート日付</span><span class="sxs-lookup"><span data-stu-id="eb079-146">Report Date</span></span>
- <span data-ttu-id="eb079-147">レポート期間</span><span class="sxs-lookup"><span data-stu-id="eb079-147">Report Period</span></span>
- <span data-ttu-id="eb079-148">IM</span><span class="sxs-lookup"><span data-stu-id="eb079-148">IM</span></span>
- <span data-ttu-id="eb079-149">オーディオ</span><span class="sxs-lookup"><span data-stu-id="eb079-149">Audio</span></span>
- <span data-ttu-id="eb079-150">ビデオ</span><span class="sxs-lookup"><span data-stu-id="eb079-150">Video</span></span>
- <span data-ttu-id="eb079-151">アプリ共有</span><span class="sxs-lookup"><span data-stu-id="eb079-151">App Sharing</span></span>
- <span data-ttu-id="eb079-152">ファイル転送</span><span class="sxs-lookup"><span data-stu-id="eb079-152">File Transfer</span></span>

## <a name="example"></a><span data-ttu-id="eb079-153">例</span><span class="sxs-lookup"><span data-stu-id="eb079-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="eb079-154">要求</span><span class="sxs-lookup"><span data-stu-id="eb079-154">Request</span></span>

<span data-ttu-id="eb079-155">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="eb079-155">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinesspeertopeeractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="eb079-156">応答</span><span class="sxs-lookup"><span data-stu-id="eb079-156">Response</span></span>

<span data-ttu-id="eb079-157">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="eb079-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="eb079-158">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="eb079-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio,Video,App Sharing,File Transfer
```
