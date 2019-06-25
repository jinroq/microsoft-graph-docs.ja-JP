---
title: JSON バッチ処理を使用した複数要求の単一 HTTP 呼び出しへの統合
description: JSON のバッチ処理を使用すると、複数の要求を単一の JSON オブジェクトに統合することにより、アプリケーションを最適化することができます。たとえば、次のような互いに無関係なデータからビューを作成する場合、
author: piotrci
localization_priority: Priority
ms.openlocfilehash: 7b725545008cd512ef0058d678d057f567f40618
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/22/2019
ms.locfileid: "35133825"
---
# <a name="combine-multiple-requests-in-one-http-call-using-json-batching"></a><span data-ttu-id="33522-104">JSON バッチ処理を使用した複数要求の単一 HTTP 呼び出しへの統合</span><span class="sxs-lookup"><span data-stu-id="33522-104">Combine multiple requests in one HTTP call using JSON batching</span></span>

<span data-ttu-id="33522-p102">JSON のバッチ処理を使用すると、複数の要求を単一の JSON オブジェクトに統合することにより、アプリケーションを最適化することができます。たとえば、次のような互いに無関係なデータからビューを作成する場合、</span><span class="sxs-lookup"><span data-stu-id="33522-p102">JSON batching allows you to optimize your application by combining multiple requests into a single JSON object. For example, a client might want to compose a view of unrelated data such as:</span></span>

1. <span data-ttu-id="33522-107">OneDrive に保存されているイメージ</span><span class="sxs-lookup"><span data-stu-id="33522-107">An image stored in OneDrive</span></span>
2. <span data-ttu-id="33522-108">Planner タスクのリスト</span><span class="sxs-lookup"><span data-stu-id="33522-108">A list of Planner tasks</span></span>
3. <span data-ttu-id="33522-109">グループの予定表</span><span class="sxs-lookup"><span data-stu-id="33522-109">The calendar for a group</span></span>

<span data-ttu-id="33522-110">これらの 3 つの要求を 1 つのバッチ要求にまとめることで、ネットワーク待機時間を大きく削減できます。</span><span class="sxs-lookup"><span data-stu-id="33522-110">Combining these three individual requests into a single batch request can save the application significant network latency.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/tzWGOp8zYh8]

## <a name="first-json-batch-request"></a><span data-ttu-id="33522-111">JSON の最初のバッチ要求</span><span class="sxs-lookup"><span data-stu-id="33522-111">First JSON batch request</span></span>

<span data-ttu-id="33522-p103">まず、前の例の JSON バッチ要求を作成します。このシナリオでは、各要求に相互の依存関係はありません。よって、バッチ要求には、各要求を任意の順序で配置できます。</span><span class="sxs-lookup"><span data-stu-id="33522-p103">First you construct the JSON batch request for the previous example. In this scenario, the individual requests are not interdependent in any way and therefore can be placed into the batch request in any order.</span></span>

```http
POST https://graph.microsoft.com/v1.0/$batch
Accept: application/json
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "id": "1",
      "method": "GET",
      "url": "/me/drive/root:/{file}:/content"
    },
    {
      "id": "2",
      "method": "GET",
      "url": "/me/planner/tasks"
    },
    {
      "id": "3",
      "method": "GET",
      "url": "/groups/{id}/events"
    },
    {
      "id": "4",
      "url": "/me",
      "method": "PATCH",
      "body": {
        "city" : "Redmond"
      },
      "headers": {
        "Content-Type": "application/json"
      }
    }
  ]
}
```

<span data-ttu-id="33522-p104">バッチ要求への応答は、異なる順序で返されることがあります。`id` プロパティを使い、各要求と応答を対応させることができます。</span><span class="sxs-lookup"><span data-stu-id="33522-p104">Responses to the batched requests might appear in a different order. The `id` property can be used to correlate individual requests and responses.</span></span>

```http
200 OK
Content-Type: application/json
```

```json
{
  "responses": [
    {
      "id": "1",
      "status": 302,
      "headers": {
        "location": "https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi"
      }
    },
    {
      "id": "3",
      "status": 401,
      "body": {
        "error": {
          "code": "Forbidden",
          "message": "..."
        }
      }
    },
    {
      "id": "2",
      "status": 200,
      "body": {
        "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.plannerTask)",
        "value": []
      }
    },
    {
      "id": "4",
      "status": 204,
      "body": null
    }
  ]
}
```

## <a name="request-format"></a><span data-ttu-id="33522-116">要求の形式</span><span class="sxs-lookup"><span data-stu-id="33522-116">Request format</span></span>

<span data-ttu-id="33522-117">バッチ要求は常に `/$batch` エンドポイントに対して `POST` を使用して送信されます。</span><span class="sxs-lookup"><span data-stu-id="33522-117">Batch requests are always sent using `POST` to the `/$batch` endpoint.</span></span>

