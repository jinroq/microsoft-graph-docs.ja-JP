---
title: 同期スキーマを取得する
description: 指定された同期ジョブまたはテンプレートのスキーマを取得します。
localization_priority: Normal
ms.openlocfilehash: ed1c937af182afaec75724273c35c7c243d25679
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271275"
---
# <a name="get-synchronizationschema"></a><span data-ttu-id="38656-103">同期スキーマを取得する</span><span class="sxs-lookup"><span data-stu-id="38656-103">Get synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38656-104">指定された同期ジョブまたはテンプレートのスキーマを取得します。</span><span class="sxs-lookup"><span data-stu-id="38656-104">Retrieve the schema for a given synchronization job or template.</span></span>

## <a name="permissions"></a><span data-ttu-id="38656-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="38656-105">Permissions</span></span>
<span data-ttu-id="38656-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="38656-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38656-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="38656-108">Permission type</span></span>                        | <span data-ttu-id="38656-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="38656-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="38656-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="38656-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="38656-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38656-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="38656-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="38656-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="38656-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="38656-113">Not supported.</span></span> |
|<span data-ttu-id="38656-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="38656-114">Application</span></span>                            |<span data-ttu-id="38656-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="38656-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="38656-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="38656-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema
GET /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="38656-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="38656-117">Request headers</span></span>

| <span data-ttu-id="38656-118">名前</span><span class="sxs-lookup"><span data-stu-id="38656-118">Name</span></span>           | <span data-ttu-id="38656-119">型</span><span class="sxs-lookup"><span data-stu-id="38656-119">Type</span></span>    | <span data-ttu-id="38656-120">説明</span><span class="sxs-lookup"><span data-stu-id="38656-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="38656-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="38656-121">Authorization</span></span>  | <span data-ttu-id="38656-122">string</span><span class="sxs-lookup"><span data-stu-id="38656-122">string</span></span>  | <span data-ttu-id="38656-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="38656-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38656-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="38656-125">Request body</span></span>

<span data-ttu-id="38656-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="38656-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38656-127">応答</span><span class="sxs-lookup"><span data-stu-id="38656-127">Response</span></span>

<span data-ttu-id="38656-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[同期スキーマ](../resources/synchronization-synchronizationschema.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="38656-128">If successful, this method returns a `200 OK` response code and a [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38656-129">例</span><span class="sxs-lookup"><span data-stu-id="38656-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="38656-130">要求</span><span class="sxs-lookup"><span data-stu-id="38656-130">Request</span></span>
<span data-ttu-id="38656-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="38656-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a><span data-ttu-id="38656-132">応答</span><span class="sxs-lookup"><span data-stu-id="38656-132">Response</span></span>
<span data-ttu-id="38656-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="38656-133">The following is an example of a response.</span></span>

><span data-ttu-id="38656-134">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="38656-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="38656-135">実際の呼び出しでは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="38656-135">All the properties will be returned in an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="38656-136">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="38656-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="38656-137">C#</span><span class="sxs-lookup"><span data-stu-id="38656-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_synchronizationschema-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="38656-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="38656-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_synchronizationschema-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="38656-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="38656-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_synchronizationschema-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
