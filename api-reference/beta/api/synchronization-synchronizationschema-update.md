---
title: 同期スキーマの更新
description: 特定のジョブまたはテンプレートの同期スキーマを更新します。 このメソッドは、現在のスキーマを要求で指定されたものに完全に置き換えます。 テンプレートのスキーマを更新するには、アプリケーションオブジェクトに対して呼び出しを行います。 アプリケーションの所有者である必要があります。
localization_priority: Normal
ms.openlocfilehash: 13ee7d996b0e02834b77cd222380747c02d7fcc2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536958"
---
# <a name="update-synchronizationschema"></a><span data-ttu-id="cba52-106">同期スキーマの更新</span><span class="sxs-lookup"><span data-stu-id="cba52-106">Update synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cba52-107">特定のジョブまたはテンプレートの同期スキーマを更新します。</span><span class="sxs-lookup"><span data-stu-id="cba52-107">Update the synchronization schema for a given job or template.</span></span> <span data-ttu-id="cba52-108">このメソッドは、現在のスキーマを要求で指定されたものに完全に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="cba52-108">This method fully replaces the current schema with the one provided in the request.</span></span> <span data-ttu-id="cba52-109">テンプレートのスキーマを更新するには、アプリケーションオブジェクトに対して呼び出しを行います。</span><span class="sxs-lookup"><span data-stu-id="cba52-109">To update the schema of a template, make the call on the application object.</span></span> <span data-ttu-id="cba52-110">アプリケーションの所有者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="cba52-110">You must be the owner of the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="cba52-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cba52-111">Permissions</span></span>
<span data-ttu-id="cba52-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cba52-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cba52-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cba52-114">Permission type</span></span>                        | <span data-ttu-id="cba52-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cba52-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="cba52-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cba52-116">Delegated (work or school account)</span></span>     |<span data-ttu-id="cba52-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cba52-117">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="cba52-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cba52-118">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="cba52-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cba52-119">Not supported.</span></span>|
|<span data-ttu-id="cba52-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cba52-120">Application</span></span>                            |<span data-ttu-id="cba52-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cba52-121">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="cba52-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cba52-122">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
PUT /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="cba52-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cba52-123">Request headers</span></span>

| <span data-ttu-id="cba52-124">名前</span><span class="sxs-lookup"><span data-stu-id="cba52-124">Name</span></span>           | <span data-ttu-id="cba52-125">型</span><span class="sxs-lookup"><span data-stu-id="cba52-125">Type</span></span>    | <span data-ttu-id="cba52-126">説明</span><span class="sxs-lookup"><span data-stu-id="cba52-126">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="cba52-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="cba52-127">Authorization</span></span>  | <span data-ttu-id="cba52-128">string</span><span class="sxs-lookup"><span data-stu-id="cba52-128">string</span></span>  | <span data-ttu-id="cba52-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cba52-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cba52-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="cba52-131">Request body</span></span>

<span data-ttu-id="cba52-132">要求本文で、既存のスキーマを置換するための[同期スキーマ](../resources/synchronization-synchronizationschema.md)オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="cba52-132">In the request body, supply the [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object to replace the existing schema with.</span></span>

## <a name="response"></a><span data-ttu-id="cba52-133">応答</span><span class="sxs-lookup"><span data-stu-id="cba52-133">Response</span></span>

<span data-ttu-id="cba52-134">成功した場合は`204 No Content` 、応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="cba52-134">If successful, returns a `204 No Content` response code.</span></span> <span data-ttu-id="cba52-135">応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="cba52-135">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cba52-136">例</span><span class="sxs-lookup"><span data-stu-id="cba52-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cba52-137">要求</span><span class="sxs-lookup"><span data-stu-id="cba52-137">Request</span></span>
<span data-ttu-id="cba52-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cba52-138">The following is an example of a request.</span></span>

><span data-ttu-id="cba52-139">**注:** ここに示す要求オブジェクトは読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="cba52-139">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="cba52-140">実際の呼び出しですべてのプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="cba52-140">Supply all the properties in an actual call.</span></span>
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

##### <a name="response"></a><span data-ttu-id="cba52-141">応答</span><span class="sxs-lookup"><span data-stu-id="cba52-141">Response</span></span>
<span data-ttu-id="cba52-142">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cba52-142">The following is an example of a response.</span></span>
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
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
