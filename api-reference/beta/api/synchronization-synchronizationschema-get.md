---
title: 同期スキーマを取得する
description: 指定された同期ジョブまたはテンプレートのスキーマを取得します。
localization_priority: Normal
ms.openlocfilehash: 3b834d955a79c45ef5ae1e43ec9ca0f1fd18cedd
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637963"
---
# <a name="get-synchronizationschema"></a><span data-ttu-id="4ae36-103">同期スキーマを取得する</span><span class="sxs-lookup"><span data-stu-id="4ae36-103">Get synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ae36-104">指定された同期ジョブまたはテンプレートのスキーマを取得します。</span><span class="sxs-lookup"><span data-stu-id="4ae36-104">Retrieve the schema for a given synchronization job or template.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ae36-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4ae36-105">Permissions</span></span>
<span data-ttu-id="4ae36-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4ae36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ae36-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4ae36-108">Permission type</span></span>                        | <span data-ttu-id="4ae36-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4ae36-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ae36-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4ae36-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="4ae36-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ae36-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="4ae36-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4ae36-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="4ae36-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4ae36-113">Not supported.</span></span> |
|<span data-ttu-id="4ae36-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4ae36-114">Application</span></span>                            |<span data-ttu-id="4ae36-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4ae36-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4ae36-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4ae36-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema
GET /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="4ae36-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4ae36-117">Request headers</span></span>

| <span data-ttu-id="4ae36-118">名前</span><span class="sxs-lookup"><span data-stu-id="4ae36-118">Name</span></span>           | <span data-ttu-id="4ae36-119">型</span><span class="sxs-lookup"><span data-stu-id="4ae36-119">Type</span></span>    | <span data-ttu-id="4ae36-120">説明</span><span class="sxs-lookup"><span data-stu-id="4ae36-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="4ae36-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ae36-121">Authorization</span></span>  | <span data-ttu-id="4ae36-122">string</span><span class="sxs-lookup"><span data-stu-id="4ae36-122">string</span></span>  | <span data-ttu-id="4ae36-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4ae36-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ae36-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="4ae36-125">Request body</span></span>

<span data-ttu-id="4ae36-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4ae36-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ae36-127">応答</span><span class="sxs-lookup"><span data-stu-id="4ae36-127">Response</span></span>

<span data-ttu-id="4ae36-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[同期スキーマ](../resources/synchronization-synchronizationschema.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4ae36-128">If successful, this method returns a `200 OK` response code and a [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ae36-129">例</span><span class="sxs-lookup"><span data-stu-id="4ae36-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4ae36-130">要求</span><span class="sxs-lookup"><span data-stu-id="4ae36-130">Request</span></span>
<span data-ttu-id="4ae36-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4ae36-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a><span data-ttu-id="4ae36-132">応答</span><span class="sxs-lookup"><span data-stu-id="4ae36-132">Response</span></span>
<span data-ttu-id="4ae36-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4ae36-133">The following is an example of a response.</span></span>

><span data-ttu-id="4ae36-134">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="4ae36-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4ae36-135">実際の呼び出しでは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4ae36-135">All the properties will be returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSchema"
} -->
```http
HTTP/1.1 200 OK

{
    "directories": [
        {
            "name": "Azure Active Directory",
            "objects": [
                {
                    "name": "User",
                    "attributes": [
                        {
                            "name": "userPrincipalName",
                            "type": "string"
                        }
                    ]
                }
            ]
        },
        {
            "name": "Salesforce",
            "objects": [{}]
        }
    ],
    "synchronizationRules":[
        {
            "name": "USER_TO_USER",
            "sourceDirectoryName": "Azure Active Directory",
            "targetDirectoryName": "Salesforce",
            "objectMappings": [
                {
                    "sourceObjectName": "User",
                    "targetObjectName": "User",
                    "attributeMappings": [
                        {
                            "source": {},
                            "targetAttributeName": "userName"
                        },
                        {}
                    ]
                },
                {}
            ]
        },
        {}
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4ae36-136">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="4ae36-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4ae36-137">Visual</span><span class="sxs-lookup"><span data-stu-id="4ae36-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_synchronizationschema-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4ae36-138">Java</span><span class="sxs-lookup"><span data-stu-id="4ae36-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_synchronizationschema-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get synchronizationSchema",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
