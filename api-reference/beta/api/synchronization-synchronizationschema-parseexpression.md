---
title: '同期スキーマ: parseExpression'
description: '(../resources/synchronization_attributemappingsource.md) オブジェクト。 '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 24e223be3dc5ffbe50aed30ffabcf8959bdbaa6c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869142"
---
# <a name="synchronizationschema-parseexpression"></a><span data-ttu-id="7f673-103">同期スキーマ: parseExpression</span><span class="sxs-lookup"><span data-stu-id="7f673-103">synchronizationSchema: parseExpression</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f673-104">指定した文字列式を解析します [attributeMappingSource | (../resources/synchronization_attributemappingsource.md) オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="7f673-104">Parse a given string expression into an [attributeMappingSource|(../resources/synchronization_attributemappingsource.md) object.</span></span> 

<span data-ttu-id="7f673-105">式の詳細については、「 [Azure Active Directory での属性マッピングの式の書き込み](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-writing-expressions-for-attribute-mappings)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f673-105">For more information about expressions, see [Writing Expressions for Attribute Mappings in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-writing-expressions-for-attribute-mappings).</span></span>

## <a name="permissions"></a><span data-ttu-id="7f673-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7f673-106">Permissions</span></span>
<span data-ttu-id="7f673-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f673-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f673-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7f673-109">Permission type</span></span>                        | <span data-ttu-id="7f673-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7f673-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f673-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7f673-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="7f673-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f673-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="7f673-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7f673-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="7f673-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f673-114">Not supported.</span></span>|
|<span data-ttu-id="7f673-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7f673-115">Application</span></span>                            |<span data-ttu-id="7f673-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f673-116">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="7f673-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7f673-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/schema/parseExpression
POST /servicePrincipals/{id}/synchronization/templates/{id}/schema/parseExpression

```
## <a name="request-headers"></a><span data-ttu-id="7f673-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f673-118">Request headers</span></span>
| <span data-ttu-id="7f673-119">名前</span><span class="sxs-lookup"><span data-stu-id="7f673-119">Name</span></span>       | <span data-ttu-id="7f673-120">説明</span><span class="sxs-lookup"><span data-stu-id="7f673-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7f673-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f673-121">Authorization</span></span>  | <span data-ttu-id="7f673-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="7f673-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f673-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="7f673-123">Request body</span></span>
<span data-ttu-id="7f673-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="7f673-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7f673-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="7f673-125">Parameter</span></span>    | <span data-ttu-id="7f673-126">型</span><span class="sxs-lookup"><span data-stu-id="7f673-126">Type</span></span>   |<span data-ttu-id="7f673-127">説明</span><span class="sxs-lookup"><span data-stu-id="7f673-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f673-128">式</span><span class="sxs-lookup"><span data-stu-id="7f673-128">expression</span></span>               |<span data-ttu-id="7f673-129">String</span><span class="sxs-lookup"><span data-stu-id="7f673-129">String</span></span>               |<span data-ttu-id="7f673-130">解析する式を指定します。</span><span class="sxs-lookup"><span data-stu-id="7f673-130">Expression to parse.</span></span>|
|<span data-ttu-id="7f673-131">testInputObject</span><span class="sxs-lookup"><span data-stu-id="7f673-131">testInputObject</span></span>          |[<span data-ttu-id="7f673-132">式 Inputobject</span><span class="sxs-lookup"><span data-stu-id="7f673-132">expressionInputObject</span></span>](../resources/synchronization-expressioninputobject.md)|<span data-ttu-id="7f673-133">式を評価するためのテストデータオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="7f673-133">Test data object to evaluate expression against.</span></span> <span data-ttu-id="7f673-134">省略可能。</span><span class="sxs-lookup"><span data-stu-id="7f673-134">Optional.</span></span>|
|<span data-ttu-id="7f673-135">targetAttributeDefinition</span><span class="sxs-lookup"><span data-stu-id="7f673-135">targetAttributeDefinition</span></span>|[<span data-ttu-id="7f673-136">attributeDefinition</span><span class="sxs-lookup"><span data-stu-id="7f673-136">attributeDefinition</span></span>](../resources/synchronization-attributedefinition.md) |<span data-ttu-id="7f673-137">この式にマップされる属性の定義。</span><span class="sxs-lookup"><span data-stu-id="7f673-137">Definition of the attribute that will be mapped to this expression.</span></span> <span data-ttu-id="7f673-138">省略可能。</span><span class="sxs-lookup"><span data-stu-id="7f673-138">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="7f673-139">応答</span><span class="sxs-lookup"><span data-stu-id="7f673-139">Response</span></span>
<span data-ttu-id="7f673-140">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[parseexpression response](../resources/synchronization-parseexpressionresponse.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7f673-140">If successful, this method returns a `200 OK` response code and a [parseExpressionResponse](../resources/synchronization-parseexpressionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f673-141">例</span><span class="sxs-lookup"><span data-stu-id="7f673-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7f673-142">要求</span><span class="sxs-lookup"><span data-stu-id="7f673-142">Request</span></span>
<span data-ttu-id="7f673-143">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7f673-143">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7f673-144">プロトコル</span><span class="sxs-lookup"><span data-stu-id="7f673-144">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="7f673-145">C#</span><span class="sxs-lookup"><span data-stu-id="7f673-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationschema-parseexpression-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7f673-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="7f673-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationschema-parseexpression-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7f673-147">目的-C</span><span class="sxs-lookup"><span data-stu-id="7f673-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationschema-parseexpression-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7f673-148">Java</span><span class="sxs-lookup"><span data-stu-id="7f673-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationschema-parseexpression-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7f673-149">応答</span><span class="sxs-lookup"><span data-stu-id="7f673-149">Response</span></span>
<span data-ttu-id="7f673-150">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7f673-150">The following is an example of the response.</span></span> 

><span data-ttu-id="7f673-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7f673-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSchema: parseExpression",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
