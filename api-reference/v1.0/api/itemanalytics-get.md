---
author: daspek
ms.author: dspektor
title: ItemAnalytics の取得
description: このリソースの下で行われたビューに関する itemAnalytics を取得します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 3923237cd608207f0c06f4acd3bb241b2808605d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461609"
---
# <a name="get-itemanalytics"></a><span data-ttu-id="bb4a0-103">ItemAnalytics の取得</span><span class="sxs-lookup"><span data-stu-id="bb4a0-103">Get itemAnalytics</span></span>

<span data-ttu-id="bb4a0-104">このリソースの下で行われたビューに関する[Itemanalytics][]を取得します。</span><span class="sxs-lookup"><span data-stu-id="bb4a0-104">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="bb4a0-105">**Itemanalytics**リソースは、およびのアクティビティの`allTime`統計を取得する便利な`lastSevenDays`方法です。</span><span class="sxs-lookup"><span data-stu-id="bb4a0-105">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="bb4a0-106">ユーザー設定の時間範囲または間隔の場合は、 [getActivitiesByInterval][] API を使用します。</span><span class="sxs-lookup"><span data-stu-id="bb4a0-106">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="bb4a0-107">**注:\*\*\*\*Itemanalytics**リソースは、すべての[国内展開](/graph/deployments)でまだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="bb4a0-107">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="permissions"></a><span data-ttu-id="bb4a0-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bb4a0-110">Permissions</span></span>

<span data-ttu-id="bb4a0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb4a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb4a0-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bb4a0-113">Permission type</span></span>                        | <span data-ttu-id="bb4a0-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bb4a0-114">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="bb4a0-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bb4a0-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="bb4a0-116">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb4a0-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="bb4a0-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bb4a0-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb4a0-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb4a0-118">Not supported.</span></span>
|<span data-ttu-id="bb4a0-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bb4a0-119">Application</span></span>                            | <span data-ttu-id="bb4a0-120">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb4a0-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="bb4a0-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bb4a0-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bb4a0-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="bb4a0-122">Optional query parameters</span></span>
<span data-ttu-id="bb4a0-123">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="bb4a0-123">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb4a0-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bb4a0-124">Request headers</span></span>

| <span data-ttu-id="bb4a0-125">名前</span><span class="sxs-lookup"><span data-stu-id="bb4a0-125">Name</span></span>      |<span data-ttu-id="bb4a0-126">説明</span><span class="sxs-lookup"><span data-stu-id="bb4a0-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bb4a0-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb4a0-127">Authorization</span></span>  | <span data-ttu-id="bb4a0-128">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="bb4a0-128">Bearer {code}.</span></span> <span data-ttu-id="bb4a0-129">必須です。</span><span class="sxs-lookup"><span data-stu-id="bb4a0-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb4a0-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="bb4a0-130">Request body</span></span>

<span data-ttu-id="bb4a0-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bb4a0-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb4a0-132">応答</span><span class="sxs-lookup"><span data-stu-id="bb4a0-132">Response</span></span> 

<span data-ttu-id="bb4a0-133">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[itemanalytics][]オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="bb4a0-133">If successful, this method returns a `200 OK` response code and a collection of [itemAnalytics][] object in the response body.</span></span> 

## <a name="example"></a><span data-ttu-id="bb4a0-134">例</span><span class="sxs-lookup"><span data-stu-id="bb4a0-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb4a0-135">要求</span><span class="sxs-lookup"><span data-stu-id="bb4a0-135">Request</span></span>

<!-- { "blockType": "request", "name": "get-analytics" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
```

### <a name="response"></a><span data-ttu-id="bb4a0-136">応答</span><span class="sxs-lookup"><span data-stu-id="bb4a0-136">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.itemAnalytics", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "allTime": {
        "access": {
            "actionCount": 123,
            "actorCount": 89
        }
    },
    "lastSevenDays": {
        "access": {
            "actionCount": 52,
            "actorCount": 41
        }
    }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bb4a0-137">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="bb4a0-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bb4a0-138">C#</span><span class="sxs-lookup"><span data-stu-id="bb4a0-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-analytics-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bb4a0-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="bb4a0-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-analytics-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get analytics",
  "suppressions": [
    "Error: /api-reference/v1.0/api/itemanalytics-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/itemanalytics-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
  ]
}
-->
