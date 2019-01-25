---
title: メンバー グループを取得する
description: すべてのグループを返し、指定したユーザー、グループ、サービス主体またはディレクトリ オブジェクトがメンバーであるのです。 この関数は、推移的です。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9ab73b691ed9cfa4c756e4f0134adf9df7350aae
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526173"
---
# <a name="get-member-groups"></a><span data-ttu-id="58425-104">メンバー グループを取得する</span><span class="sxs-lookup"><span data-stu-id="58425-104">Get member groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58425-105">すべてのグループを返し、指定したユーザー、グループ、サービス主体またはディレクトリ オブジェクトがメンバーであるのです。</span><span class="sxs-lookup"><span data-stu-id="58425-105">Return all the groups that the specified user, group, service principal or directory object is a member of.</span></span> <span data-ttu-id="58425-106">この関数は、推移的です。</span><span class="sxs-lookup"><span data-stu-id="58425-106">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="58425-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="58425-107">Permissions</span></span>
<span data-ttu-id="58425-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="58425-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="58425-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="58425-110">Permission type</span></span>      | <span data-ttu-id="58425-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="58425-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58425-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="58425-112">Delegated (work or school account)</span></span> | <span data-ttu-id="58425-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="58425-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="58425-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="58425-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58425-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58425-115">Not supported.</span></span>    |
|<span data-ttu-id="58425-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="58425-116">Application</span></span> | <span data-ttu-id="58425-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="58425-117">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="58425-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="58425-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /servicePrincipals/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="58425-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="58425-119">Request headers</span></span>
| <span data-ttu-id="58425-120">名前</span><span class="sxs-lookup"><span data-stu-id="58425-120">Name</span></span>       | <span data-ttu-id="58425-121">型</span><span class="sxs-lookup"><span data-stu-id="58425-121">Type</span></span> | <span data-ttu-id="58425-122">説明</span><span class="sxs-lookup"><span data-stu-id="58425-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="58425-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="58425-123">Authorization</span></span>  | <span data-ttu-id="58425-124">string</span><span class="sxs-lookup"><span data-stu-id="58425-124">string</span></span>  | <span data-ttu-id="58425-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="58425-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="58425-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="58425-127">Content-Type</span></span>  | <span data-ttu-id="58425-128">application/json</span><span class="sxs-lookup"><span data-stu-id="58425-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="58425-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="58425-129">Request body</span></span>
<span data-ttu-id="58425-130">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="58425-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="58425-131">パラメーター</span><span class="sxs-lookup"><span data-stu-id="58425-131">Parameter</span></span>    | <span data-ttu-id="58425-132">型</span><span class="sxs-lookup"><span data-stu-id="58425-132">Type</span></span>   |<span data-ttu-id="58425-133">説明</span><span class="sxs-lookup"><span data-stu-id="58425-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58425-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="58425-134">securityEnabledOnly</span></span>|<span data-ttu-id="58425-135">ブール型</span><span class="sxs-lookup"><span data-stu-id="58425-135">Boolean</span></span>| <span data-ttu-id="58425-p105">エンティティがメンバーであるセキュリティ グループのみを返すように指定するには **true**、がメンバーであるすべてのグループとディレクトリ ロールを返すように指定するには **false** を設定します。**注**:パラメーターが **true** の場合、関数はユーザーでのみ呼び出せます。</span><span class="sxs-lookup"><span data-stu-id="58425-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="58425-138">応答</span><span class="sxs-lookup"><span data-stu-id="58425-138">Response</span></span>

<span data-ttu-id="58425-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="58425-139">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58425-140">例</span><span class="sxs-lookup"><span data-stu-id="58425-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="58425-141">要求</span><span class="sxs-lookup"><span data-stu-id="58425-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="58425-142">応答</span><span class="sxs-lookup"><span data-stu-id="58425-142">Response</span></span>
<span data-ttu-id="58425-p106">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="58425-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(Edm.String)",
    "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryobject-getmembergroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
