---
title: 'reportRoot: getOffice365ActivationCounts'
description: デスクトップとデバイスでの Office 365 のライセンス認証の数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 8d9bf5576cf459d21a2338dce2df702727836008
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447027"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="7e0d3-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="7e0d3-103">reportRoot: getOffice365ActivationCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e0d3-104">デスクトップとデバイスでの Office 365 のライセンス認証の数を取得します。</span><span class="sxs-lookup"><span data-stu-id="7e0d3-104">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="7e0d3-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Microsoft Office ライセンス認証](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7e0d3-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="7e0d3-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7e0d3-106">Permissions</span></span>

<span data-ttu-id="7e0d3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7e0d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7e0d3-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7e0d3-109">Permission type</span></span>                        | <span data-ttu-id="7e0d3-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7e0d3-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7e0d3-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="7e0d3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7e0d3-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e0d3-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7e0d3-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7e0d3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e0d3-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e0d3-114">Not supported.</span></span>                           |
| <span data-ttu-id="7e0d3-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7e0d3-115">Application</span></span>                            | <span data-ttu-id="7e0d3-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e0d3-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7e0d3-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7e0d3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="query-parameters"></a><span data-ttu-id="7e0d3-118">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7e0d3-118">Query parameters</span></span>

<span data-ttu-id="7e0d3-119">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7e0d3-119">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="7e0d3-120">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="7e0d3-120">The default output type is text/csv.</span></span> <span data-ttu-id="7e0d3-121">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="7e0d3-121">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7e0d3-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7e0d3-122">Request headers</span></span>

| <span data-ttu-id="7e0d3-123">名前</span><span class="sxs-lookup"><span data-stu-id="7e0d3-123">Name</span></span>          | <span data-ttu-id="7e0d3-124">説明</span><span class="sxs-lookup"><span data-stu-id="7e0d3-124">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7e0d3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e0d3-125">Authorization</span></span> | <span data-ttu-id="7e0d3-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7e0d3-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7e0d3-128">応答</span><span class="sxs-lookup"><span data-stu-id="7e0d3-128">Response</span></span>

### <a name="csv"></a><span data-ttu-id="7e0d3-129">CSV</span><span class="sxs-lookup"><span data-stu-id="7e0d3-129">CSV</span></span>

<span data-ttu-id="7e0d3-130">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="7e0d3-130">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7e0d3-131">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="7e0d3-131">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7e0d3-132">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="7e0d3-132">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7e0d3-133">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="7e0d3-133">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7e0d3-134">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="7e0d3-134">Report Refresh Date</span></span>
- <span data-ttu-id="7e0d3-135">製品の種類</span><span class="sxs-lookup"><span data-stu-id="7e0d3-135">Product Type</span></span>
- <span data-ttu-id="7e0d3-136">Windows</span><span class="sxs-lookup"><span data-stu-id="7e0d3-136">Windows</span></span>
- <span data-ttu-id="7e0d3-137">Mac</span><span class="sxs-lookup"><span data-stu-id="7e0d3-137">Mac</span></span>
- <span data-ttu-id="7e0d3-138">Android</span><span class="sxs-lookup"><span data-stu-id="7e0d3-138">Android</span></span>
- <span data-ttu-id="7e0d3-139">iOS</span><span class="sxs-lookup"><span data-stu-id="7e0d3-139">iOS</span></span>
- <span data-ttu-id="7e0d3-140">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="7e0d3-140">Windows 10 Mobile</span></span>

### <a name="json"></a><span data-ttu-id="7e0d3-141">JSON</span><span class="sxs-lookup"><span data-stu-id="7e0d3-141">JSON</span></span>

<span data-ttu-id="7e0d3-142">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[office365ActivationCounts](../resources/office365activationcounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7e0d3-142">If successful, this method returns a `200 OK` response code and an **[office365ActivationCounts](../resources/office365activationcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e0d3-143">例</span><span class="sxs-lookup"><span data-stu-id="7e0d3-143">Example</span></span>

### <a name="csv"></a><span data-ttu-id="7e0d3-144">CSV</span><span class="sxs-lookup"><span data-stu-id="7e0d3-144">CSV</span></span>

<span data-ttu-id="7e0d3-145">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7e0d3-145">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="7e0d3-146">要求</span><span class="sxs-lookup"><span data-stu-id="7e0d3-146">Request</span></span>

<span data-ttu-id="7e0d3-147">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7e0d3-147">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7e0d3-148">プロトコル</span><span class="sxs-lookup"><span data-stu-id="7e0d3-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7e0d3-149">C#</span><span class="sxs-lookup"><span data-stu-id="7e0d3-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationcounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7e0d3-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="7e0d3-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationcounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7e0d3-151">目的-C</span><span class="sxs-lookup"><span data-stu-id="7e0d3-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationcounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7e0d3-152">応答</span><span class="sxs-lookup"><span data-stu-id="7e0d3-152">Response</span></span>

<span data-ttu-id="7e0d3-153">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7e0d3-153">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7e0d3-154">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="7e0d3-154">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="7e0d3-155">JSON</span><span class="sxs-lookup"><span data-stu-id="7e0d3-155">JSON</span></span>

<span data-ttu-id="7e0d3-156">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="7e0d3-156">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="7e0d3-157">要求</span><span class="sxs-lookup"><span data-stu-id="7e0d3-157">Request</span></span>

<span data-ttu-id="7e0d3-158">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="7e0d3-158">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7e0d3-159">プロトコル</span><span class="sxs-lookup"><span data-stu-id="7e0d3-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7e0d3-160">C#</span><span class="sxs-lookup"><span data-stu-id="7e0d3-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationcounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7e0d3-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="7e0d3-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationcounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7e0d3-162">目的-C</span><span class="sxs-lookup"><span data-stu-id="7e0d3-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationcounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7e0d3-163">応答</span><span class="sxs-lookup"><span data-stu-id="7e0d3-163">Response</span></span>

<span data-ttu-id="7e0d3-164">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="7e0d3-164">The following example shows the response.</span></span>

> <span data-ttu-id="7e0d3-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7e0d3-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
