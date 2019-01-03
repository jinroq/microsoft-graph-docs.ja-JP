---
title: 'reportRoot: getSkypeForBusinessActivityUserCounts'
description: Skype for Business を介して組織内で行われた会議セッションにおける、それぞれ別個の開催ユーザー数と参加ユーザー数の傾向を取得します。 レポートには、ピア ツー ピア セッションの数も含まれます。
ms.openlocfilehash: 9a797d9af29d9964c2b1797f82be2c28893337d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022419"
---
# <a name="reportroot-getskypeforbusinessactivityusercounts"></a><span data-ttu-id="f10ab-104">reportRoot: getSkypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="f10ab-104">reportRoot: getSkypeForBusinessActivityUserCounts</span></span>

<span data-ttu-id="f10ab-105">Skype for Business を介して組織内で行われた会議セッションにおける、それぞれ別個の開催ユーザー数と参加ユーザー数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="f10ab-105">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="f10ab-106">レポートには、ピア ツー ピア セッションの数も含まれます。</span><span class="sxs-lookup"><span data-stu-id="f10ab-106">The report also includes the number of peer-to-peer sessions.</span></span>

> <span data-ttu-id="f10ab-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business アクティビティ](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f10ab-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="f10ab-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f10ab-108">Permissions</span></span>

<span data-ttu-id="f10ab-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f10ab-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f10ab-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f10ab-111">Permission type</span></span>                        | <span data-ttu-id="f10ab-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f10ab-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f10ab-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="f10ab-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f10ab-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f10ab-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f10ab-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f10ab-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f10ab-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f10ab-116">Not supported.</span></span>                           |
| <span data-ttu-id="f10ab-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f10ab-117">Application</span></span>                            | <span data-ttu-id="f10ab-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f10ab-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f10ab-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f10ab-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f10ab-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="f10ab-120">Function parameters</span></span>

<span data-ttu-id="f10ab-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="f10ab-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f10ab-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f10ab-122">Parameter</span></span> | <span data-ttu-id="f10ab-123">型</span><span class="sxs-lookup"><span data-stu-id="f10ab-123">Type</span></span>   | <span data-ttu-id="f10ab-124">説明</span><span class="sxs-lookup"><span data-stu-id="f10ab-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f10ab-125">period</span><span class="sxs-lookup"><span data-stu-id="f10ab-125">period</span></span>    | <span data-ttu-id="f10ab-126">文字列</span><span class="sxs-lookup"><span data-stu-id="f10ab-126">string</span></span> | <span data-ttu-id="f10ab-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="f10ab-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f10ab-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="f10ab-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f10ab-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="f10ab-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f10ab-130">必須。</span><span class="sxs-lookup"><span data-stu-id="f10ab-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f10ab-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f10ab-131">Request headers</span></span>

| <span data-ttu-id="f10ab-132">名前</span><span class="sxs-lookup"><span data-stu-id="f10ab-132">Name</span></span>          | <span data-ttu-id="f10ab-133">説明</span><span class="sxs-lookup"><span data-stu-id="f10ab-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="f10ab-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="f10ab-134">Authorization</span></span> | <span data-ttu-id="f10ab-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f10ab-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="f10ab-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="f10ab-137">If-None-Match</span></span> | <span data-ttu-id="f10ab-138">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="f10ab-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="f10ab-139">省略可能。</span><span class="sxs-lookup"><span data-stu-id="f10ab-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="f10ab-140">応答</span><span class="sxs-lookup"><span data-stu-id="f10ab-140">Response</span></span>

<span data-ttu-id="f10ab-141">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="f10ab-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f10ab-142">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="f10ab-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f10ab-143">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="f10ab-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f10ab-144">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="f10ab-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f10ab-145">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="f10ab-145">Report Refresh Date</span></span>
- <span data-ttu-id="f10ab-146">レポート日付</span><span class="sxs-lookup"><span data-stu-id="f10ab-146">Report Date</span></span>
- <span data-ttu-id="f10ab-147">レポート期間</span><span class="sxs-lookup"><span data-stu-id="f10ab-147">Report Period</span></span>
- <span data-ttu-id="f10ab-148">ピアツーピア</span><span class="sxs-lookup"><span data-stu-id="f10ab-148">Peer-to-peer</span></span>
- <span data-ttu-id="f10ab-149">開催</span><span class="sxs-lookup"><span data-stu-id="f10ab-149">Organized</span></span>
- <span data-ttu-id="f10ab-150">参加</span><span class="sxs-lookup"><span data-stu-id="f10ab-150">Participated</span></span>

## <a name="example"></a><span data-ttu-id="f10ab-151">例</span><span class="sxs-lookup"><span data-stu-id="f10ab-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f10ab-152">要求</span><span class="sxs-lookup"><span data-stu-id="f10ab-152">Request</span></span>

<span data-ttu-id="f10ab-153">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f10ab-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessactivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="f10ab-154">応答</span><span class="sxs-lookup"><span data-stu-id="f10ab-154">Response</span></span>

<span data-ttu-id="f10ab-155">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f10ab-155">The following is an example of the response.</span></span>

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

<span data-ttu-id="f10ab-156">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="f10ab-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Peer-to-peer,Organized,Participated
```