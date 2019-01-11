---
title: 'reportRoot: getSharePointActivityFileCounts'
description: SharePoint サイトに保存されているファイルを操作した、それぞれ別個のライセンス ユーザーの数を取得します。
localization_priority: Normal
ms.openlocfilehash: 46e522b620fed3f7a9da3b4d8e707f38abc07817
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853187"
---
# <a name="reportroot-getsharepointactivityfilecounts"></a><span data-ttu-id="fe392-103">reportRoot: getSharePointActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="fe392-103">reportRoot: getSharePointActivityFileCounts</span></span>

<span data-ttu-id="fe392-104">SharePoint サイトに保存されているファイルを操作した、それぞれ別個のライセンス ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="fe392-104">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span>

> <span data-ttu-id="fe392-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint アクティビティ](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe392-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="fe392-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fe392-106">Permissions</span></span>

<span data-ttu-id="fe392-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe392-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fe392-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fe392-109">Permission type</span></span>                        | <span data-ttu-id="fe392-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fe392-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="fe392-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="fe392-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fe392-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe392-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="fe392-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fe392-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe392-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe392-114">Not supported.</span></span>                           |
| <span data-ttu-id="fe392-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fe392-115">Application</span></span>                            | <span data-ttu-id="fe392-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe392-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="fe392-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fe392-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="fe392-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="fe392-118">Function parameters</span></span>

<span data-ttu-id="fe392-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="fe392-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="fe392-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="fe392-120">Parameter</span></span> | <span data-ttu-id="fe392-121">Type</span><span class="sxs-lookup"><span data-stu-id="fe392-121">Type</span></span>   | <span data-ttu-id="fe392-122">説明</span><span class="sxs-lookup"><span data-stu-id="fe392-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="fe392-123">period</span><span class="sxs-lookup"><span data-stu-id="fe392-123">period</span></span>    | <span data-ttu-id="fe392-124">文字列</span><span class="sxs-lookup"><span data-stu-id="fe392-124">string</span></span> | <span data-ttu-id="fe392-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="fe392-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="fe392-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="fe392-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="fe392-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="fe392-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="fe392-128">必須。</span><span class="sxs-lookup"><span data-stu-id="fe392-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="fe392-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fe392-129">Request headers</span></span>

| <span data-ttu-id="fe392-130">名前</span><span class="sxs-lookup"><span data-stu-id="fe392-130">Name</span></span>          | <span data-ttu-id="fe392-131">説明</span><span class="sxs-lookup"><span data-stu-id="fe392-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="fe392-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe392-132">Authorization</span></span> | <span data-ttu-id="fe392-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fe392-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="fe392-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="fe392-135">If-None-Match</span></span> | <span data-ttu-id="fe392-136">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="fe392-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="fe392-137">省略可能。</span><span class="sxs-lookup"><span data-stu-id="fe392-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="fe392-138">応答</span><span class="sxs-lookup"><span data-stu-id="fe392-138">Response</span></span>

<span data-ttu-id="fe392-139">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="fe392-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="fe392-140">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="fe392-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="fe392-141">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="fe392-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="fe392-142">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="fe392-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="fe392-143">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="fe392-143">Report Refresh Date</span></span>
- <span data-ttu-id="fe392-144">表示済みまたは編集済み</span><span class="sxs-lookup"><span data-stu-id="fe392-144">Viewed Or Edited</span></span>
- <span data-ttu-id="fe392-145">同期済み</span><span class="sxs-lookup"><span data-stu-id="fe392-145">Synced</span></span>
- <span data-ttu-id="fe392-146">社内で共有済み</span><span class="sxs-lookup"><span data-stu-id="fe392-146">Shared Internally</span></span>
- <span data-ttu-id="fe392-147">外部で共有済み</span><span class="sxs-lookup"><span data-stu-id="fe392-147">Shared Externally</span></span>
- <span data-ttu-id="fe392-148">レポート日付</span><span class="sxs-lookup"><span data-stu-id="fe392-148">Report Date</span></span>
- <span data-ttu-id="fe392-149">レポート期間</span><span class="sxs-lookup"><span data-stu-id="fe392-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="fe392-150">例</span><span class="sxs-lookup"><span data-stu-id="fe392-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="fe392-151">要求</span><span class="sxs-lookup"><span data-stu-id="fe392-151">Request</span></span>

<span data-ttu-id="fe392-152">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fe392-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityfilecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityFileCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="fe392-153">応答</span><span class="sxs-lookup"><span data-stu-id="fe392-153">Response</span></span>

<span data-ttu-id="fe392-154">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fe392-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="fe392-155">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="fe392-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```
