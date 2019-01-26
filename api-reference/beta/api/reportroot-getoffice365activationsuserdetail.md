---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Office 365 がアクティブ化されているユーザーに関する詳細情報を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 1603ce547723ffe7271a76986f51241466c306f3
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571367"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="7f1b5-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="7f1b5-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f1b5-104">Office 365 がアクティブ化されているユーザーに関する詳細情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="7f1b5-104">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="7f1b5-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Microsoft Office ライセンス認証](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f1b5-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="7f1b5-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7f1b5-106">Permissions</span></span>

<span data-ttu-id="7f1b5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f1b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7f1b5-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7f1b5-109">Permission type</span></span>                        | <span data-ttu-id="7f1b5-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7f1b5-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7f1b5-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="7f1b5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7f1b5-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f1b5-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7f1b5-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7f1b5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f1b5-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f1b5-114">Not supported.</span></span>                           |
| <span data-ttu-id="7f1b5-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7f1b5-115">Application</span></span>                            | <span data-ttu-id="7f1b5-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f1b5-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7f1b5-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7f1b5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="query-parameters"></a><span data-ttu-id="7f1b5-118">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7f1b5-118">Query parameters</span></span>

<span data-ttu-id="7f1b5-119">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7f1b5-119">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="7f1b5-120">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="7f1b5-120">The default output type is text/csv.</span></span> <span data-ttu-id="7f1b5-121">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="7f1b5-121">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7f1b5-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f1b5-122">Request headers</span></span>

| <span data-ttu-id="7f1b5-123">名前</span><span class="sxs-lookup"><span data-stu-id="7f1b5-123">Name</span></span>          | <span data-ttu-id="7f1b5-124">説明</span><span class="sxs-lookup"><span data-stu-id="7f1b5-124">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7f1b5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f1b5-125">Authorization</span></span> | <span data-ttu-id="7f1b5-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7f1b5-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7f1b5-128">応答</span><span class="sxs-lookup"><span data-stu-id="7f1b5-128">Response</span></span>

### <a name="csv"></a><span data-ttu-id="7f1b5-129">CSV</span><span class="sxs-lookup"><span data-stu-id="7f1b5-129">CSV</span></span>

<span data-ttu-id="7f1b5-130">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="7f1b5-130">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7f1b5-131">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="7f1b5-131">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7f1b5-132">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="7f1b5-132">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7f1b5-133">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="7f1b5-133">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7f1b5-134">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="7f1b5-134">Report Refresh Date</span></span>
- <span data-ttu-id="7f1b5-135">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="7f1b5-135">User Principal Name</span></span>
- <span data-ttu-id="7f1b5-136">表示名</span><span class="sxs-lookup"><span data-stu-id="7f1b5-136">Display Name</span></span>
- <span data-ttu-id="7f1b5-137">製品の種類</span><span class="sxs-lookup"><span data-stu-id="7f1b5-137">Product Type</span></span>
- <span data-ttu-id="7f1b5-138">最後のライセンス認証日</span><span class="sxs-lookup"><span data-stu-id="7f1b5-138">Last Activated Date</span></span>
- <span data-ttu-id="7f1b5-139">Windows</span><span class="sxs-lookup"><span data-stu-id="7f1b5-139">Windows</span></span>
- <span data-ttu-id="7f1b5-140">Mac</span><span class="sxs-lookup"><span data-stu-id="7f1b5-140">Mac</span></span>
- <span data-ttu-id="7f1b5-141">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="7f1b5-141">Windows 10 Mobile</span></span>
- <span data-ttu-id="7f1b5-142">iOS</span><span class="sxs-lookup"><span data-stu-id="7f1b5-142">iOS</span></span>
- <span data-ttu-id="7f1b5-143">Android</span><span class="sxs-lookup"><span data-stu-id="7f1b5-143">Android</span></span>
- <span data-ttu-id="7f1b5-144">共有コンピューター上でアクティブ化</span><span class="sxs-lookup"><span data-stu-id="7f1b5-144">Activated On Shared Computer</span></span>

### <a name="json"></a><span data-ttu-id="7f1b5-145">JSON</span><span class="sxs-lookup"><span data-stu-id="7f1b5-145">JSON</span></span>

<span data-ttu-id="7f1b5-146">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の**[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="7f1b5-146">If successful, this method returns a `200 OK` response code and an **[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="7f1b5-147">この要求の既定のページ サイズは、アイテムは 200 個です。</span><span class="sxs-lookup"><span data-stu-id="7f1b5-147">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="7f1b5-148">例</span><span class="sxs-lookup"><span data-stu-id="7f1b5-148">Example</span></span>

### <a name="csv"></a><span data-ttu-id="7f1b5-149">CSV</span><span class="sxs-lookup"><span data-stu-id="7f1b5-149">CSV</span></span>

<span data-ttu-id="7f1b5-150">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="7f1b5-150">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="7f1b5-151">要求</span><span class="sxs-lookup"><span data-stu-id="7f1b5-151">Request</span></span>

<span data-ttu-id="7f1b5-152">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7f1b5-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="7f1b5-153">応答</span><span class="sxs-lookup"><span data-stu-id="7f1b5-153">Response</span></span>

<span data-ttu-id="7f1b5-154">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7f1b5-154">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7f1b5-155">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="7f1b5-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Product Type,Last Activated Date,Windows,Mac,Windows 10 Mobile,iOS,Android,Activated On Shared Computer
```

### <a name="json"></a><span data-ttu-id="7f1b5-156">JSON</span><span class="sxs-lookup"><span data-stu-id="7f1b5-156">JSON</span></span>

<span data-ttu-id="7f1b5-157">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="7f1b5-157">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="7f1b5-158">要求</span><span class="sxs-lookup"><span data-stu-id="7f1b5-158">Request</span></span>

<span data-ttu-id="7f1b5-159">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7f1b5-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="7f1b5-160">応答</span><span class="sxs-lookup"><span data-stu-id="7f1b5-160">Response</span></span>

<span data-ttu-id="7f1b5-161">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7f1b5-161">The following is an example of the response.</span></span>

> <span data-ttu-id="7f1b5-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7f1b5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActivationsUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActivationsUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userprincipalname-value", 
      "displayName": "displayname-value", 
      "userActivationCounts": [
        {
          "productType": "Project Client", 
          "lastActivatedDate": "2017-08-20", 
          "windows": 5, 
          "mac": 0, 
          "windows10Mobile": 0, 
          "ios": 0, 
          "android": 2,
          "activatedOnSharedComputer": true
        }
      ]
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365activationsuserdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
