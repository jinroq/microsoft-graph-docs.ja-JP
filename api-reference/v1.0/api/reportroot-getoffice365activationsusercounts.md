---
title: 'reportRoot: getOffice365ActivationsUserCounts'
description: 有効になっているユーザーの数と、デスクトップまたはデバイスまたは共有コンピューターで Office サブスクリプションをアクティブ化したユーザーの数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 9a150911e9234cde7258acbeed7f825fb9db4c66
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582158"
---
# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="2e5db-103">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="2e5db-103">reportRoot: getOffice365ActivationsUserCounts</span></span>

<span data-ttu-id="2e5db-104">有効になっているユーザーの数と、デスクトップまたはデバイスまたは共有コンピューターで Office サブスクリプションをアクティブ化したユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="2e5db-104">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices or shared computers.</span></span>

> <span data-ttu-id="2e5db-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Microsoft Office ライセンス認証](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2e5db-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="2e5db-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2e5db-106">Permissions</span></span>

<span data-ttu-id="2e5db-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2e5db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2e5db-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2e5db-109">Permission type</span></span>                        | <span data-ttu-id="2e5db-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2e5db-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2e5db-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2e5db-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2e5db-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e5db-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2e5db-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2e5db-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e5db-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2e5db-114">Not supported.</span></span>                           |
| <span data-ttu-id="2e5db-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2e5db-115">Application</span></span>                            | <span data-ttu-id="2e5db-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e5db-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2e5db-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2e5db-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="request-headers"></a><span data-ttu-id="2e5db-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2e5db-118">Request headers</span></span>

| <span data-ttu-id="2e5db-119">名前</span><span class="sxs-lookup"><span data-stu-id="2e5db-119">Name</span></span>          | <span data-ttu-id="2e5db-120">説明</span><span class="sxs-lookup"><span data-stu-id="2e5db-120">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="2e5db-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e5db-121">Authorization</span></span> | <span data-ttu-id="2e5db-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2e5db-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="2e5db-124">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="2e5db-124">If-None-Match</span></span> | <span data-ttu-id="2e5db-125">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="2e5db-125">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="2e5db-126">省略可能。</span><span class="sxs-lookup"><span data-stu-id="2e5db-126">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="2e5db-127">応答</span><span class="sxs-lookup"><span data-stu-id="2e5db-127">Response</span></span>

<span data-ttu-id="2e5db-128">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="2e5db-128">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2e5db-129">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="2e5db-129">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2e5db-130">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="2e5db-130">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2e5db-131">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="2e5db-131">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2e5db-132">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="2e5db-132">Report Refresh Date</span></span>
- <span data-ttu-id="2e5db-133">製品の種類</span><span class="sxs-lookup"><span data-stu-id="2e5db-133">Product Type</span></span>
- <span data-ttu-id="2e5db-134">割り当て済み</span><span class="sxs-lookup"><span data-stu-id="2e5db-134">Assigned</span></span>
- <span data-ttu-id="2e5db-135">アクティブ</span><span class="sxs-lookup"><span data-stu-id="2e5db-135">Activated</span></span>
- <span data-ttu-id="2e5db-136">共有コンピューターのライセンス認証</span><span class="sxs-lookup"><span data-stu-id="2e5db-136">Shared Computer Activation</span></span>

## <a name="example"></a><span data-ttu-id="2e5db-137">例</span><span class="sxs-lookup"><span data-stu-id="2e5db-137">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2e5db-138">要求</span><span class="sxs-lookup"><span data-stu-id="2e5db-138">Request</span></span>

<span data-ttu-id="2e5db-139">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2e5db-139">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserCounts
```

#### <a name="response"></a><span data-ttu-id="2e5db-140">応答</span><span class="sxs-lookup"><span data-stu-id="2e5db-140">Response</span></span>

<span data-ttu-id="2e5db-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2e5db-141">The following is an example of the response.</span></span>

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

<span data-ttu-id="2e5db-142">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="2e5db-142">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Assigned,Activated,Shared Computer Activation
```
