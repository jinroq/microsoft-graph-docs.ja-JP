---
title: '同期ジョブ: validateCredentials'
description: テナントで資格情報が有効であることを検証します。
localization_priority: Normal
ms.openlocfilehash: aede9dbb505ce43eee3399972ad26958cb9ff1b8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271317"
---
# <a name="synchronizationjob-validatecredentials"></a><span data-ttu-id="09e86-103">同期ジョブ: validateCredentials</span><span class="sxs-lookup"><span data-stu-id="09e86-103">synchronizationJob: validateCredentials</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09e86-104">テナントで資格情報が有効であることを検証します。</span><span class="sxs-lookup"><span data-stu-id="09e86-104">Validate that the credentials are valid in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="09e86-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="09e86-105">Permissions</span></span>
<span data-ttu-id="09e86-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="09e86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09e86-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="09e86-108">Permission type</span></span>                        | <span data-ttu-id="09e86-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="09e86-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="09e86-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="09e86-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="09e86-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09e86-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="09e86-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="09e86-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="09e86-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09e86-113">Not supported.</span></span> |
|<span data-ttu-id="09e86-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="09e86-114">Application</span></span>                            |<span data-ttu-id="09e86-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09e86-115">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="09e86-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="09e86-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials

```
## <a name="request-headers"></a><span data-ttu-id="09e86-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="09e86-117">Request headers</span></span>
| <span data-ttu-id="09e86-118">名前</span><span class="sxs-lookup"><span data-stu-id="09e86-118">Name</span></span>       | <span data-ttu-id="09e86-119">説明</span><span class="sxs-lookup"><span data-stu-id="09e86-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="09e86-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="09e86-120">Authorization</span></span>  | <span data-ttu-id="09e86-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="09e86-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="09e86-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="09e86-122">Request body</span></span>
<span data-ttu-id="09e86-123">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="09e86-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="09e86-124">パラメーター</span><span class="sxs-lookup"><span data-stu-id="09e86-124">Parameter</span></span>    | <span data-ttu-id="09e86-125">型</span><span class="sxs-lookup"><span data-stu-id="09e86-125">Type</span></span>   |<span data-ttu-id="09e86-126">説明</span><span class="sxs-lookup"><span data-stu-id="09e86-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09e86-127">の場合は、資格情報</span><span class="sxs-lookup"><span data-stu-id="09e86-127">useSavedCredentials</span></span>|<span data-ttu-id="09e86-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="09e86-128">Boolean</span></span>|<span data-ttu-id="09e86-129">の`true`場合、 `credentials`パラメーターは無視され、以前に保存された資格情報 (ある場合) が代わりに検証されます。</span><span class="sxs-lookup"><span data-stu-id="09e86-129">When `true`, the `credentials` parameter will be ignored and the previously saved credentials (if any) will be validated instead.</span></span> |
|<span data-ttu-id="09e86-130">クリデンシャル</span><span class="sxs-lookup"><span data-stu-id="09e86-130">credentials</span></span>|<span data-ttu-id="09e86-131">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="09e86-131">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="09e86-132">検証する資格情報。</span><span class="sxs-lookup"><span data-stu-id="09e86-132">Credentials to validate.</span></span> <span data-ttu-id="09e86-133">`useSavedCredentials`パラメーターがの場合は`true`無視されます。</span><span class="sxs-lookup"><span data-stu-id="09e86-133">Ignored when the `useSavedCredentials` parameter is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="09e86-134">応答</span><span class="sxs-lookup"><span data-stu-id="09e86-134">Response</span></span>
<span data-ttu-id="09e86-135">検証が成功した場合、このメソッド`204, No Content`は応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="09e86-135">If validation is successful, this method returns a `204, No Content` response code.</span></span> <span data-ttu-id="09e86-136">応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="09e86-136">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09e86-137">例</span><span class="sxs-lookup"><span data-stu-id="09e86-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="09e86-138">要求</span><span class="sxs-lookup"><span data-stu-id="09e86-138">Request</span></span>
<span data-ttu-id="09e86-139">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="09e86-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_validatecredentials"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials
Content-type: application/json
Content-length: 218

{ 
    credentials: [ 
        { key: "UserName", value: "user@domain.com" },
        { key: "Password", value: "password-value" }
    ]
}
```

##### <a name="response"></a><span data-ttu-id="09e86-140">応答</span><span class="sxs-lookup"><span data-stu-id="09e86-140">Response</span></span>
<span data-ttu-id="09e86-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="09e86-141">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="09e86-142">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="09e86-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="09e86-143">C#</span><span class="sxs-lookup"><span data-stu-id="09e86-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/synchronizationjob_validatecredentials-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="09e86-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="09e86-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/synchronizationjob_validatecredentials-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="09e86-145">目的-C</span><span class="sxs-lookup"><span data-stu-id="09e86-145">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/synchronizationjob_validatecredentials-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob: validateCredentials",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-validatecredentials.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-validatecredentials.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-validatecredentials.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
