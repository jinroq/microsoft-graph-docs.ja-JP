---
title: 'reportRoot: getOffice365ActivationsUserCounts'
description: 有効になっているユーザーの数と、デスクトップまたはデバイスまたは共有コンピューターで Office サブスクリプションをアクティブ化したユーザーの数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 6dea39dc2c3d2eddffae03dcd5df3070ea213979
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447041"
---
# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="66fbc-103">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="66fbc-103">reportRoot: getOffice365ActivationsUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66fbc-104">有効になっているユーザーの数と、デスクトップまたはデバイスまたは共有コンピューターで Office サブスクリプションをアクティブ化したユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="66fbc-104">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices or shared computers.</span></span>

> <span data-ttu-id="66fbc-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Microsoft Office ライセンス認証](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="66fbc-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="66fbc-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="66fbc-106">Permissions</span></span>

<span data-ttu-id="66fbc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="66fbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="66fbc-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="66fbc-109">Permission type</span></span>                        | <span data-ttu-id="66fbc-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="66fbc-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="66fbc-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="66fbc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="66fbc-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="66fbc-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="66fbc-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="66fbc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66fbc-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66fbc-114">Not supported.</span></span>                           |
| <span data-ttu-id="66fbc-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="66fbc-115">Application</span></span>                            | <span data-ttu-id="66fbc-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="66fbc-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="66fbc-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="66fbc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="query-parameters"></a><span data-ttu-id="66fbc-118">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="66fbc-118">Query parameters</span></span>

<span data-ttu-id="66fbc-119">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="66fbc-119">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="66fbc-120">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="66fbc-120">The default output type is text/csv.</span></span> <span data-ttu-id="66fbc-121">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="66fbc-121">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="66fbc-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="66fbc-122">Request headers</span></span>

| <span data-ttu-id="66fbc-123">名前</span><span class="sxs-lookup"><span data-stu-id="66fbc-123">Name</span></span>          | <span data-ttu-id="66fbc-124">説明</span><span class="sxs-lookup"><span data-stu-id="66fbc-124">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="66fbc-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="66fbc-125">Authorization</span></span> | <span data-ttu-id="66fbc-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="66fbc-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="66fbc-128">応答</span><span class="sxs-lookup"><span data-stu-id="66fbc-128">Response</span></span>

### <a name="csv"></a><span data-ttu-id="66fbc-129">CSV</span><span class="sxs-lookup"><span data-stu-id="66fbc-129">CSV</span></span>

<span data-ttu-id="66fbc-130">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="66fbc-130">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="66fbc-131">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="66fbc-131">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="66fbc-132">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="66fbc-132">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="66fbc-133">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="66fbc-133">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="66fbc-134">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="66fbc-134">Report Refresh Date</span></span>
- <span data-ttu-id="66fbc-135">製品の種類</span><span class="sxs-lookup"><span data-stu-id="66fbc-135">Product Type</span></span>
- <span data-ttu-id="66fbc-136">割り当て済み</span><span class="sxs-lookup"><span data-stu-id="66fbc-136">Assigned</span></span>
- <span data-ttu-id="66fbc-137">アクティブ</span><span class="sxs-lookup"><span data-stu-id="66fbc-137">Activated</span></span>
- <span data-ttu-id="66fbc-138">共有コンピューターのライセンス認証</span><span class="sxs-lookup"><span data-stu-id="66fbc-138">Shared Computer Activation</span></span>

### <a name="json"></a><span data-ttu-id="66fbc-139">JSON</span><span class="sxs-lookup"><span data-stu-id="66fbc-139">JSON</span></span>

<span data-ttu-id="66fbc-140">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[office365ActivationsUserCounts](../resources/office365activationsusercounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="66fbc-140">If successful, this method returns a `200 OK` response code and an **[office365ActivationsUserCounts](../resources/office365activationsusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66fbc-141">例</span><span class="sxs-lookup"><span data-stu-id="66fbc-141">Example</span></span>

### <a name="csv"></a><span data-ttu-id="66fbc-142">CSV</span><span class="sxs-lookup"><span data-stu-id="66fbc-142">CSV</span></span>

<span data-ttu-id="66fbc-143">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="66fbc-143">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="66fbc-144">要求</span><span class="sxs-lookup"><span data-stu-id="66fbc-144">Request</span></span>

<span data-ttu-id="66fbc-145">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="66fbc-145">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="66fbc-146">プロトコル</span><span class="sxs-lookup"><span data-stu-id="66fbc-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserCounts?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="66fbc-147">C#</span><span class="sxs-lookup"><span data-stu-id="66fbc-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationsusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="66fbc-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="66fbc-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationsusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="66fbc-149">目的-C</span><span class="sxs-lookup"><span data-stu-id="66fbc-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationsusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="66fbc-150">応答</span><span class="sxs-lookup"><span data-stu-id="66fbc-150">Response</span></span>

<span data-ttu-id="66fbc-151">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="66fbc-151">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="66fbc-152">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="66fbc-152">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Assigned,Activated,Shared Computer Activation
```

### <a name="json"></a><span data-ttu-id="66fbc-153">JSON</span><span class="sxs-lookup"><span data-stu-id="66fbc-153">JSON</span></span>

<span data-ttu-id="66fbc-154">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="66fbc-154">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="66fbc-155">要求</span><span class="sxs-lookup"><span data-stu-id="66fbc-155">Request</span></span>

<span data-ttu-id="66fbc-156">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="66fbc-156">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="66fbc-157">プロトコル</span><span class="sxs-lookup"><span data-stu-id="66fbc-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserCounts?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="66fbc-158">C#</span><span class="sxs-lookup"><span data-stu-id="66fbc-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationsusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="66fbc-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="66fbc-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationsusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="66fbc-160">目的-C</span><span class="sxs-lookup"><span data-stu-id="66fbc-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationsusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="66fbc-161">応答</span><span class="sxs-lookup"><span data-stu-id="66fbc-161">Response</span></span>

<span data-ttu-id="66fbc-162">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="66fbc-162">The following example shows the response.</span></span>

> <span data-ttu-id="66fbc-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="66fbc-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActivationsUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActivationsUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "productType": "Office 365 ProPlus", 
      "assigned": 2679, 
      "activated": 1710,
      "sharedComputerActivation": 1024
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
