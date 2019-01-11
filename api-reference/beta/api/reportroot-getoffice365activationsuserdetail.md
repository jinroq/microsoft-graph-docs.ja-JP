---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Office 365 がアクティブ化されているユーザーに関する詳細情報を取得します。
localization_priority: Normal
ms.openlocfilehash: 686a27f0942f89a9d173544d565c2562622c6e05
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835281"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="9b6c2-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="9b6c2-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

> <span data-ttu-id="9b6c2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9b6c2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b6c2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b6c2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9b6c2-106">Office 365 がアクティブ化されているユーザーに関する詳細情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="9b6c2-106">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="9b6c2-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Microsoft Office ライセンス認証](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9b6c2-107">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="9b6c2-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9b6c2-108">Permissions</span></span>

<span data-ttu-id="9b6c2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9b6c2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9b6c2-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9b6c2-111">Permission type</span></span>                        | <span data-ttu-id="9b6c2-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9b6c2-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9b6c2-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="9b6c2-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="9b6c2-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b6c2-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9b6c2-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9b6c2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b6c2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b6c2-116">Not supported.</span></span>                           |
| <span data-ttu-id="9b6c2-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9b6c2-117">Application</span></span>                            | <span data-ttu-id="9b6c2-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b6c2-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="9b6c2-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9b6c2-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="query-parameters"></a><span data-ttu-id="9b6c2-120">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9b6c2-120">Query parameters</span></span>

<span data-ttu-id="9b6c2-121">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="9b6c2-121">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="9b6c2-122">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="9b6c2-122">The default output type is text/csv.</span></span> <span data-ttu-id="9b6c2-123">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="9b6c2-123">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9b6c2-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9b6c2-124">Request headers</span></span>

| <span data-ttu-id="9b6c2-125">名前</span><span class="sxs-lookup"><span data-stu-id="9b6c2-125">Name</span></span>          | <span data-ttu-id="9b6c2-126">説明</span><span class="sxs-lookup"><span data-stu-id="9b6c2-126">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="9b6c2-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b6c2-127">Authorization</span></span> | <span data-ttu-id="9b6c2-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9b6c2-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="9b6c2-130">応答</span><span class="sxs-lookup"><span data-stu-id="9b6c2-130">Response</span></span>

### <a name="csv"></a><span data-ttu-id="9b6c2-131">CSV</span><span class="sxs-lookup"><span data-stu-id="9b6c2-131">CSV</span></span>

<span data-ttu-id="9b6c2-132">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="9b6c2-132">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9b6c2-133">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="9b6c2-133">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9b6c2-134">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="9b6c2-134">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9b6c2-135">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="9b6c2-135">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9b6c2-136">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="9b6c2-136">Report Refresh Date</span></span>
- <span data-ttu-id="9b6c2-137">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="9b6c2-137">User Principal Name</span></span>
- <span data-ttu-id="9b6c2-138">表示名</span><span class="sxs-lookup"><span data-stu-id="9b6c2-138">Display Name</span></span>
- <span data-ttu-id="9b6c2-139">製品の種類</span><span class="sxs-lookup"><span data-stu-id="9b6c2-139">Product Type</span></span>
- <span data-ttu-id="9b6c2-140">最後のライセンス認証日</span><span class="sxs-lookup"><span data-stu-id="9b6c2-140">Last Activated Date</span></span>
- <span data-ttu-id="9b6c2-141">Windows</span><span class="sxs-lookup"><span data-stu-id="9b6c2-141">Windows</span></span>
- <span data-ttu-id="9b6c2-142">Mac</span><span class="sxs-lookup"><span data-stu-id="9b6c2-142">Mac</span></span>
- <span data-ttu-id="9b6c2-143">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="9b6c2-143">Windows 10 Mobile</span></span>
- <span data-ttu-id="9b6c2-144">iOS</span><span class="sxs-lookup"><span data-stu-id="9b6c2-144">iOS</span></span>
- <span data-ttu-id="9b6c2-145">Android</span><span class="sxs-lookup"><span data-stu-id="9b6c2-145">Android</span></span>
- <span data-ttu-id="9b6c2-146">共有コンピューター上でアクティブ化</span><span class="sxs-lookup"><span data-stu-id="9b6c2-146">Activated On Shared Computer</span></span>

### <a name="json"></a><span data-ttu-id="9b6c2-147">JSON</span><span class="sxs-lookup"><span data-stu-id="9b6c2-147">JSON</span></span>

<span data-ttu-id="9b6c2-148">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の**[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="9b6c2-148">If successful, this method returns a `200 OK` response code and an **[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="9b6c2-149">この要求の既定のページ サイズは、アイテムは 200 個です。</span><span class="sxs-lookup"><span data-stu-id="9b6c2-149">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="9b6c2-150">例</span><span class="sxs-lookup"><span data-stu-id="9b6c2-150">Example</span></span>

### <a name="csv"></a><span data-ttu-id="9b6c2-151">CSV</span><span class="sxs-lookup"><span data-stu-id="9b6c2-151">CSV</span></span>

<span data-ttu-id="9b6c2-152">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="9b6c2-152">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="9b6c2-153">要求</span><span class="sxs-lookup"><span data-stu-id="9b6c2-153">Request</span></span>

<span data-ttu-id="9b6c2-154">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9b6c2-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="9b6c2-155">応答</span><span class="sxs-lookup"><span data-stu-id="9b6c2-155">Response</span></span>

<span data-ttu-id="9b6c2-156">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9b6c2-156">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="9b6c2-157">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="9b6c2-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="9b6c2-158">JSON</span><span class="sxs-lookup"><span data-stu-id="9b6c2-158">JSON</span></span>

<span data-ttu-id="9b6c2-159">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="9b6c2-159">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="9b6c2-160">要求</span><span class="sxs-lookup"><span data-stu-id="9b6c2-160">Request</span></span>

<span data-ttu-id="9b6c2-161">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9b6c2-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="9b6c2-162">応答</span><span class="sxs-lookup"><span data-stu-id="9b6c2-162">Response</span></span>

<span data-ttu-id="9b6c2-163">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9b6c2-163">The following is an example of the response.</span></span>

> <span data-ttu-id="9b6c2-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9b6c2-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
