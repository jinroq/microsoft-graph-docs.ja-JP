---
title: 'reportRoot: getOffice365ActivationsUserCounts'
description: 有効になっているユーザーとデスクトップやデバイスに Office のサブスクリプションをアクティブ化または共有のコンピューターの数を取得します。
ms.openlocfilehash: f46d3e01e7eeb212ea50675bbcf7371e4af2ec40
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021498"
---
# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="d04e5-103">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="d04e5-103">reportRoot: getOffice365ActivationsUserCounts</span></span>

<span data-ttu-id="d04e5-104">有効になっているユーザーとデスクトップやデバイスに Office のサブスクリプションをアクティブ化または共有のコンピューターの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="d04e5-104">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices or shared computers.</span></span>

> <span data-ttu-id="d04e5-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Microsoft Office ライセンス認証](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d04e5-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="d04e5-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d04e5-106">Permissions</span></span>

<span data-ttu-id="d04e5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d04e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d04e5-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d04e5-109">Permission type</span></span>                        | <span data-ttu-id="d04e5-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d04e5-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d04e5-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="d04e5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d04e5-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d04e5-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d04e5-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d04e5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d04e5-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d04e5-114">Not supported.</span></span>                           |
| <span data-ttu-id="d04e5-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d04e5-115">Application</span></span>                            | <span data-ttu-id="d04e5-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d04e5-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d04e5-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d04e5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="request-headers"></a><span data-ttu-id="d04e5-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d04e5-118">Request headers</span></span>

| <span data-ttu-id="d04e5-119">名前</span><span class="sxs-lookup"><span data-stu-id="d04e5-119">Name</span></span>          | <span data-ttu-id="d04e5-120">説明</span><span class="sxs-lookup"><span data-stu-id="d04e5-120">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="d04e5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d04e5-121">Authorization</span></span> | <span data-ttu-id="d04e5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d04e5-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="d04e5-124">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="d04e5-124">If-None-Match</span></span> | <span data-ttu-id="d04e5-125">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="d04e5-125">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="d04e5-126">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d04e5-126">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="d04e5-127">応答</span><span class="sxs-lookup"><span data-stu-id="d04e5-127">Response</span></span>

<span data-ttu-id="d04e5-128">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="d04e5-128">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d04e5-129">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="d04e5-129">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d04e5-130">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="d04e5-130">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d04e5-131">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="d04e5-131">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d04e5-132">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="d04e5-132">Report Refresh Date</span></span>
- <span data-ttu-id="d04e5-133">製品の種類</span><span class="sxs-lookup"><span data-stu-id="d04e5-133">Product Type</span></span>
- <span data-ttu-id="d04e5-134">割り当て済み</span><span class="sxs-lookup"><span data-stu-id="d04e5-134">Assigned</span></span>
- <span data-ttu-id="d04e5-135">アクティブ</span><span class="sxs-lookup"><span data-stu-id="d04e5-135">Activated</span></span>
- <span data-ttu-id="d04e5-136">共有のコンピューターのライセンス認証</span><span class="sxs-lookup"><span data-stu-id="d04e5-136">Shared Computer Activation</span></span>

## <a name="example"></a><span data-ttu-id="d04e5-137">例</span><span class="sxs-lookup"><span data-stu-id="d04e5-137">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d04e5-138">要求</span><span class="sxs-lookup"><span data-stu-id="d04e5-138">Request</span></span>

<span data-ttu-id="d04e5-139">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d04e5-139">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserCounts
```

#### <a name="response"></a><span data-ttu-id="d04e5-140">応答</span><span class="sxs-lookup"><span data-stu-id="d04e5-140">Response</span></span>

<span data-ttu-id="d04e5-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d04e5-141">The following is an example of the response.</span></span>

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

<span data-ttu-id="d04e5-142">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="d04e5-142">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Assigned,Activated,Shared Computer Activation
```
