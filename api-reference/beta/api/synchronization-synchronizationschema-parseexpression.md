---
title: '同期スキーマ: parseexpression'
description: '(../resources/synchronization_attributemappingsource.md) オブジェクト。 '
localization_priority: Normal
ms.openlocfilehash: 27545333c6ff7b3c9ffde3e1c59abd09465db1c2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545368"
---
# <a name="synchronizationschema-parseexpression"></a><span data-ttu-id="98006-103">同期スキーマ: parseexpression</span><span class="sxs-lookup"><span data-stu-id="98006-103">synchronizationSchema: parseExpression</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98006-104">指定した文字列式を解析します [attributeMappingSource | (../resources/synchronization_attributemappingsource.md) オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="98006-104">Parse a given string expression into an [attributeMappingSource|(../resources/synchronization_attributemappingsource.md) object.</span></span> 

<span data-ttu-id="98006-105">式の詳細については、「 [Azure Active Directory での属性マッピングの式の書き込み](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-writing-expressions-for-attribute-mappings)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="98006-105">For more information about expressions, see [Writing Expressions for Attribute Mappings in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-writing-expressions-for-attribute-mappings).</span></span>

## <a name="permissions"></a><span data-ttu-id="98006-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="98006-106">Permissions</span></span>
<span data-ttu-id="98006-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="98006-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98006-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="98006-109">Permission type</span></span>                        | <span data-ttu-id="98006-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="98006-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="98006-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="98006-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="98006-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98006-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="98006-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="98006-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="98006-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="98006-114">Not supported.</span></span>|
|<span data-ttu-id="98006-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="98006-115">Application</span></span>                            |<span data-ttu-id="98006-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="98006-116">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="98006-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="98006-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/schema/parseExpression
POST /servicePrincipals/{id}/synchronization/templates/{id}/schema/parseExpression

```
## <a name="request-headers"></a><span data-ttu-id="98006-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="98006-118">Request headers</span></span>
| <span data-ttu-id="98006-119">名前</span><span class="sxs-lookup"><span data-stu-id="98006-119">Name</span></span>       | <span data-ttu-id="98006-120">説明</span><span class="sxs-lookup"><span data-stu-id="98006-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="98006-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="98006-121">Authorization</span></span>  | <span data-ttu-id="98006-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="98006-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="98006-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="98006-123">Request body</span></span>
<span data-ttu-id="98006-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="98006-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="98006-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="98006-125">Parameter</span></span>    | <span data-ttu-id="98006-126">型</span><span class="sxs-lookup"><span data-stu-id="98006-126">Type</span></span>   |<span data-ttu-id="98006-127">説明</span><span class="sxs-lookup"><span data-stu-id="98006-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98006-128">式</span><span class="sxs-lookup"><span data-stu-id="98006-128">expression</span></span>               |<span data-ttu-id="98006-129">String</span><span class="sxs-lookup"><span data-stu-id="98006-129">String</span></span>               |<span data-ttu-id="98006-130">解析する式を指定します。</span><span class="sxs-lookup"><span data-stu-id="98006-130">Expression to parse.</span></span>|
|<span data-ttu-id="98006-131">testinputobject</span><span class="sxs-lookup"><span data-stu-id="98006-131">testInputObject</span></span>          |[<span data-ttu-id="98006-132">式 inputobject</span><span class="sxs-lookup"><span data-stu-id="98006-132">expressionInputObject</span></span>](../resources/synchronization-expressioninputobject.md)|<span data-ttu-id="98006-133">式を評価するためのテストデータオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="98006-133">Test data object to evaluate expression against.</span></span> <span data-ttu-id="98006-134">省略可能。</span><span class="sxs-lookup"><span data-stu-id="98006-134">Optional.</span></span>|
|<span data-ttu-id="98006-135">targetattributedefinition</span><span class="sxs-lookup"><span data-stu-id="98006-135">targetAttributeDefinition</span></span>|[<span data-ttu-id="98006-136">attributedefinition</span><span class="sxs-lookup"><span data-stu-id="98006-136">attributeDefinition</span></span>](../resources/synchronization-attributedefinition.md) |<span data-ttu-id="98006-137">この式にマップされる属性の定義。</span><span class="sxs-lookup"><span data-stu-id="98006-137">Definition of the attribute that will be mapped to this expression.</span></span> <span data-ttu-id="98006-138">省略可能。</span><span class="sxs-lookup"><span data-stu-id="98006-138">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="98006-139">応答</span><span class="sxs-lookup"><span data-stu-id="98006-139">Response</span></span>
<span data-ttu-id="98006-140">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[parseexpression response](../resources/synchronization-parseexpressionresponse.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="98006-140">If successful, this method returns a `200 OK` response code and a [parseExpressionResponse](../resources/synchronization-parseexpressionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98006-141">例</span><span class="sxs-lookup"><span data-stu-id="98006-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="98006-142">要求</span><span class="sxs-lookup"><span data-stu-id="98006-142">Request</span></span>
<span data-ttu-id="98006-143">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="98006-143">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="98006-144">応答</span><span class="sxs-lookup"><span data-stu-id="98006-144">Response</span></span>
<span data-ttu-id="98006-145">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="98006-145">The following is an example of the response.</span></span> 

><span data-ttu-id="98006-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="98006-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-parseexpression.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
