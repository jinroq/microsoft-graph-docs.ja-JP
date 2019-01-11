---
title: 'reportRoot: getOffice365ActivationCounts'
description: デスクトップとデバイスでの Office 365 のライセンス認証の数を取得します。
localization_priority: Normal
ms.openlocfilehash: a8447c0a8b98b9bf26bf7e8efd728a6ef120813d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890553"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="138b1-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="138b1-103">reportRoot: getOffice365ActivationCounts</span></span>

<span data-ttu-id="138b1-104">デスクトップとデバイスでの Office 365 のライセンス認証の数を取得します。</span><span class="sxs-lookup"><span data-stu-id="138b1-104">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="138b1-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Microsoft Office ライセンス認証](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="138b1-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="138b1-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="138b1-106">Permissions</span></span>

<span data-ttu-id="138b1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="138b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="138b1-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="138b1-109">Permission type</span></span>                        | <span data-ttu-id="138b1-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="138b1-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="138b1-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="138b1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="138b1-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="138b1-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="138b1-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="138b1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="138b1-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="138b1-114">Not supported.</span></span>                           |
| <span data-ttu-id="138b1-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="138b1-115">Application</span></span>                            | <span data-ttu-id="138b1-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="138b1-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="138b1-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="138b1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="request-headers"></a><span data-ttu-id="138b1-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="138b1-118">Request headers</span></span>

| <span data-ttu-id="138b1-119">名前</span><span class="sxs-lookup"><span data-stu-id="138b1-119">Name</span></span>          | <span data-ttu-id="138b1-120">説明</span><span class="sxs-lookup"><span data-stu-id="138b1-120">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="138b1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="138b1-121">Authorization</span></span> | <span data-ttu-id="138b1-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="138b1-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="138b1-124">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="138b1-124">If-None-Match</span></span> | <span data-ttu-id="138b1-125">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="138b1-125">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="138b1-126">省略可能。</span><span class="sxs-lookup"><span data-stu-id="138b1-126">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="138b1-127">応答</span><span class="sxs-lookup"><span data-stu-id="138b1-127">Response</span></span>

<span data-ttu-id="138b1-128">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="138b1-128">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="138b1-129">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="138b1-129">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="138b1-130">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="138b1-130">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="138b1-131">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="138b1-131">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="138b1-132">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="138b1-132">Report Refresh Date</span></span>
- <span data-ttu-id="138b1-133">製品の種類</span><span class="sxs-lookup"><span data-stu-id="138b1-133">Product Type</span></span>
- <span data-ttu-id="138b1-134">Windows</span><span class="sxs-lookup"><span data-stu-id="138b1-134">Windows</span></span>
- <span data-ttu-id="138b1-135">Mac</span><span class="sxs-lookup"><span data-stu-id="138b1-135">Mac</span></span>
- <span data-ttu-id="138b1-136">Android</span><span class="sxs-lookup"><span data-stu-id="138b1-136">Android</span></span>
- <span data-ttu-id="138b1-137">iOS</span><span class="sxs-lookup"><span data-stu-id="138b1-137">iOS</span></span>
- <span data-ttu-id="138b1-138">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="138b1-138">Windows 10 Mobile</span></span>

## <a name="example"></a><span data-ttu-id="138b1-139">例</span><span class="sxs-lookup"><span data-stu-id="138b1-139">Example</span></span>

#### <a name="request"></a><span data-ttu-id="138b1-140">要求</span><span class="sxs-lookup"><span data-stu-id="138b1-140">Request</span></span>

<span data-ttu-id="138b1-141">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="138b1-141">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationCounts
```

#### <a name="response"></a><span data-ttu-id="138b1-142">応答</span><span class="sxs-lookup"><span data-stu-id="138b1-142">Response</span></span>

<span data-ttu-id="138b1-143">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="138b1-143">The following is an example of the response.</span></span>

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

<span data-ttu-id="138b1-144">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="138b1-144">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Windows,Mac,Android,iOS,Windows 10 Mobile
```
