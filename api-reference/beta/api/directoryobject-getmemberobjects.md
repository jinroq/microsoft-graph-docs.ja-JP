---
title: メンバー オブジェクトを取得する
description: " すべてのグループ、管理単位、およびディレクトリの役割のメンバーであるユーザー、グループ、サービス ・ プリンシパルまたはディレクトリ オブジェクトを返します。 この関数は、推移的です。 "
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 00709d0a71b5c13a07d1f07ba41d1273ea0fb034
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946365"
---
# <a name="get-member-objects"></a><span data-ttu-id="b690c-104">メンバー オブジェクトを取得する</span><span class="sxs-lookup"><span data-stu-id="b690c-104">Get member objects</span></span>

> <span data-ttu-id="b690c-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b690c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b690c-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b690c-106">Use of these APIs in production applications is not supported.</span></span>

 <span data-ttu-id="b690c-107">すべてのグループ、管理単位、およびディレクトリの役割のメンバーであるユーザー、グループ、サービス ・ プリンシパルまたはディレクトリ オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b690c-107">Returns all the groups, administrative units and directory roles that a user, group, service principals or directory object is a member of.</span></span> <span data-ttu-id="b690c-108">この関数は、推移的です。</span><span class="sxs-lookup"><span data-stu-id="b690c-108">This function is transitive.</span></span> 
 > <span data-ttu-id="b690c-109">注:ユーザーのみがディレクトリ ロールのメンバーになることができます。</span><span class="sxs-lookup"><span data-stu-id="b690c-109">Note: Only users can be members of directory roles.</span></span>

## <a name="permissions"></a><span data-ttu-id="b690c-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b690c-110">Permissions</span></span>
<span data-ttu-id="b690c-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b690c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b690c-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b690c-113">Permission type</span></span>      | <span data-ttu-id="b690c-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b690c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b690c-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b690c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="b690c-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b690c-116">Directory.Read.All</span></span>    |
|<span data-ttu-id="b690c-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b690c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b690c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b690c-118">Not supported.</span></span>    |
|<span data-ttu-id="b690c-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b690c-119">Application</span></span> | <span data-ttu-id="b690c-120">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b690c-120">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b690c-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b690c-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberObjects
POST /servicePrincipals/{id}/getMemberObjects
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="b690c-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b690c-122">Request headers</span></span>
| <span data-ttu-id="b690c-123">名前</span><span class="sxs-lookup"><span data-stu-id="b690c-123">Name</span></span>       | <span data-ttu-id="b690c-124">種類</span><span class="sxs-lookup"><span data-stu-id="b690c-124">Type</span></span> | <span data-ttu-id="b690c-125">説明</span><span class="sxs-lookup"><span data-stu-id="b690c-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b690c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b690c-126">Authorization</span></span>  | <span data-ttu-id="b690c-127">string</span><span class="sxs-lookup"><span data-stu-id="b690c-127">string</span></span>  | <span data-ttu-id="b690c-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b690c-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b690c-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b690c-130">Content-Type</span></span>  | <span data-ttu-id="b690c-131">application/json</span><span class="sxs-lookup"><span data-stu-id="b690c-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b690c-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="b690c-132">Request body</span></span>
<span data-ttu-id="b690c-133">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="b690c-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b690c-134">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b690c-134">Parameter</span></span>    | <span data-ttu-id="b690c-135">Type</span><span class="sxs-lookup"><span data-stu-id="b690c-135">Type</span></span>   |<span data-ttu-id="b690c-136">説明</span><span class="sxs-lookup"><span data-stu-id="b690c-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b690c-137">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="b690c-137">securityEnabledOnly</span></span>|<span data-ttu-id="b690c-138">ブール型</span><span class="sxs-lookup"><span data-stu-id="b690c-138">Boolean</span></span>| <span data-ttu-id="b690c-p106">エンティティがメンバーであるセキュリティ グループのみを返すように指定するには **true**、がメンバーであるすべてのグループとディレクトリ ロールを返すように指定するには **false** を設定します。**注**:パラメーターが **true** の場合、関数はユーザーでのみ呼び出せます。</span><span class="sxs-lookup"><span data-stu-id="b690c-p106">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="b690c-141">応答</span><span class="sxs-lookup"><span data-stu-id="b690c-141">Response</span></span>

<span data-ttu-id="b690c-142">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b690c-142">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b690c-143">例</span><span class="sxs-lookup"><span data-stu-id="b690c-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b690c-144">要求</span><span class="sxs-lookup"><span data-stu-id="b690c-144">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberObjects
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="b690c-145">応答</span><span class="sxs-lookup"><span data-stu-id="b690c-145">Response</span></span>
<span data-ttu-id="b690c-p107">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b690c-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "c9ee2d50-9e8a-4352-b97c-4c2c99557c22",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
