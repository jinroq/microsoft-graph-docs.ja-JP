---
title: 'synchronizationSchema: parseExpression'
description: '(../resources/synchronization_attributemappingsource.md) オブジェクト。 '
localization_priority: Normal
ms.openlocfilehash: dbde03b9ae85377801ad894c8b8ca22c6baebc85
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811026"
---
# <a name="synchronizationschema-parseexpression"></a><span data-ttu-id="8ee60-103">synchronizationSchema: parseExpression</span><span class="sxs-lookup"><span data-stu-id="8ee60-103">synchronizationSchema: parseExpression</span></span>

> <span data-ttu-id="8ee60-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8ee60-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ee60-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ee60-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8ee60-106">指定された文字列式を解析する [attributeMappingSource | (../resources/synchronization_attributemappingsource.md) オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="8ee60-106">Parse a given string expression into an [attributeMappingSource|(../resources/synchronization_attributemappingsource.md) object.</span></span> 

<span data-ttu-id="8ee60-107">式の詳細については、 [Azure Active Directory 内の属性のマッピングの式の記述](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-writing-expressions-for-attribute-mappings)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8ee60-107">For more information about expressions, see [Writing Expressions for Attribute Mappings in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-writing-expressions-for-attribute-mappings).</span></span>

## <a name="permissions"></a><span data-ttu-id="8ee60-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8ee60-108">Permissions</span></span>
<span data-ttu-id="8ee60-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8ee60-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ee60-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8ee60-111">Permission type</span></span>                        | <span data-ttu-id="8ee60-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8ee60-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ee60-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8ee60-113">Delegated (work or school account)</span></span>     |<span data-ttu-id="8ee60-114">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ee60-114">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="8ee60-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8ee60-115">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="8ee60-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ee60-116">Not supported.</span></span>|
|<span data-ttu-id="8ee60-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8ee60-117">Application</span></span>                            |<span data-ttu-id="8ee60-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ee60-118">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="8ee60-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8ee60-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/schema/parseExpression
POST /servicePrincipals/{id}/synchronization/templates/{id}/schema/parseExpression

```
## <a name="request-headers"></a><span data-ttu-id="8ee60-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8ee60-120">Request headers</span></span>
| <span data-ttu-id="8ee60-121">名前</span><span class="sxs-lookup"><span data-stu-id="8ee60-121">Name</span></span>       | <span data-ttu-id="8ee60-122">説明</span><span class="sxs-lookup"><span data-stu-id="8ee60-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8ee60-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ee60-123">Authorization</span></span>  | <span data-ttu-id="8ee60-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8ee60-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ee60-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="8ee60-125">Request body</span></span>
<span data-ttu-id="8ee60-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="8ee60-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8ee60-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="8ee60-127">Parameter</span></span>    | <span data-ttu-id="8ee60-128">Type</span><span class="sxs-lookup"><span data-stu-id="8ee60-128">Type</span></span>   |<span data-ttu-id="8ee60-129">説明</span><span class="sxs-lookup"><span data-stu-id="8ee60-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ee60-130">式</span><span class="sxs-lookup"><span data-stu-id="8ee60-130">expression</span></span>               |<span data-ttu-id="8ee60-131">String</span><span class="sxs-lookup"><span data-stu-id="8ee60-131">String</span></span>               |<span data-ttu-id="8ee60-132">解析する式を指定します。</span><span class="sxs-lookup"><span data-stu-id="8ee60-132">Expression to parse.</span></span>|
|<span data-ttu-id="8ee60-133">testInputObject</span><span class="sxs-lookup"><span data-stu-id="8ee60-133">testInputObject</span></span>          |[<span data-ttu-id="8ee60-134">expressionInputObject</span><span class="sxs-lookup"><span data-stu-id="8ee60-134">expressionInputObject</span></span>](../resources/synchronization-expressioninputobject.md)|<span data-ttu-id="8ee60-135">に対して式を評価するためにデータ オブジェクトをテストします。</span><span class="sxs-lookup"><span data-stu-id="8ee60-135">Test data object to evaluate expression against.</span></span> <span data-ttu-id="8ee60-136">省略可能。</span><span class="sxs-lookup"><span data-stu-id="8ee60-136">Optional.</span></span>|
|<span data-ttu-id="8ee60-137">targetAttributeDefinition</span><span class="sxs-lookup"><span data-stu-id="8ee60-137">targetAttributeDefinition</span></span>|[<span data-ttu-id="8ee60-138">attributeDefinition</span><span class="sxs-lookup"><span data-stu-id="8ee60-138">attributeDefinition</span></span>](../resources/synchronization-attributedefinition.md) |<span data-ttu-id="8ee60-139">この式にマップされる属性の定義。</span><span class="sxs-lookup"><span data-stu-id="8ee60-139">Definition of the attribute that will be mapped to this expression.</span></span> <span data-ttu-id="8ee60-140">省略可能。</span><span class="sxs-lookup"><span data-stu-id="8ee60-140">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="8ee60-141">応答</span><span class="sxs-lookup"><span data-stu-id="8ee60-141">Response</span></span>
<span data-ttu-id="8ee60-142">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[parseExpressionResponse](../resources/synchronization-parseexpressionresponse.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="8ee60-142">If successful, this method returns a `200 OK` response code and a [parseExpressionResponse](../resources/synchronization-parseexpressionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ee60-143">例</span><span class="sxs-lookup"><span data-stu-id="8ee60-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8ee60-144">要求</span><span class="sxs-lookup"><span data-stu-id="8ee60-144">Request</span></span>
<span data-ttu-id="8ee60-145">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8ee60-145">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_parseexpression"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{id}/schema/parseExpression
Content-type: application/json

{
    "expression":"Replace([preferredLanguage], \"-\", , , \"_\", ,  )",
    "targetAttributeDefinition":null,
    "testInputObject": {
        definition: null,
        properties:[
            { key: "objectId", value : "66E4A8CC-1B7B-435E-95F8-F06CEA133828" },
            { key: "IsSoftDeleted", value: "false"},
            { key: "accountEnabled", value: "true"},
            { key: "streetAddress", value: "1 Redmond Way"},
            { key: "city", value: "Redmond"},
            { key: "state", value: "WA"},
            { key: "postalCode", value: "98052"},
            { key: "country", value: "USA"},
            { key: "department", value: "Sales"},
            { key: "displayName", value: "John Smith"},
            { key: "extensionAttribute1", value: "Sample 1"},
            { key: "extensionAttribute2", value: "Sample 2"},
            { key: "extensionAttribute3", value: "Sample 3"},
            { key: "extensionAttribute4", value: "Sample 4"},
            { key: "extensionAttribute5", value: "Sample 5"},
            { key: "extensionAttribute6", value: "Sample 6"},
            { key: "extensionAttribute7", value: "Sample 1"},
            { key: "extensionAttribute8", value: "Sample 1"},
            { key: "extensionAttribute9", value: "Sample 1"},
            { key: "extensionAttribute10", value: "Sample 1"},
            { key: "extensionAttribute11", value: "Sample 1"},
            { key: "extensionAttribute12", value: "Sample 1"},
            { key: "extensionAttribute13", value: "Sample 1"},
            { key: "extensionAttribute14", value: "Sample 1"},
            { key: "extensionAttribute15", value: "Sample 1"},
            { key: "givenName", value: "John"},
            { key: "jobTitle", value: "Finance manager"},
            { key: "mail", value: "johns@contoso.com"},
            { key: "mailNickname", value: "johns"},
            { key: "manager", value: "maxs@contoso.com"},
            { key: "mobile", value: "425-555-0010"},
            { key: "onPremisesSecurityIdentifier", value: "66E4A8CC-1B7B-435E-95F8-F06CEA133828"},
            { key: "passwordProfile.password", value: ""},
            { key: "physicalDeliveryOfficeName", value: "Main Office"},
            { key: "preferredLanguage", value: "EN-US"},
            { key: "proxyAddresses", value: ""},
            { key: "surname", value: "Smith"},
            { key: "telephoneNumber", value: "425-555-0011"},
            { key: "userPrincipalName", value: "johns@contoso.com"},
            { key: "appRoleAssignments", "value@odata.type":"#Collection(String)", value: ["Default Assignment"] }
        ]
    }
}
```

##### <a name="response"></a><span data-ttu-id="8ee60-146">応答</span><span class="sxs-lookup"><span data-stu-id="8ee60-146">Response</span></span>
<span data-ttu-id="8ee60-147">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8ee60-147">The following is an example of the response.</span></span> 

><span data-ttu-id="8ee60-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8ee60-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.parseExpressionResponse"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "error": null,
    "evaluationSucceeded": true,
    "evaluationResult": [
        "EN_US"
    ],
    "parsedExpression": {
        "expression": "Replace([preferredLanguage], \"-\", , , \"_\", , )",
        "name": "Replace",
        "parameters": [
            {
                "key": "source",
                "value": {
                    "expression": "[preferredLanguage]",
                    "name": "preferredLanguage",
                    "parameters": [],
                    "type": "Attribute"
                }
            },
            {
                "key": "Find",
                "value": {
                    "expression": "\"-\"",
                    "name": "-",
                    "parameters": [],
                    "type": "Constant"
                }
            },
            {
                "key": "Replacement",
                "value": {
                    "expression": "\"_\"",
                    "name": "_",
                    "parameters": [],
                    "type": "Constant"
                }
            }
        ],
        "type": "Function"
    },
    "parsingSucceeded": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSchema: parseExpression",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
