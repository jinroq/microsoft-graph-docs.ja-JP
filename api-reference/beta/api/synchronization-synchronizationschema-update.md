---
title: 同期スキーマの更新
description: 特定のジョブまたはテンプレートの同期スキーマを更新します。 このメソッドは、現在のスキーマを要求で指定されたものに完全に置き換えます。 テンプレートのスキーマを更新するには、アプリケーションオブジェクトに対して呼び出しを行います。 アプリケーションの所有者である必要があります。
localization_priority: Normal
ms.openlocfilehash: 0990c1218d93b75e93b20271fc929621ab7e83e2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458186"
---
# <a name="update-synchronizationschema"></a><span data-ttu-id="8c995-106">同期スキーマの更新</span><span class="sxs-lookup"><span data-stu-id="8c995-106">Update synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c995-107">特定のジョブまたはテンプレートの同期スキーマを更新します。</span><span class="sxs-lookup"><span data-stu-id="8c995-107">Update the synchronization schema for a given job or template.</span></span> <span data-ttu-id="8c995-108">このメソッドは、現在のスキーマを要求で指定されたものに完全に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="8c995-108">This method fully replaces the current schema with the one provided in the request.</span></span> <span data-ttu-id="8c995-109">テンプレートのスキーマを更新するには、アプリケーションオブジェクトに対して呼び出しを行います。</span><span class="sxs-lookup"><span data-stu-id="8c995-109">To update the schema of a template, make the call on the application object.</span></span> <span data-ttu-id="8c995-110">アプリケーションの所有者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="8c995-110">You must be the owner of the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c995-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8c995-111">Permissions</span></span>
<span data-ttu-id="8c995-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8c995-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c995-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8c995-114">Permission type</span></span>                        | <span data-ttu-id="8c995-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8c995-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c995-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8c995-116">Delegated (work or school account)</span></span>     |<span data-ttu-id="8c995-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c995-117">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="8c995-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8c995-118">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="8c995-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c995-119">Not supported.</span></span>|
|<span data-ttu-id="8c995-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8c995-120">Application</span></span>                            |<span data-ttu-id="8c995-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c995-121">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="8c995-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8c995-122">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
PUT /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="8c995-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8c995-123">Request headers</span></span>

| <span data-ttu-id="8c995-124">名前</span><span class="sxs-lookup"><span data-stu-id="8c995-124">Name</span></span>           | <span data-ttu-id="8c995-125">型</span><span class="sxs-lookup"><span data-stu-id="8c995-125">Type</span></span>    | <span data-ttu-id="8c995-126">説明</span><span class="sxs-lookup"><span data-stu-id="8c995-126">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="8c995-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c995-127">Authorization</span></span>  | <span data-ttu-id="8c995-128">string</span><span class="sxs-lookup"><span data-stu-id="8c995-128">string</span></span>  | <span data-ttu-id="8c995-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8c995-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c995-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="8c995-131">Request body</span></span>

<span data-ttu-id="8c995-132">要求本文で、既存のスキーマを置換するための[同期スキーマ](../resources/synchronization-synchronizationschema.md)オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="8c995-132">In the request body, supply the [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object to replace the existing schema with.</span></span>

## <a name="response"></a><span data-ttu-id="8c995-133">応答</span><span class="sxs-lookup"><span data-stu-id="8c995-133">Response</span></span>

<span data-ttu-id="8c995-134">成功した場合は`204 No Content` 、応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="8c995-134">If successful, returns a `204 No Content` response code.</span></span> <span data-ttu-id="8c995-135">応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="8c995-135">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c995-136">例</span><span class="sxs-lookup"><span data-stu-id="8c995-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8c995-137">要求</span><span class="sxs-lookup"><span data-stu-id="8c995-137">Request</span></span>
<span data-ttu-id="8c995-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8c995-138">The following is an example of a request.</span></span>

><span data-ttu-id="8c995-139">**注:** ここに示す要求オブジェクトは読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="8c995-139">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="8c995-140">実際の呼び出しですべてのプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="8c995-140">Supply all the properties in an actual call.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8c995-141">プロトコル</span><span class="sxs-lookup"><span data-stu-id="8c995-141">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8c995-142">C#</span><span class="sxs-lookup"><span data-stu-id="8c995-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-synchronizationschema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8c995-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="8c995-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-synchronizationschema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8c995-144">目的-C</span><span class="sxs-lookup"><span data-stu-id="8c995-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-synchronizationschema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8c995-145">応答</span><span class="sxs-lookup"><span data-stu-id="8c995-145">Response</span></span>
<span data-ttu-id="8c995-146">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8c995-146">The following is an example of a response.</span></span>
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
  "suppressions": [
  ]
}
-->
