---
title: SynchronizationSchema を取得します。
description: 指定された同期ジョブまたはテンプレートのスキーマを取得します。
localization_priority: Normal
ms.openlocfilehash: 768a35940593231bbc4fbd4c3f5498c7eb3243fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863470"
---
# <a name="get-synchronizationschema"></a><span data-ttu-id="e1d3a-103">SynchronizationSchema を取得します。</span><span class="sxs-lookup"><span data-stu-id="e1d3a-103">Get synchronizationSchema</span></span>

> <span data-ttu-id="e1d3a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e1d3a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1d3a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1d3a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e1d3a-106">指定された同期ジョブまたはテンプレートのスキーマを取得します。</span><span class="sxs-lookup"><span data-stu-id="e1d3a-106">Retrieve the schema for a given synchronization job or template.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1d3a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e1d3a-107">Permissions</span></span>
<span data-ttu-id="e1d3a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e1d3a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1d3a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e1d3a-110">Permission type</span></span>                        | <span data-ttu-id="e1d3a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e1d3a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1d3a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e1d3a-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="e1d3a-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1d3a-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="e1d3a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e1d3a-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="e1d3a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1d3a-115">Not supported.</span></span> |
|<span data-ttu-id="e1d3a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e1d3a-116">Application</span></span>                            |<span data-ttu-id="e1d3a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1d3a-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e1d3a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e1d3a-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema
GET /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="e1d3a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e1d3a-119">Request headers</span></span>

| <span data-ttu-id="e1d3a-120">名前</span><span class="sxs-lookup"><span data-stu-id="e1d3a-120">Name</span></span>           | <span data-ttu-id="e1d3a-121">種類</span><span class="sxs-lookup"><span data-stu-id="e1d3a-121">Type</span></span>    | <span data-ttu-id="e1d3a-122">説明</span><span class="sxs-lookup"><span data-stu-id="e1d3a-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="e1d3a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1d3a-123">Authorization</span></span>  | <span data-ttu-id="e1d3a-124">string</span><span class="sxs-lookup"><span data-stu-id="e1d3a-124">string</span></span>  | <span data-ttu-id="e1d3a-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e1d3a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1d3a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e1d3a-127">Request body</span></span>

<span data-ttu-id="e1d3a-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e1d3a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1d3a-129">応答</span><span class="sxs-lookup"><span data-stu-id="e1d3a-129">Response</span></span>

<span data-ttu-id="e1d3a-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[synchronizationSchema](../resources/synchronization-synchronizationschema.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="e1d3a-130">If successful, this method returns a `200 OK` response code and a [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1d3a-131">例</span><span class="sxs-lookup"><span data-stu-id="e1d3a-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e1d3a-132">要求</span><span class="sxs-lookup"><span data-stu-id="e1d3a-132">Request</span></span>
<span data-ttu-id="e1d3a-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e1d3a-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a><span data-ttu-id="e1d3a-134">応答</span><span class="sxs-lookup"><span data-stu-id="e1d3a-134">Response</span></span>
<span data-ttu-id="e1d3a-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e1d3a-135">The following is an example of a response.</span></span>

><span data-ttu-id="e1d3a-136">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="e1d3a-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e1d3a-137">すべてのプロパティは、実際の呼び出しで返されます。</span><span class="sxs-lookup"><span data-stu-id="e1d3a-137">All the properties will be returned in an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get synchronizationSchema",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
