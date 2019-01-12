---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Office 365 がアクティブ化されているユーザーに関する詳細情報を取得します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 02e06e36a2329a3a302c042d71ff259b3e6c57b4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978061"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="6ead4-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="6ead4-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

<span data-ttu-id="6ead4-104">Office 365 がアクティブ化されているユーザーに関する詳細情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="6ead4-104">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="6ead4-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Microsoft Office ライセンス認証](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6ead4-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="6ead4-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6ead4-106">Permissions</span></span>

<span data-ttu-id="6ead4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6ead4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6ead4-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6ead4-109">Permission type</span></span>                        | <span data-ttu-id="6ead4-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6ead4-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6ead4-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="6ead4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6ead4-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ead4-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6ead4-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6ead4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ead4-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ead4-114">Not supported.</span></span>                           |
| <span data-ttu-id="6ead4-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6ead4-115">Application</span></span>                            | <span data-ttu-id="6ead4-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ead4-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6ead4-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6ead4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="request-headers"></a><span data-ttu-id="6ead4-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6ead4-118">Request headers</span></span>

| <span data-ttu-id="6ead4-119">名前</span><span class="sxs-lookup"><span data-stu-id="6ead4-119">Name</span></span>          | <span data-ttu-id="6ead4-120">説明</span><span class="sxs-lookup"><span data-stu-id="6ead4-120">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="6ead4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ead4-121">Authorization</span></span> | <span data-ttu-id="6ead4-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6ead4-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="6ead4-124">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="6ead4-124">If-None-Match</span></span> | <span data-ttu-id="6ead4-125">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="6ead4-125">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="6ead4-126">省略可能。</span><span class="sxs-lookup"><span data-stu-id="6ead4-126">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="6ead4-127">応答</span><span class="sxs-lookup"><span data-stu-id="6ead4-127">Response</span></span>

<span data-ttu-id="6ead4-128">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="6ead4-128">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6ead4-129">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="6ead4-129">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6ead4-130">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="6ead4-130">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6ead4-131">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="6ead4-131">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6ead4-132">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="6ead4-132">Report Refresh Date</span></span>
- <span data-ttu-id="6ead4-133">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="6ead4-133">User Principal Name</span></span>
- <span data-ttu-id="6ead4-134">表示名</span><span class="sxs-lookup"><span data-stu-id="6ead4-134">Display Name</span></span>
- <span data-ttu-id="6ead4-135">製品の種類</span><span class="sxs-lookup"><span data-stu-id="6ead4-135">Product Type</span></span>
- <span data-ttu-id="6ead4-136">最後のライセンス認証日</span><span class="sxs-lookup"><span data-stu-id="6ead4-136">Last Activated Date</span></span>
- <span data-ttu-id="6ead4-137">Windows</span><span class="sxs-lookup"><span data-stu-id="6ead4-137">Windows</span></span>
- <span data-ttu-id="6ead4-138">Mac</span><span class="sxs-lookup"><span data-stu-id="6ead4-138">Mac</span></span>
- <span data-ttu-id="6ead4-139">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="6ead4-139">Windows 10 Mobile</span></span>
- <span data-ttu-id="6ead4-140">iOS</span><span class="sxs-lookup"><span data-stu-id="6ead4-140">iOS</span></span>
- <span data-ttu-id="6ead4-141">Android</span><span class="sxs-lookup"><span data-stu-id="6ead4-141">Android</span></span>
- <span data-ttu-id="6ead4-142">共有コンピューター上でアクティブ化</span><span class="sxs-lookup"><span data-stu-id="6ead4-142">Activated On Shared Computer</span></span>

## <a name="example"></a><span data-ttu-id="6ead4-143">例</span><span class="sxs-lookup"><span data-stu-id="6ead4-143">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6ead4-144">要求</span><span class="sxs-lookup"><span data-stu-id="6ead4-144">Request</span></span>

<span data-ttu-id="6ead4-145">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6ead4-145">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserDetail
```

#### <a name="response"></a><span data-ttu-id="6ead4-146">応答</span><span class="sxs-lookup"><span data-stu-id="6ead4-146">Response</span></span>

<span data-ttu-id="6ead4-147">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6ead4-147">The following is an example of the response.</span></span>

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

<span data-ttu-id="6ead4-148">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="6ead4-148">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Product Type,Last Activated Date,Windows,Mac,Windows 10 Mobile,iOS,Android,Activated On Shared Computer
```
