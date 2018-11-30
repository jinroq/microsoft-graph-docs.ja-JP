---
title: 'synchronizationJob: validateCredentials'
description: 資格情報は、テナントの有効なことを検証します。
ms.openlocfilehash: b4f488787474158172800fe23d7d0ae78ef6a366
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068072"
---
# <a name="synchronizationjob-validatecredentials"></a><span data-ttu-id="324b4-103">synchronizationJob: validateCredentials</span><span class="sxs-lookup"><span data-stu-id="324b4-103">synchronizationJob: validateCredentials</span></span>

> <span data-ttu-id="324b4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="324b4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="324b4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="324b4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="324b4-106">資格情報は、テナントの有効なことを検証します。</span><span class="sxs-lookup"><span data-stu-id="324b4-106">Validate that the credentials are valid in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="324b4-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="324b4-107">Permissions</span></span>
<span data-ttu-id="324b4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="324b4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="324b4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="324b4-110">Permission type</span></span>                        | <span data-ttu-id="324b4-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="324b4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="324b4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="324b4-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="324b4-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="324b4-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="324b4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="324b4-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="324b4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="324b4-115">Not supported.</span></span> |
|<span data-ttu-id="324b4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="324b4-116">Application</span></span>                            |<span data-ttu-id="324b4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="324b4-117">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="324b4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="324b4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials

```
## <a name="request-headers"></a><span data-ttu-id="324b4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="324b4-119">Request headers</span></span>
| <span data-ttu-id="324b4-120">名前</span><span class="sxs-lookup"><span data-stu-id="324b4-120">Name</span></span>       | <span data-ttu-id="324b4-121">説明</span><span class="sxs-lookup"><span data-stu-id="324b4-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="324b4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="324b4-122">Authorization</span></span>  | <span data-ttu-id="324b4-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="324b4-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="324b4-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="324b4-124">Request body</span></span>
<span data-ttu-id="324b4-125">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="324b4-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="324b4-126">パラメーター</span><span class="sxs-lookup"><span data-stu-id="324b4-126">Parameter</span></span>    | <span data-ttu-id="324b4-127">型</span><span class="sxs-lookup"><span data-stu-id="324b4-127">Type</span></span>   |<span data-ttu-id="324b4-128">説明</span><span class="sxs-lookup"><span data-stu-id="324b4-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="324b4-129">useSavedCredentials</span><span class="sxs-lookup"><span data-stu-id="324b4-129">useSavedCredentials</span></span>|<span data-ttu-id="324b4-130">ブール値</span><span class="sxs-lookup"><span data-stu-id="324b4-130">Boolean</span></span>|<span data-ttu-id="324b4-131">`true`、`credentials`パラメーターは無視され、代わりに (存在する場合) には、以前に保存した資格情報が検証されます。</span><span class="sxs-lookup"><span data-stu-id="324b4-131">When `true`, the `credentials` parameter will be ignored and the previously saved credentials (if any) will be validated instead.</span></span> |
|<span data-ttu-id="324b4-132">資格情報</span><span class="sxs-lookup"><span data-stu-id="324b4-132">credentials</span></span>|<span data-ttu-id="324b4-133">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="324b4-133">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="324b4-134">検証する資格情報。</span><span class="sxs-lookup"><span data-stu-id="324b4-134">Credentials to validate.</span></span> <span data-ttu-id="324b4-135">無視する場合、`useSavedCredentials`のパラメーターは、 `true`。</span><span class="sxs-lookup"><span data-stu-id="324b4-135">Ignored when the `useSavedCredentials` parameter is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="324b4-136">応答</span><span class="sxs-lookup"><span data-stu-id="324b4-136">Response</span></span>
<span data-ttu-id="324b4-137">検証は成功を返します、`204, No Content`応答コード。</span><span class="sxs-lookup"><span data-stu-id="324b4-137">If validation is successful, this method returns a `204, No Content` response code.</span></span> <span data-ttu-id="324b4-138">応答本体には何もは返されません。</span><span class="sxs-lookup"><span data-stu-id="324b4-138">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="324b4-139">例</span><span class="sxs-lookup"><span data-stu-id="324b4-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="324b4-140">要求</span><span class="sxs-lookup"><span data-stu-id="324b4-140">Request</span></span>
<span data-ttu-id="324b4-141">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="324b4-141">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="324b4-142">応答</span><span class="sxs-lookup"><span data-stu-id="324b4-142">Response</span></span>
<span data-ttu-id="324b4-143">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="324b4-143">The following is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationJob: validateCredentials",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->