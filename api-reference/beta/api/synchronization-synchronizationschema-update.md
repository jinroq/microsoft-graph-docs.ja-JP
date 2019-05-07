---
title: 同期スキーマの更新
description: 特定のジョブまたはテンプレートの同期スキーマを更新します。 このメソッドは、現在のスキーマを要求で指定されたものに完全に置き換えます。 テンプレートのスキーマを更新するには、アプリケーションオブジェクトに対して呼び出しを行います。 アプリケーションの所有者である必要があります。
localization_priority: Normal
ms.openlocfilehash: 114b55c135fe81e214da71047f681f26c72aa55b
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637935"
---
# <a name="update-synchronizationschema"></a><span data-ttu-id="636c1-106">同期スキーマの更新</span><span class="sxs-lookup"><span data-stu-id="636c1-106">Update synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="636c1-107">特定のジョブまたはテンプレートの同期スキーマを更新します。</span><span class="sxs-lookup"><span data-stu-id="636c1-107">Update the synchronization schema for a given job or template.</span></span> <span data-ttu-id="636c1-108">このメソッドは、現在のスキーマを要求で指定されたものに完全に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="636c1-108">This method fully replaces the current schema with the one provided in the request.</span></span> <span data-ttu-id="636c1-109">テンプレートのスキーマを更新するには、アプリケーションオブジェクトに対して呼び出しを行います。</span><span class="sxs-lookup"><span data-stu-id="636c1-109">To update the schema of a template, make the call on the application object.</span></span> <span data-ttu-id="636c1-110">アプリケーションの所有者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="636c1-110">You must be the owner of the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="636c1-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="636c1-111">Permissions</span></span>
<span data-ttu-id="636c1-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="636c1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="636c1-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="636c1-114">Permission type</span></span>                        | <span data-ttu-id="636c1-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="636c1-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="636c1-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="636c1-116">Delegated (work or school account)</span></span>     |<span data-ttu-id="636c1-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="636c1-117">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="636c1-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="636c1-118">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="636c1-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="636c1-119">Not supported.</span></span>|
|<span data-ttu-id="636c1-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="636c1-120">Application</span></span>                            |<span data-ttu-id="636c1-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="636c1-121">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="636c1-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="636c1-122">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
PUT /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="636c1-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="636c1-123">Request headers</span></span>

| <span data-ttu-id="636c1-124">名前</span><span class="sxs-lookup"><span data-stu-id="636c1-124">Name</span></span>           | <span data-ttu-id="636c1-125">型</span><span class="sxs-lookup"><span data-stu-id="636c1-125">Type</span></span>    | <span data-ttu-id="636c1-126">説明</span><span class="sxs-lookup"><span data-stu-id="636c1-126">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="636c1-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="636c1-127">Authorization</span></span>  | <span data-ttu-id="636c1-128">string</span><span class="sxs-lookup"><span data-stu-id="636c1-128">string</span></span>  | <span data-ttu-id="636c1-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="636c1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="636c1-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="636c1-131">Request body</span></span>

<span data-ttu-id="636c1-132">要求本文で、既存のスキーマを置換するための[同期スキーマ](../resources/synchronization-synchronizationschema.md)オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="636c1-132">In the request body, supply the [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object to replace the existing schema with.</span></span>

## <a name="response"></a><span data-ttu-id="636c1-133">応答</span><span class="sxs-lookup"><span data-stu-id="636c1-133">Response</span></span>

<span data-ttu-id="636c1-134">成功した場合は`204 No Content` 、応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="636c1-134">If successful, returns a `204 No Content` response code.</span></span> <span data-ttu-id="636c1-135">応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="636c1-135">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="636c1-136">例</span><span class="sxs-lookup"><span data-stu-id="636c1-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="636c1-137">要求</span><span class="sxs-lookup"><span data-stu-id="636c1-137">Request</span></span>
<span data-ttu-id="636c1-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="636c1-138">The following is an example of a request.</span></span>

><span data-ttu-id="636c1-139">**注:** ここに示す要求オブジェクトは読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="636c1-139">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="636c1-140">実際の呼び出しですべてのプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="636c1-140">Supply all the properties in an actual call.</span></span>
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

##### <a name="response"></a><span data-ttu-id="636c1-141">応答</span><span class="sxs-lookup"><span data-stu-id="636c1-141">Response</span></span>
<span data-ttu-id="636c1-142">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="636c1-142">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSchema"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="636c1-143">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="636c1-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="636c1-144">Visual</span><span class="sxs-lookup"><span data-stu-id="636c1-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_synchronizationschema-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="636c1-145">Java</span><span class="sxs-lookup"><span data-stu-id="636c1-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_synchronizationschema-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
