---
title: 'reportRoot: getOffice365ActivationsUserCounts'
description: 有効になっているユーザーとデスクトップやデバイスに Office のサブスクリプションをアクティブ化または共有のコンピューターの数を取得します。
ms.openlocfilehash: 4d7d75d084408e4d0d8af0473397252fdcbe7aa9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066275"
---
# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="38c3a-103">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="38c3a-103">reportRoot: getOffice365ActivationsUserCounts</span></span>

> <span data-ttu-id="38c3a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="38c3a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="38c3a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="38c3a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="38c3a-106">有効になっているユーザーとデスクトップやデバイスに Office のサブスクリプションをアクティブ化または共有のコンピューターの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="38c3a-106">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices or shared computers.</span></span>

> <span data-ttu-id="38c3a-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Microsoft Office ライセンス認証](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="38c3a-107">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="38c3a-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="38c3a-108">Permissions</span></span>

<span data-ttu-id="38c3a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="38c3a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="38c3a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="38c3a-111">Permission type</span></span>                        | <span data-ttu-id="38c3a-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="38c3a-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="38c3a-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="38c3a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="38c3a-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="38c3a-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="38c3a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="38c3a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38c3a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="38c3a-116">Not supported.</span></span>                           |
| <span data-ttu-id="38c3a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="38c3a-117">Application</span></span>                            | <span data-ttu-id="38c3a-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="38c3a-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="38c3a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="38c3a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="query-parameters"></a><span data-ttu-id="38c3a-120">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="38c3a-120">Query parameters</span></span>

<span data-ttu-id="38c3a-121">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="38c3a-121">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="38c3a-122">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="38c3a-122">The default output type is text/csv.</span></span> <span data-ttu-id="38c3a-123">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="38c3a-123">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="38c3a-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="38c3a-124">Request headers</span></span>

| <span data-ttu-id="38c3a-125">名前</span><span class="sxs-lookup"><span data-stu-id="38c3a-125">Name</span></span>          | <span data-ttu-id="38c3a-126">説明</span><span class="sxs-lookup"><span data-stu-id="38c3a-126">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="38c3a-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="38c3a-127">Authorization</span></span> | <span data-ttu-id="38c3a-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="38c3a-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="38c3a-130">応答</span><span class="sxs-lookup"><span data-stu-id="38c3a-130">Response</span></span>

### <a name="csv"></a><span data-ttu-id="38c3a-131">CSV</span><span class="sxs-lookup"><span data-stu-id="38c3a-131">CSV</span></span>

<span data-ttu-id="38c3a-132">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="38c3a-132">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="38c3a-133">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="38c3a-133">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="38c3a-134">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="38c3a-134">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="38c3a-135">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="38c3a-135">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="38c3a-136">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="38c3a-136">Report Refresh Date</span></span>
- <span data-ttu-id="38c3a-137">製品の種類</span><span class="sxs-lookup"><span data-stu-id="38c3a-137">Product Type</span></span>
- <span data-ttu-id="38c3a-138">割り当て済み</span><span class="sxs-lookup"><span data-stu-id="38c3a-138">Assigned</span></span>
- <span data-ttu-id="38c3a-139">アクティブ</span><span class="sxs-lookup"><span data-stu-id="38c3a-139">Activated</span></span>
- <span data-ttu-id="38c3a-140">共有のコンピューターのライセンス認証</span><span class="sxs-lookup"><span data-stu-id="38c3a-140">Shared Computer Activation</span></span>

### <a name="json"></a><span data-ttu-id="38c3a-141">JSON</span><span class="sxs-lookup"><span data-stu-id="38c3a-141">JSON</span></span>

<span data-ttu-id="38c3a-142">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の**[office365ActivationsUserCounts](../resources/office365activationsusercounts.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="38c3a-142">If successful, this method returns a `200 OK` response code and an **[office365ActivationsUserCounts](../resources/office365activationsusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38c3a-143">使用例</span><span class="sxs-lookup"><span data-stu-id="38c3a-143">Example</span></span>

### <a name="csv"></a><span data-ttu-id="38c3a-144">CSV</span><span class="sxs-lookup"><span data-stu-id="38c3a-144">CSV</span></span>

<span data-ttu-id="38c3a-145">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="38c3a-145">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="38c3a-146">要求</span><span class="sxs-lookup"><span data-stu-id="38c3a-146">Request</span></span>

<span data-ttu-id="38c3a-147">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="38c3a-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserCounts?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="38c3a-148">応答</span><span class="sxs-lookup"><span data-stu-id="38c3a-148">Response</span></span>

<span data-ttu-id="38c3a-149">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="38c3a-149">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="38c3a-150">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="38c3a-150">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="38c3a-151">JSON</span><span class="sxs-lookup"><span data-stu-id="38c3a-151">JSON</span></span>

<span data-ttu-id="38c3a-152">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="38c3a-152">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="38c3a-153">要求</span><span class="sxs-lookup"><span data-stu-id="38c3a-153">Request</span></span>

<span data-ttu-id="38c3a-154">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="38c3a-154">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserCounts?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="38c3a-155">応答</span><span class="sxs-lookup"><span data-stu-id="38c3a-155">Response</span></span>

<span data-ttu-id="38c3a-156">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="38c3a-156">The following example shows the response.</span></span>

> <span data-ttu-id="38c3a-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="38c3a-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
