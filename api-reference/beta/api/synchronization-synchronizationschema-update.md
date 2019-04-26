---
title: 同期スキーマの更新
description: 特定のジョブまたはテンプレートの同期スキーマを更新します。 このメソッドは、現在のスキーマを要求で指定されたものに完全に置き換えます。 テンプレートのスキーマを更新するには、アプリケーションオブジェクトに対して呼び出しを行います。 アプリケーションの所有者である必要があります。
localization_priority: Normal
ms.openlocfilehash: 3c61c39ac6e4b263dd9e5805fbccc1b7bb55d74d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335599"
---
# <a name="update-synchronizationschema"></a><span data-ttu-id="91b17-106">同期スキーマの更新</span><span class="sxs-lookup"><span data-stu-id="91b17-106">Update synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91b17-107">特定のジョブまたはテンプレートの同期スキーマを更新します。</span><span class="sxs-lookup"><span data-stu-id="91b17-107">Update the synchronization schema for a given job or template.</span></span> <span data-ttu-id="91b17-108">このメソッドは、現在のスキーマを要求で指定されたものに完全に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="91b17-108">This method fully replaces the current schema with the one provided in the request.</span></span> <span data-ttu-id="91b17-109">テンプレートのスキーマを更新するには、アプリケーションオブジェクトに対して呼び出しを行います。</span><span class="sxs-lookup"><span data-stu-id="91b17-109">To update the schema of a template, make the call on the application object.</span></span> <span data-ttu-id="91b17-110">アプリケーションの所有者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="91b17-110">You must be the owner of the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="91b17-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="91b17-111">Permissions</span></span>
<span data-ttu-id="91b17-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="91b17-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91b17-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="91b17-114">Permission type</span></span>                        | <span data-ttu-id="91b17-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="91b17-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="91b17-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="91b17-116">Delegated (work or school account)</span></span>     |<span data-ttu-id="91b17-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91b17-117">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="91b17-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="91b17-118">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="91b17-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91b17-119">Not supported.</span></span>|
|<span data-ttu-id="91b17-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="91b17-120">Application</span></span>                            |<span data-ttu-id="91b17-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91b17-121">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="91b17-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="91b17-122">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
PUT /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="91b17-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="91b17-123">Request headers</span></span>

| <span data-ttu-id="91b17-124">名前</span><span class="sxs-lookup"><span data-stu-id="91b17-124">Name</span></span>           | <span data-ttu-id="91b17-125">型</span><span class="sxs-lookup"><span data-stu-id="91b17-125">Type</span></span>    | <span data-ttu-id="91b17-126">説明</span><span class="sxs-lookup"><span data-stu-id="91b17-126">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="91b17-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="91b17-127">Authorization</span></span>  | <span data-ttu-id="91b17-128">string</span><span class="sxs-lookup"><span data-stu-id="91b17-128">string</span></span>  | <span data-ttu-id="91b17-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="91b17-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91b17-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="91b17-131">Request body</span></span>

<span data-ttu-id="91b17-132">要求本文で、既存のスキーマを置換するための[同期スキーマ](../resources/synchronization-synchronizationschema.md)オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="91b17-132">In the request body, supply the [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object to replace the existing schema with.</span></span>

## <a name="response"></a><span data-ttu-id="91b17-133">応答</span><span class="sxs-lookup"><span data-stu-id="91b17-133">Response</span></span>

<span data-ttu-id="91b17-134">成功した場合は`204 No Content` 、応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="91b17-134">If successful, returns a `204 No Content` response code.</span></span> <span data-ttu-id="91b17-135">応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="91b17-135">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91b17-136">例</span><span class="sxs-lookup"><span data-stu-id="91b17-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="91b17-137">要求</span><span class="sxs-lookup"><span data-stu-id="91b17-137">Request</span></span>
<span data-ttu-id="91b17-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="91b17-138">The following is an example of a request.</span></span>

><span data-ttu-id="91b17-139">**注:** ここに示す要求オブジェクトは読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="91b17-139">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="91b17-140">実際の呼び出しですべてのプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="91b17-140">Supply all the properties in an actual call.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_synchronizationschema"
}-->
```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
Content-type: application/json

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

##### <a name="response"></a><span data-ttu-id="91b17-141">応答</span><span class="sxs-lookup"><span data-stu-id="91b17-141">Response</span></span>
<span data-ttu-id="91b17-142">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="91b17-142">The following is an example of a response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update synchronizationschema",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