<span data-ttu-id="33522-p105">JSON バッチ要求本文は必須のプロパティ `requests` をもつ単一の JSON オブジェクトです。`requests` プロパティは個別要求の配列です。個別要求には、それぞれ `id`、`method`、および`url` プロパティが必要です。</span><span class="sxs-lookup"><span data-stu-id="33522-p105">A JSON batch request body consists of a single JSON object with one required property: `requests`. The `requests` property is an array of individual requests. For each individual request, the `id`, `method`, and `url` properties are required.</span></span>

<span data-ttu-id="33522-p106">
            \`id\` プロパティは主に個別の応答と要求を関連付けるための相互関係値として機能します。これにより、サーバーでは最も効率のよい順序でバッチの要求処理が可能となります。</span><span class="sxs-lookup"><span data-stu-id="33522-p106">The `id` property functions primarily as a correlation value to associate individual responses with requests. This allows the server to process requests in the batch in the most efficient order.</span></span>

<span data-ttu-id="33522-p107">
            `method\` および \`url\` プロパティは、指定した任意の HTTP 要求の先頭と同一のものです。メソッドは HTTP であり、URL は各要求が通常送信される宛先のリソースの URL です。</span><span class="sxs-lookup"><span data-stu-id="33522-p107">The `method` and `url` properties are exactly what you would see at the start of any given HTTP request. The method is the HTTP method, and the URL is the resource URL the individual request would typically be sent to.</span></span>

<span data-ttu-id="33522-125">個々の要求は、任意で、`headers` プロパティと `body` プロパティを含むこともできます。</span><span class="sxs-lookup"><span data-stu-id="33522-125">Individual requests can optionally also contain a `headers` property and a `body` property.</span></span> <span data-ttu-id="33522-126">これら両方のプロパティは、前の例のように、通常 JSON オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="33522-126">Both of these properties are typically JSON objects, as shown in the previous example.</span></span> <span data-ttu-id="33522-127">場合によっては、`body` は JSON オブジェクトではなく、Base64 で URL エンコードされた値となることがあります。たとえば、本文が画像である場合などです。</span><span class="sxs-lookup"><span data-stu-id="33522-127">In some cases, the `body` might be a base64 URL-encoded value rather than a JSON object - for example, when the body is an image.</span></span> <span data-ttu-id="33522-128">要求に `body` が含まれている場合、`headers` オブジェクトには `Content-Type` の値が含まれている必要があります。</span><span class="sxs-lookup"><span data-stu-id="33522-128">When a `body` is included with the request, the `headers` object must contain a value for `Content-Type`.</span></span>

## <a name="response-format"></a><span data-ttu-id="33522-129">応答の形式</span><span class="sxs-lookup"><span data-stu-id="33522-129">Response format</span></span>

<span data-ttu-id="33522-p109">JSON バッチ要求への応答の形式は、要求の形式と似ています。主な違いを以下に示します。</span><span class="sxs-lookup"><span data-stu-id="33522-p109">The response format for JSON batch requests is similar to the request format. The following are the key differences:</span></span>

* <span data-ttu-id="33522-132">メインの JSON オブジェクトのプロパティは、`requests` ではなく、`responses` と命名されている。</span><span class="sxs-lookup"><span data-stu-id="33522-132">The property in the main JSON object is named `responses` as opposed to `requests`.</span></span>
* <span data-ttu-id="33522-133">個々の応答は、要求と異なる順序で返されることがある。</span><span class="sxs-lookup"><span data-stu-id="33522-133">Individual responses might appear in a different order than the requests.</span></span>
* <span data-ttu-id="33522-p110">`method` と `url` ではなく、個々の応答には `status` プロパティが存在する。`status` の値は、HTTP ステータス コードを表す数字である。</span><span class="sxs-lookup"><span data-stu-id="33522-p110">Rather than `method` and `url`, individual responses have a `status` property. The value of `status` is a number that represents the HTTP status code.</span></span>

<span data-ttu-id="33522-p111">バッチ応答のステータス コードは、通常 `200` または `400` です。バッチ要求自体が正しい形式でない場合、状態コードは `400` になります。バッチ要求が解析可能であれば、状態コードは `200` になります。バッチ応答のステータス コード `200` はバッチ内の個々の要求が成功したことを示すものではありません。そのため、`responses` プロパティの個々の応答にステータス コードがあります。</span><span class="sxs-lookup"><span data-stu-id="33522-p111">The status code on a batch response is typically `200` or `400`. If the batch request itself is malformed, the status code is `400`. If the batch request is parseable, the status code is `200`. A `200` status code on the batch response does not indicate that the individual requests inside the batch succeeded. This is why each individual response in the `responses` property has a status code.</span></span>

<span data-ttu-id="33522-p112">`responses` プロパティに加え、バッチ応答には `nextLink` プロパティが存在することがあります。これにより、Microsoft Graph が個々の要求が完了するとすぐにバッチ応答を返すようにできます。個々の応答を確実にすべて受信するため、`nextLink` が存在する限りそのリンクを追い続けます。</span><span class="sxs-lookup"><span data-stu-id="33522-p112">In addition to the `responses` property, there might be a `nextLink` property in the batch response. This allows Microsoft Graph to return a batch response as soon as any of the individual requests has completed. To ensure that all individual responses have been received, continue to follow the `nextLink` as long as it exists.</span></span>

## <a name="sequencing-requests-with-the-dependson-property"></a><span data-ttu-id="33522-144">dependsOn プロパティによる要求の順序指定</span><span class="sxs-lookup"><span data-stu-id="33522-144">Sequencing requests with the dependsOn property</span></span>

<span data-ttu-id="33522-p113">`dependsOn` プロパティを使い、個別の要求の実行順序を指定できます。このプロパティは個別の要求の `id` を参照する文字列の配列です。このため、`id` の値は一意である必要があります。たとえば、次の要求で、クライアントは要求 1 と 3 を先に実行し、その後に 2 そして 4 を実行するよう指定しています。</span><span class="sxs-lookup"><span data-stu-id="33522-p113">Individual requests can be executed in a specified order by using the `dependsOn` property. This property is an array of strings that reference the `id` of a different individual request. For this reason, the values for `id` must be unique. For example, in the following request, the client is specifying that requests 1 and 3 should be run first, then request 2, then request 4.</span></span>

```json
{
  "requests": [
    {
      "id": "1",
      "method": "GET",
      "url": "..."
    },
    {
      "id": "2",
      "dependsOn": [ "1" ],
      "method": "GET",
      "url": "..."
    },
    {
      "id": "3",
      "method": "GET",
      "url": "..."
    },
    {
      "id": "4",
      "dependsOn": [ "2" ],
      "method": "GET",
      "url": "..."
    }
  ]
}
```

<span data-ttu-id="33522-149">個々の要求が失敗した場合、その要求に依存するすべての要求が失敗し、ステータス コードは `424` (Failed Dependency) になります。</span><span class="sxs-lookup"><span data-stu-id="33522-149">If an individual request fails, any request that depends on that request fails with status code `424` (Failed Dependency).</span></span>

## <a name="bypassing-url-length-limitations-with-batching"></a><span data-ttu-id="33522-150">バッチ処理による URL 長さ制限の回避</span><span class="sxs-lookup"><span data-stu-id="33522-150">Bypassing URL length limitations with batching</span></span>

<span data-ttu-id="33522-p114">他にも、URL の長さの制限を回避するために JSON バッチ処理を利用できます。フィルター句が複雑な場合、URL の長さがブラウザーまたはその他の HTTP クライアントによる制限を超えることがあります。JSON バッチ処理を使うと、長い URL は単純に要求のペイロードとなるため、制限を回避できます。</span><span class="sxs-lookup"><span data-stu-id="33522-p114">An additional use case for JSON batching is to bypass URL length limitations. In cases where the filter clause is complex, the URL length might surpass limitations built into browsers or other HTTP clients. You can use JSON batching as a workaround for running these requests because the lengthy URL simply becomes part of the request payload.</span></span>

## <a name="known-issues"></a><span data-ttu-id="33522-154">既知の問題</span><span class="sxs-lookup"><span data-stu-id="33522-154">Known issues</span></span>

<span data-ttu-id="33522-155">バッチ処理に関連する現在の制限事項の一覧は「[既知の問題][batching-known-issues]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="33522-155">For a list of current limitations related to batching, see [known issues][batching-known-issues].</span></span>

[batching-known-issues]: known-issues.md#json-batching
[odata-4.01-json]: https://www.oasis-open.org/committees/download.php/60365/odata-json-format-v4.01-wd02-2017-03-24.docx


## <a name="see-also"></a><span data-ttu-id="33522-156">関連項目</span><span class="sxs-lookup"><span data-stu-id="33522-156">See also</span></span>

<span data-ttu-id="33522-p115">JSON のバッチ要求/応答形式の詳細については「[OData JSON 形式バージョン 4.01 仕様][odata-4.01-json]」のセクション 18 を参照してください。この仕様は現在ドラフト バージョンですが、変更の予定はありません。</span><span class="sxs-lookup"><span data-stu-id="33522-p115">For more information about the JSON batch request/response format, see the [OData JSON Format Version 4.01 specification][odata-4.01-json], section 18. Note that this specification is currently in a draft version, but is not expected to change.</span></span>

