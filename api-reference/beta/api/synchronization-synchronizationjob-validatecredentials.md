---
title: '同期ジョブ: validateCredentials'
description: テナントで資格情報が有効であることを検証します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ee711e1ef6a74c667ac2f6c72bd45c9ac2e9eec4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869237"
---
# <a name="synchronizationjob-validatecredentials"></a><span data-ttu-id="4d220-103">同期ジョブ: validateCredentials</span><span class="sxs-lookup"><span data-stu-id="4d220-103">synchronizationJob: validateCredentials</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d220-104">テナントで資格情報が有効であることを検証します。</span><span class="sxs-lookup"><span data-stu-id="4d220-104">Validate that the credentials are valid in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d220-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4d220-105">Permissions</span></span>
<span data-ttu-id="4d220-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d220-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d220-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4d220-108">Permission type</span></span>                        | <span data-ttu-id="4d220-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4d220-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d220-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4d220-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="4d220-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d220-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="4d220-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4d220-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="4d220-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d220-113">Not supported.</span></span> |
|<span data-ttu-id="4d220-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4d220-114">Application</span></span>                            |<span data-ttu-id="4d220-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d220-115">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="4d220-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4d220-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials

```
## <a name="request-headers"></a><span data-ttu-id="4d220-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4d220-117">Request headers</span></span>
| <span data-ttu-id="4d220-118">名前</span><span class="sxs-lookup"><span data-stu-id="4d220-118">Name</span></span>       | <span data-ttu-id="4d220-119">説明</span><span class="sxs-lookup"><span data-stu-id="4d220-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4d220-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d220-120">Authorization</span></span>  | <span data-ttu-id="4d220-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4d220-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d220-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="4d220-122">Request body</span></span>
<span data-ttu-id="4d220-123">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="4d220-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4d220-124">パラメーター</span><span class="sxs-lookup"><span data-stu-id="4d220-124">Parameter</span></span>    | <span data-ttu-id="4d220-125">型</span><span class="sxs-lookup"><span data-stu-id="4d220-125">Type</span></span>   |<span data-ttu-id="4d220-126">説明</span><span class="sxs-lookup"><span data-stu-id="4d220-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d220-127">の場合は、資格情報</span><span class="sxs-lookup"><span data-stu-id="4d220-127">useSavedCredentials</span></span>|<span data-ttu-id="4d220-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d220-128">Boolean</span></span>|<span data-ttu-id="4d220-129">の`true`場合、 `credentials`パラメーターは無視され、以前に保存された資格情報 (ある場合) が代わりに検証されます。</span><span class="sxs-lookup"><span data-stu-id="4d220-129">When `true`, the `credentials` parameter will be ignored and the previously saved credentials (if any) will be validated instead.</span></span> |
|<span data-ttu-id="4d220-130">クリデンシャル</span><span class="sxs-lookup"><span data-stu-id="4d220-130">credentials</span></span>|<span data-ttu-id="4d220-131">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4d220-131">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="4d220-132">検証する資格情報。</span><span class="sxs-lookup"><span data-stu-id="4d220-132">Credentials to validate.</span></span> <span data-ttu-id="4d220-133">`useSavedCredentials`パラメーターがの場合は`true`無視されます。</span><span class="sxs-lookup"><span data-stu-id="4d220-133">Ignored when the `useSavedCredentials` parameter is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="4d220-134">応答</span><span class="sxs-lookup"><span data-stu-id="4d220-134">Response</span></span>
<span data-ttu-id="4d220-135">検証が成功した場合、このメソッド`204, No Content`は応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="4d220-135">If validation is successful, this method returns a `204, No Content` response code.</span></span> <span data-ttu-id="4d220-136">応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="4d220-136">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d220-137">例</span><span class="sxs-lookup"><span data-stu-id="4d220-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4d220-138">要求</span><span class="sxs-lookup"><span data-stu-id="4d220-138">Request</span></span>
<span data-ttu-id="4d220-139">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4d220-139">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4d220-140">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4d220-140">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="4d220-141">C#</span><span class="sxs-lookup"><span data-stu-id="4d220-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-validatecredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4d220-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="4d220-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-validatecredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4d220-143">目的-C</span><span class="sxs-lookup"><span data-stu-id="4d220-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-validatecredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4d220-144">Java</span><span class="sxs-lookup"><span data-stu-id="4d220-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-validatecredentials-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4d220-145">応答</span><span class="sxs-lookup"><span data-stu-id="4d220-145">Response</span></span>
<span data-ttu-id="4d220-146">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4d220-146">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

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
  ]
}
-->
