---
title: 'reportRoot: getOffice365ActivationCounts'
description: デスクトップとデバイスでの Office 365 のライセンス認証の数を取得します。
ms.openlocfilehash: c75b957f02eb5d5fa77f5e3dfa696f3086f9d817
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068074"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="e23db-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="e23db-103">reportRoot: getOffice365ActivationCounts</span></span>

> <span data-ttu-id="e23db-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e23db-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e23db-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e23db-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e23db-106">デスクトップとデバイスでの Office 365 のライセンス認証の数を取得します。</span><span class="sxs-lookup"><span data-stu-id="e23db-106">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="e23db-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Microsoft Office ライセンス認証](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e23db-107">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="e23db-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e23db-108">Permissions</span></span>

<span data-ttu-id="e23db-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e23db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e23db-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e23db-111">Permission type</span></span>                        | <span data-ttu-id="e23db-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e23db-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e23db-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="e23db-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="e23db-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e23db-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e23db-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e23db-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e23db-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e23db-116">Not supported.</span></span>                           |
| <span data-ttu-id="e23db-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e23db-117">Application</span></span>                            | <span data-ttu-id="e23db-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e23db-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e23db-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e23db-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="query-parameters"></a><span data-ttu-id="e23db-120">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e23db-120">Query parameters</span></span>

<span data-ttu-id="e23db-121">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="e23db-121">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e23db-122">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="e23db-122">The default output type is text/csv.</span></span> <span data-ttu-id="e23db-123">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="e23db-123">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e23db-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e23db-124">Request headers</span></span>

| <span data-ttu-id="e23db-125">名前</span><span class="sxs-lookup"><span data-stu-id="e23db-125">Name</span></span>          | <span data-ttu-id="e23db-126">説明</span><span class="sxs-lookup"><span data-stu-id="e23db-126">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e23db-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="e23db-127">Authorization</span></span> | <span data-ttu-id="e23db-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e23db-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e23db-130">応答</span><span class="sxs-lookup"><span data-stu-id="e23db-130">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e23db-131">CSV</span><span class="sxs-lookup"><span data-stu-id="e23db-131">CSV</span></span>

<span data-ttu-id="e23db-132">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="e23db-132">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e23db-133">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="e23db-133">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e23db-134">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="e23db-134">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e23db-135">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="e23db-135">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e23db-136">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="e23db-136">Report Refresh Date</span></span>
- <span data-ttu-id="e23db-137">製品の種類</span><span class="sxs-lookup"><span data-stu-id="e23db-137">Product Type</span></span>
- <span data-ttu-id="e23db-138">Windows</span><span class="sxs-lookup"><span data-stu-id="e23db-138">Windows</span></span>
- <span data-ttu-id="e23db-139">Mac</span><span class="sxs-lookup"><span data-stu-id="e23db-139">Mac</span></span>
- <span data-ttu-id="e23db-140">Android</span><span class="sxs-lookup"><span data-stu-id="e23db-140">Android</span></span>
- <span data-ttu-id="e23db-141">iOS</span><span class="sxs-lookup"><span data-stu-id="e23db-141">iOS</span></span>
- <span data-ttu-id="e23db-142">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="e23db-142">Windows 10 Mobile</span></span>

### <a name="json"></a><span data-ttu-id="e23db-143">JSON</span><span class="sxs-lookup"><span data-stu-id="e23db-143">JSON</span></span>

<span data-ttu-id="e23db-144">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の**[office365ActivationCounts](../resources/office365activationcounts.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="e23db-144">If successful, this method returns a `200 OK` response code and an **[office365ActivationCounts](../resources/office365activationcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e23db-145">使用例</span><span class="sxs-lookup"><span data-stu-id="e23db-145">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e23db-146">CSV</span><span class="sxs-lookup"><span data-stu-id="e23db-146">CSV</span></span>

<span data-ttu-id="e23db-147">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="e23db-147">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e23db-148">要求</span><span class="sxs-lookup"><span data-stu-id="e23db-148">Request</span></span>

<span data-ttu-id="e23db-149">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e23db-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="e23db-150">応答</span><span class="sxs-lookup"><span data-stu-id="e23db-150">Response</span></span>

<span data-ttu-id="e23db-151">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e23db-151">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="e23db-152">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="e23db-152">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Windows,Mac,Android,iOS,Windows 10 Mobile
```

### <a name="json"></a><span data-ttu-id="e23db-153">JSON</span><span class="sxs-lookup"><span data-stu-id="e23db-153">JSON</span></span>

<span data-ttu-id="e23db-154">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="e23db-154">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e23db-155">要求</span><span class="sxs-lookup"><span data-stu-id="e23db-155">Request</span></span>

<span data-ttu-id="e23db-156">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="e23db-156">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="e23db-157">応答</span><span class="sxs-lookup"><span data-stu-id="e23db-157">Response</span></span>

<span data-ttu-id="e23db-158">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="e23db-158">The following example shows the response.</span></span>

> <span data-ttu-id="e23db-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e23db-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActivationCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 268

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActivationCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "productType": "Office 365 ProPlus", 
      "windows": 9157, 
      "mac": 576, 
      "android": 358, 
      "ios": 1452, 
      "windows10Mobile": 2309
    }
  ]
}
```