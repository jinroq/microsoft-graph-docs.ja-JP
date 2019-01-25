---
title: SynchronizationSchema を取得します。
description: 指定された同期ジョブまたはテンプレートのスキーマを取得します。
localization_priority: Normal
ms.openlocfilehash: 050357c94997ca7a45d9ca09bf164638072d1354
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512494"
---
# <a name="get-synchronizationschema"></a><span data-ttu-id="7dd6f-103">SynchronizationSchema を取得します。</span><span class="sxs-lookup"><span data-stu-id="7dd6f-103">Get synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7dd6f-104">指定された同期ジョブまたはテンプレートのスキーマを取得します。</span><span class="sxs-lookup"><span data-stu-id="7dd6f-104">Retrieve the schema for a given synchronization job or template.</span></span>

## <a name="permissions"></a><span data-ttu-id="7dd6f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7dd6f-105">Permissions</span></span>
<span data-ttu-id="7dd6f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7dd6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dd6f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7dd6f-108">Permission type</span></span>                        | <span data-ttu-id="7dd6f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7dd6f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7dd6f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7dd6f-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="7dd6f-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dd6f-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="7dd6f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7dd6f-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="7dd6f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7dd6f-113">Not supported.</span></span> |
|<span data-ttu-id="7dd6f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7dd6f-114">Application</span></span>                            |<span data-ttu-id="7dd6f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7dd6f-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7dd6f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7dd6f-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema
GET /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="7dd6f-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7dd6f-117">Request headers</span></span>

| <span data-ttu-id="7dd6f-118">名前</span><span class="sxs-lookup"><span data-stu-id="7dd6f-118">Name</span></span>           | <span data-ttu-id="7dd6f-119">型</span><span class="sxs-lookup"><span data-stu-id="7dd6f-119">Type</span></span>    | <span data-ttu-id="7dd6f-120">説明</span><span class="sxs-lookup"><span data-stu-id="7dd6f-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="7dd6f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7dd6f-121">Authorization</span></span>  | <span data-ttu-id="7dd6f-122">string</span><span class="sxs-lookup"><span data-stu-id="7dd6f-122">string</span></span>  | <span data-ttu-id="7dd6f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7dd6f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7dd6f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="7dd6f-125">Request body</span></span>

<span data-ttu-id="7dd6f-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7dd6f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7dd6f-127">応答</span><span class="sxs-lookup"><span data-stu-id="7dd6f-127">Response</span></span>

<span data-ttu-id="7dd6f-128">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[synchronizationSchema](../resources/synchronization-synchronizationschema.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="7dd6f-128">If successful, this method returns a `200 OK` response code and a [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7dd6f-129">例</span><span class="sxs-lookup"><span data-stu-id="7dd6f-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7dd6f-130">要求</span><span class="sxs-lookup"><span data-stu-id="7dd6f-130">Request</span></span>
<span data-ttu-id="7dd6f-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7dd6f-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a><span data-ttu-id="7dd6f-132">応答</span><span class="sxs-lookup"><span data-stu-id="7dd6f-132">Response</span></span>
<span data-ttu-id="7dd6f-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7dd6f-133">The following is an example of a response.</span></span>

><span data-ttu-id="7dd6f-134">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="7dd6f-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7dd6f-135">すべてのプロパティは、実際の呼び出しで返されます。</span><span class="sxs-lookup"><span data-stu-id="7dd6f-135">All the properties will be returned in an actual call.</span></span>
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
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
