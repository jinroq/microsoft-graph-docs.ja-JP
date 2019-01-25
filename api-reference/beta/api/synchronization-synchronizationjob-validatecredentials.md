---
title: 'synchronizationJob: validateCredentials'
description: 資格情報は、テナントの有効なことを検証します。
localization_priority: Normal
ms.openlocfilehash: 122d673e89f15697b2fdeefbcefb516cf9ad89ca
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519004"
---
# <a name="synchronizationjob-validatecredentials"></a><span data-ttu-id="02cb1-103">synchronizationJob: validateCredentials</span><span class="sxs-lookup"><span data-stu-id="02cb1-103">synchronizationJob: validateCredentials</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02cb1-104">資格情報は、テナントの有効なことを検証します。</span><span class="sxs-lookup"><span data-stu-id="02cb1-104">Validate that the credentials are valid in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="02cb1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="02cb1-105">Permissions</span></span>
<span data-ttu-id="02cb1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="02cb1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02cb1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="02cb1-108">Permission type</span></span>                        | <span data-ttu-id="02cb1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="02cb1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="02cb1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="02cb1-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="02cb1-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02cb1-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="02cb1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="02cb1-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="02cb1-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02cb1-113">Not supported.</span></span> |
|<span data-ttu-id="02cb1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="02cb1-114">Application</span></span>                            |<span data-ttu-id="02cb1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02cb1-115">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="02cb1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="02cb1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials

```
## <a name="request-headers"></a><span data-ttu-id="02cb1-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="02cb1-117">Request headers</span></span>
| <span data-ttu-id="02cb1-118">名前</span><span class="sxs-lookup"><span data-stu-id="02cb1-118">Name</span></span>       | <span data-ttu-id="02cb1-119">説明</span><span class="sxs-lookup"><span data-stu-id="02cb1-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="02cb1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="02cb1-120">Authorization</span></span>  | <span data-ttu-id="02cb1-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="02cb1-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="02cb1-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="02cb1-122">Request body</span></span>
<span data-ttu-id="02cb1-123">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="02cb1-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="02cb1-124">パラメーター</span><span class="sxs-lookup"><span data-stu-id="02cb1-124">Parameter</span></span>    | <span data-ttu-id="02cb1-125">型</span><span class="sxs-lookup"><span data-stu-id="02cb1-125">Type</span></span>   |<span data-ttu-id="02cb1-126">説明</span><span class="sxs-lookup"><span data-stu-id="02cb1-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02cb1-127">useSavedCredentials</span><span class="sxs-lookup"><span data-stu-id="02cb1-127">useSavedCredentials</span></span>|<span data-ttu-id="02cb1-128">ブール値</span><span class="sxs-lookup"><span data-stu-id="02cb1-128">Boolean</span></span>|<span data-ttu-id="02cb1-129">`true`、`credentials`パラメーターは無視され、代わりに (存在する場合) には、以前に保存した資格情報が検証されます。</span><span class="sxs-lookup"><span data-stu-id="02cb1-129">When `true`, the `credentials` parameter will be ignored and the previously saved credentials (if any) will be validated instead.</span></span> |
|<span data-ttu-id="02cb1-130">資格情報</span><span class="sxs-lookup"><span data-stu-id="02cb1-130">credentials</span></span>|<span data-ttu-id="02cb1-131">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="02cb1-131">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="02cb1-132">検証する資格情報。</span><span class="sxs-lookup"><span data-stu-id="02cb1-132">Credentials to validate.</span></span> <span data-ttu-id="02cb1-133">無視する場合、`useSavedCredentials`のパラメーターは、 `true`。</span><span class="sxs-lookup"><span data-stu-id="02cb1-133">Ignored when the `useSavedCredentials` parameter is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="02cb1-134">応答</span><span class="sxs-lookup"><span data-stu-id="02cb1-134">Response</span></span>
<span data-ttu-id="02cb1-135">検証は成功を返します、`204, No Content`応答コード。</span><span class="sxs-lookup"><span data-stu-id="02cb1-135">If validation is successful, this method returns a `204, No Content` response code.</span></span> <span data-ttu-id="02cb1-136">応答本体には何もは返されません。</span><span class="sxs-lookup"><span data-stu-id="02cb1-136">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02cb1-137">例</span><span class="sxs-lookup"><span data-stu-id="02cb1-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="02cb1-138">要求</span><span class="sxs-lookup"><span data-stu-id="02cb1-138">Request</span></span>
<span data-ttu-id="02cb1-139">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="02cb1-139">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="02cb1-140">応答</span><span class="sxs-lookup"><span data-stu-id="02cb1-140">Response</span></span>
<span data-ttu-id="02cb1-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="02cb1-141">The following is an example of the response.</span></span> 
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
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-validatecredentials.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
