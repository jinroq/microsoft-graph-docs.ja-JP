---
title: SynchronizationSchema を更新します。
description: やテンプレートの特定のジョブ、同期スキーマを更新します。 このメソッドは、要求で提供されるもので、現在のスキーマを完全に置き換えます。 テンプレートのスキーマを更新するには、アプリケーション オブジェクトの呼び出しを確認します。 アプリケーションの所有者でなければなりません。
localization_priority: Normal
ms.openlocfilehash: d4f3f3540fe0d304b4edc3a5fcaec7b3366dbb0a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826139"
---
# <a name="update-synchronizationschema"></a><span data-ttu-id="740b2-106">SynchronizationSchema を更新します。</span><span class="sxs-lookup"><span data-stu-id="740b2-106">Update synchronizationSchema</span></span>

> <span data-ttu-id="740b2-107">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="740b2-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="740b2-108">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="740b2-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="740b2-109">やテンプレートの特定のジョブ、同期スキーマを更新します。</span><span class="sxs-lookup"><span data-stu-id="740b2-109">Update the synchronization schema for a given job or template.</span></span> <span data-ttu-id="740b2-110">このメソッドは、要求で提供されるもので、現在のスキーマを完全に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="740b2-110">This method fully replaces the current schema with the one provided in the request.</span></span> <span data-ttu-id="740b2-111">テンプレートのスキーマを更新するには、アプリケーション オブジェクトの呼び出しを確認します。</span><span class="sxs-lookup"><span data-stu-id="740b2-111">To update the schema of a template, make the call on the application object.</span></span> <span data-ttu-id="740b2-112">アプリケーションの所有者でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="740b2-112">You must be the owner of the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="740b2-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="740b2-113">Permissions</span></span>
<span data-ttu-id="740b2-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="740b2-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="740b2-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="740b2-116">Permission type</span></span>                        | <span data-ttu-id="740b2-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="740b2-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="740b2-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="740b2-118">Delegated (work or school account)</span></span>     |<span data-ttu-id="740b2-119">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="740b2-119">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="740b2-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="740b2-120">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="740b2-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="740b2-121">Not supported.</span></span>|
|<span data-ttu-id="740b2-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="740b2-122">Application</span></span>                            |<span data-ttu-id="740b2-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="740b2-123">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="740b2-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="740b2-124">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
PUT /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="740b2-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="740b2-125">Request headers</span></span>

| <span data-ttu-id="740b2-126">名前</span><span class="sxs-lookup"><span data-stu-id="740b2-126">Name</span></span>           | <span data-ttu-id="740b2-127">種類</span><span class="sxs-lookup"><span data-stu-id="740b2-127">Type</span></span>    | <span data-ttu-id="740b2-128">説明</span><span class="sxs-lookup"><span data-stu-id="740b2-128">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="740b2-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="740b2-129">Authorization</span></span>  | <span data-ttu-id="740b2-130">string</span><span class="sxs-lookup"><span data-stu-id="740b2-130">string</span></span>  | <span data-ttu-id="740b2-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="740b2-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="740b2-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="740b2-133">Request body</span></span>

<span data-ttu-id="740b2-134">要求の本体では、既存のスキーマを置換する[synchronizationSchema](../resources/synchronization-synchronizationschema.md)オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="740b2-134">In the request body, supply the [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object to replace the existing schema with.</span></span>

## <a name="response"></a><span data-ttu-id="740b2-135">応答</span><span class="sxs-lookup"><span data-stu-id="740b2-135">Response</span></span>

<span data-ttu-id="740b2-136">正常終了した場合、`204 No Content`応答コード。</span><span class="sxs-lookup"><span data-stu-id="740b2-136">If successful, returns a `204 No Content` response code.</span></span> <span data-ttu-id="740b2-137">応答本体には何もは返されません。</span><span class="sxs-lookup"><span data-stu-id="740b2-137">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="740b2-138">例</span><span class="sxs-lookup"><span data-stu-id="740b2-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="740b2-139">要求</span><span class="sxs-lookup"><span data-stu-id="740b2-139">Request</span></span>
<span data-ttu-id="740b2-140">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="740b2-140">The following is an example of a request.</span></span>

><span data-ttu-id="740b2-141">**注:** ここで示すように、要求オブジェクトは、読みやすさの短縮されます。</span><span class="sxs-lookup"><span data-stu-id="740b2-141">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="740b2-142">実際の呼び出しのすべてのプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="740b2-142">Supply all the properties in an actual call.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_synchronizationschema"
}-->
```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema

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
                },
            ]
        },
        {
            "name": "Salesforce",
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
                    ]
                },
            ]
        },
    ]
}

```

##### <a name="response"></a><span data-ttu-id="740b2-143">応答</span><span class="sxs-lookup"><span data-stu-id="740b2-143">Response</span></span>
<span data-ttu-id="740b2-144">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="740b2-144">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSchema"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update synchronizationschema",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
