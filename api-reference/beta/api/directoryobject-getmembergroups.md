---
title: メンバー グループを取得する
description: すべてのグループを返し、指定したユーザー、グループ、サービス主体またはディレクトリ オブジェクトがメンバーであるのです。 この関数は、推移的です。
ms.openlocfilehash: 9dc6af54ba364e1c5c82dc7e14a5d2571e29ef12
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071043"
---
# <a name="get-member-groups"></a><span data-ttu-id="dfefd-104">メンバー グループを取得する</span><span class="sxs-lookup"><span data-stu-id="dfefd-104">Get member groups</span></span>

> <span data-ttu-id="dfefd-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dfefd-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dfefd-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dfefd-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dfefd-107">すべてのグループを返し、指定したユーザー、グループ、サービス主体またはディレクトリ オブジェクトがメンバーであるのです。</span><span class="sxs-lookup"><span data-stu-id="dfefd-107">Return all the groups that the specified user, group, service principal or directory object is a member of.</span></span> <span data-ttu-id="dfefd-108">この関数は、推移的です。</span><span class="sxs-lookup"><span data-stu-id="dfefd-108">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="dfefd-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dfefd-109">Permissions</span></span>
<span data-ttu-id="dfefd-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dfefd-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="dfefd-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dfefd-112">Permission type</span></span>      | <span data-ttu-id="dfefd-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dfefd-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfefd-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dfefd-114">Delegated (work or school account)</span></span> | <span data-ttu-id="dfefd-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfefd-115">Directory.Read.All</span></span>    |
|<span data-ttu-id="dfefd-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dfefd-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfefd-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dfefd-117">Not supported.</span></span>    |
|<span data-ttu-id="dfefd-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dfefd-118">Application</span></span> | <span data-ttu-id="dfefd-119">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfefd-119">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfefd-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dfefd-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /servicePrincipals/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="dfefd-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dfefd-121">Request headers</span></span>
| <span data-ttu-id="dfefd-122">名前</span><span class="sxs-lookup"><span data-stu-id="dfefd-122">Name</span></span>       | <span data-ttu-id="dfefd-123">型</span><span class="sxs-lookup"><span data-stu-id="dfefd-123">Type</span></span> | <span data-ttu-id="dfefd-124">説明</span><span class="sxs-lookup"><span data-stu-id="dfefd-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dfefd-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="dfefd-125">Authorization</span></span>  | <span data-ttu-id="dfefd-126">string</span><span class="sxs-lookup"><span data-stu-id="dfefd-126">string</span></span>  | <span data-ttu-id="dfefd-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="dfefd-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dfefd-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dfefd-129">Content-Type</span></span>  | <span data-ttu-id="dfefd-130">application/json</span><span class="sxs-lookup"><span data-stu-id="dfefd-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dfefd-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="dfefd-131">Request body</span></span>
<span data-ttu-id="dfefd-132">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="dfefd-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dfefd-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="dfefd-133">Parameter</span></span>    | <span data-ttu-id="dfefd-134">型</span><span class="sxs-lookup"><span data-stu-id="dfefd-134">Type</span></span>   |<span data-ttu-id="dfefd-135">説明</span><span class="sxs-lookup"><span data-stu-id="dfefd-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dfefd-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="dfefd-136">securityEnabledOnly</span></span>|<span data-ttu-id="dfefd-137">ブール型</span><span class="sxs-lookup"><span data-stu-id="dfefd-137">Boolean</span></span>| <span data-ttu-id="dfefd-p106">エンティティがメンバーであるセキュリティ グループのみを返すように指定するには **true**、がメンバーであるすべてのグループとディレクトリ ロールを返すように指定するには **false** を設定します。**注**:パラメーターが **true** の場合、関数はユーザーでのみ呼び出せます。</span><span class="sxs-lookup"><span data-stu-id="dfefd-p106">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="dfefd-140">応答</span><span class="sxs-lookup"><span data-stu-id="dfefd-140">Response</span></span>

<span data-ttu-id="dfefd-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dfefd-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfefd-142">例</span><span class="sxs-lookup"><span data-stu-id="dfefd-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dfefd-143">要求</span><span class="sxs-lookup"><span data-stu-id="dfefd-143">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="dfefd-144">応答</span><span class="sxs-lookup"><span data-stu-id="dfefd-144">Response</span></span>
<span data-ttu-id="dfefd-p107">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dfefd-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
