---
title: 'reportRoot: getOneDriveActivityUserDetail'
description: ユーザー別の OneDrive アクティビティに関する詳細を取得します。
ms.openlocfilehash: 43d16f9e71a2d2ab2535c206c39f3a09b4c391e9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021517"
---
# <a name="reportroot-getonedriveactivityuserdetail"></a><span data-ttu-id="493e7-103">reportRoot: getOneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="493e7-103">reportRoot: getOneDriveActivityUserDetail</span></span>

<span data-ttu-id="493e7-104">ユーザー別の OneDrive アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="493e7-104">Get details about OneDrive activity by user.</span></span>

> <span data-ttu-id="493e7-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business のアクティビティ](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="493e7-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="493e7-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="493e7-106">Permissions</span></span>

<span data-ttu-id="493e7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="493e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="493e7-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="493e7-109">Permission type</span></span>                        | <span data-ttu-id="493e7-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="493e7-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="493e7-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="493e7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="493e7-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="493e7-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="493e7-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="493e7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="493e7-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="493e7-114">Not supported.</span></span>                           |
| <span data-ttu-id="493e7-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="493e7-115">Application</span></span>                            | <span data-ttu-id="493e7-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="493e7-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="493e7-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="493e7-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOneDriveActivityUserDetail(period='{period_value}')
GET /reports/getOneDriveActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="493e7-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="493e7-118">Function parameters</span></span>

<span data-ttu-id="493e7-119">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="493e7-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="493e7-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="493e7-120">Parameter</span></span> | <span data-ttu-id="493e7-121">型</span><span class="sxs-lookup"><span data-stu-id="493e7-121">Type</span></span>   | <span data-ttu-id="493e7-122">説明</span><span class="sxs-lookup"><span data-stu-id="493e7-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="493e7-123">period</span><span class="sxs-lookup"><span data-stu-id="493e7-123">period</span></span>    | <span data-ttu-id="493e7-124">文字列</span><span class="sxs-lookup"><span data-stu-id="493e7-124">string</span></span> | <span data-ttu-id="493e7-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="493e7-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="493e7-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="493e7-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="493e7-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="493e7-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="493e7-128">date</span><span class="sxs-lookup"><span data-stu-id="493e7-128">date</span></span>      | <span data-ttu-id="493e7-129">日付</span><span class="sxs-lookup"><span data-stu-id="493e7-129">Date</span></span>   | <span data-ttu-id="493e7-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="493e7-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="493e7-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="493e7-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="493e7-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="493e7-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="493e7-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="493e7-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="493e7-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="493e7-134">Request headers</span></span>

| <span data-ttu-id="493e7-135">名前</span><span class="sxs-lookup"><span data-stu-id="493e7-135">Name</span></span>          | <span data-ttu-id="493e7-136">説明</span><span class="sxs-lookup"><span data-stu-id="493e7-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="493e7-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="493e7-137">Authorization</span></span> | <span data-ttu-id="493e7-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="493e7-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="493e7-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="493e7-140">If-None-Match</span></span> | <span data-ttu-id="493e7-141">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="493e7-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="493e7-142">省略可能。</span><span class="sxs-lookup"><span data-stu-id="493e7-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="493e7-143">応答</span><span class="sxs-lookup"><span data-stu-id="493e7-143">Response</span></span>

<span data-ttu-id="493e7-144">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="493e7-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="493e7-145">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="493e7-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="493e7-146">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="493e7-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="493e7-147">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="493e7-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="493e7-148">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="493e7-148">Report Refresh Date</span></span>
- <span data-ttu-id="493e7-149">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="493e7-149">User Principal Name</span></span>
- <span data-ttu-id="493e7-150">削除済み</span><span class="sxs-lookup"><span data-stu-id="493e7-150">Is Deleted</span></span>
- <span data-ttu-id="493e7-151">削除日</span><span class="sxs-lookup"><span data-stu-id="493e7-151">Deleted Date</span></span>
- <span data-ttu-id="493e7-152">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="493e7-152">Last Activity Date</span></span>
- <span data-ttu-id="493e7-153">表示済みまたは編集済みファイルの数</span><span class="sxs-lookup"><span data-stu-id="493e7-153">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="493e7-154">同期済みファイルの数</span><span class="sxs-lookup"><span data-stu-id="493e7-154">Synced File Count</span></span>
- <span data-ttu-id="493e7-155">社内で共有済みファイルの数</span><span class="sxs-lookup"><span data-stu-id="493e7-155">Shared Internally File Count</span></span>
- <span data-ttu-id="493e7-156">外部で共有済みファイルの数</span><span class="sxs-lookup"><span data-stu-id="493e7-156">Shared Externally File Count</span></span>
- <span data-ttu-id="493e7-157">割り当て済み製品</span><span class="sxs-lookup"><span data-stu-id="493e7-157">Assigned Products</span></span>
- <span data-ttu-id="493e7-158">レポート期間</span><span class="sxs-lookup"><span data-stu-id="493e7-158">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="493e7-159">例</span><span class="sxs-lookup"><span data-stu-id="493e7-159">Example</span></span>

#### <a name="request"></a><span data-ttu-id="493e7-160">要求</span><span class="sxs-lookup"><span data-stu-id="493e7-160">Request</span></span>

<span data-ttu-id="493e7-161">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="493e7-161">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="493e7-162">応答</span><span class="sxs-lookup"><span data-stu-id="493e7-162">Response</span></span>

<span data-ttu-id="493e7-163">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="493e7-163">The following is an example of the response.</span></span>

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

<span data-ttu-id="493e7-164">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="493e7-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Assigned Products,Report Period
```
