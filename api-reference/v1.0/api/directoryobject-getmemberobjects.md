---
title: メンバー オブジェクトを取得する
description: " ユーザー、グループ、またはディレクトリ オブジェクトがメンバーであるすべてのグループとディレクトリ ロールを返します。この関数は、推移的です。 "
ms.openlocfilehash: b9e0cd4221f4016ccc98302d194ceef8b1622707
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022445"
---
# <a name="get-member-objects"></a><span data-ttu-id="d8ced-104">メンバー オブジェクトを取得する</span><span class="sxs-lookup"><span data-stu-id="d8ced-104">Get member objects</span></span>

 <span data-ttu-id="d8ced-p102">ユーザー、グループ、またはディレクトリ オブジェクトがメンバーであるすべてのグループとディレクトリ ロールを返します。この関数は、推移的です。</span><span class="sxs-lookup"><span data-stu-id="d8ced-p102">Returns all the groups and directory roles that a user, group, or directory object is a member of. This function is transitive.</span></span> 
 > <span data-ttu-id="d8ced-107">注:ユーザーのみがディレクトリ ロールのメンバーになることができます。</span><span class="sxs-lookup"><span data-stu-id="d8ced-107">Note: Only users can be members of directory roles.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8ced-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d8ced-108">Permissions</span></span>
<span data-ttu-id="d8ced-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d8ced-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8ced-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d8ced-111">Permission type</span></span>      | <span data-ttu-id="d8ced-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d8ced-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8ced-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d8ced-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d8ced-114">User.Read.All、Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8ced-114">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="d8ced-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d8ced-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8ced-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8ced-116">Not supported.</span></span>    |
|<span data-ttu-id="d8ced-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d8ced-117">Application</span></span> | <span data-ttu-id="d8ced-118">User.Read.All、Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8ced-118">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8ced-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d8ced-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="d8ced-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d8ced-120">Request headers</span></span>
| <span data-ttu-id="d8ced-121">名前</span><span class="sxs-lookup"><span data-stu-id="d8ced-121">Name</span></span>       | <span data-ttu-id="d8ced-122">型</span><span class="sxs-lookup"><span data-stu-id="d8ced-122">Type</span></span> | <span data-ttu-id="d8ced-123">説明</span><span class="sxs-lookup"><span data-stu-id="d8ced-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d8ced-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8ced-124">Authorization</span></span>  | <span data-ttu-id="d8ced-125">string</span><span class="sxs-lookup"><span data-stu-id="d8ced-125">string</span></span>  | <span data-ttu-id="d8ced-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d8ced-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d8ced-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d8ced-128">Content-Type</span></span>   | <span data-ttu-id="d8ced-129">string</span><span class="sxs-lookup"><span data-stu-id="d8ced-129">string</span></span>  | <span data-ttu-id="d8ced-130">application/json</span><span class="sxs-lookup"><span data-stu-id="d8ced-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d8ced-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="d8ced-131">Request body</span></span>
<span data-ttu-id="d8ced-132">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="d8ced-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d8ced-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="d8ced-133">Parameter</span></span>    | <span data-ttu-id="d8ced-134">型</span><span class="sxs-lookup"><span data-stu-id="d8ced-134">Type</span></span>   |<span data-ttu-id="d8ced-135">説明</span><span class="sxs-lookup"><span data-stu-id="d8ced-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8ced-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="d8ced-136">securityEnabledOnly</span></span>|<span data-ttu-id="d8ced-137">ブール型</span><span class="sxs-lookup"><span data-stu-id="d8ced-137">Boolean</span></span>| <span data-ttu-id="d8ced-p105">エンティティがメンバーであるセキュリティ グループのみを返すように指定するには **true**、がメンバーであるすべてのグループとディレクトリ ロールを返すように指定するには **false** を設定します。**注**:パラメーターが **true** の場合、関数はユーザーでのみ呼び出せます。</span><span class="sxs-lookup"><span data-stu-id="d8ced-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="d8ced-140">応答</span><span class="sxs-lookup"><span data-stu-id="d8ced-140">Response</span></span>

<span data-ttu-id="d8ced-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d8ced-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8ced-142">例</span><span class="sxs-lookup"><span data-stu-id="d8ced-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d8ced-143">要求</span><span class="sxs-lookup"><span data-stu-id="d8ced-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{object-id}/getMemberObjects
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="d8ced-144">応答</span><span class="sxs-lookup"><span data-stu-id="d8ced-144">Response</span></span>
<span data-ttu-id="d8ced-p106">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d8ced-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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