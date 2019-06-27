---
title: メンバー オブジェクトを取得する
description: " ユーザー、グループ、サービスプリンシパル、またはディレクトリオブジェクトがメンバーになっているすべてのグループ、管理単位、およびディレクトリロールを返します。 この関数は、推移的です。 "
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1a7517d013e30e294c324f06b37954f1bd64c932
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260743"
---
# <a name="get-member-objects"></a><span data-ttu-id="ac7cf-104">メンバー オブジェクトを取得する</span><span class="sxs-lookup"><span data-stu-id="ac7cf-104">Get member objects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

 <span data-ttu-id="ac7cf-105">ユーザー、グループ、サービスプリンシパル、またはディレクトリオブジェクトがメンバーになっているすべてのグループ、管理単位、およびディレクトリロールを返します。</span><span class="sxs-lookup"><span data-stu-id="ac7cf-105">Returns all the groups, administrative units and directory roles that a user, group, service principals or directory object is a member of.</span></span> <span data-ttu-id="ac7cf-106">この関数は、推移的です。</span><span class="sxs-lookup"><span data-stu-id="ac7cf-106">This function is transitive.</span></span> 
 > <span data-ttu-id="ac7cf-107">注:ユーザーのみがディレクトリ ロールのメンバーになることができます。</span><span class="sxs-lookup"><span data-stu-id="ac7cf-107">Note: Only users can be members of directory roles.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac7cf-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ac7cf-108">Permissions</span></span>
<span data-ttu-id="ac7cf-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ac7cf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ac7cf-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ac7cf-111">Permission type</span></span>      | <span data-ttu-id="ac7cf-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ac7cf-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac7cf-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ac7cf-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ac7cf-114">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac7cf-114">Directory.Read.All</span></span>    |
|<span data-ttu-id="ac7cf-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ac7cf-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac7cf-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac7cf-116">Not supported.</span></span>    |
|<span data-ttu-id="ac7cf-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ac7cf-117">Application</span></span> | <span data-ttu-id="ac7cf-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac7cf-118">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac7cf-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ac7cf-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberObjects
POST /servicePrincipals/{id}/getMemberObjects
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="ac7cf-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ac7cf-120">Request headers</span></span>
| <span data-ttu-id="ac7cf-121">名前</span><span class="sxs-lookup"><span data-stu-id="ac7cf-121">Name</span></span>       | <span data-ttu-id="ac7cf-122">型</span><span class="sxs-lookup"><span data-stu-id="ac7cf-122">Type</span></span> | <span data-ttu-id="ac7cf-123">説明</span><span class="sxs-lookup"><span data-stu-id="ac7cf-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ac7cf-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac7cf-124">Authorization</span></span>  | <span data-ttu-id="ac7cf-125">string</span><span class="sxs-lookup"><span data-stu-id="ac7cf-125">string</span></span>  | <span data-ttu-id="ac7cf-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ac7cf-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ac7cf-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ac7cf-128">Content-Type</span></span>  | <span data-ttu-id="ac7cf-129">application/json</span><span class="sxs-lookup"><span data-stu-id="ac7cf-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ac7cf-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="ac7cf-130">Request body</span></span>
<span data-ttu-id="ac7cf-131">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="ac7cf-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ac7cf-132">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ac7cf-132">Parameter</span></span>    | <span data-ttu-id="ac7cf-133">型</span><span class="sxs-lookup"><span data-stu-id="ac7cf-133">Type</span></span>   |<span data-ttu-id="ac7cf-134">説明</span><span class="sxs-lookup"><span data-stu-id="ac7cf-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac7cf-135">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="ac7cf-135">securityEnabledOnly</span></span>|<span data-ttu-id="ac7cf-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac7cf-136">Boolean</span></span>| <span data-ttu-id="ac7cf-p105">エンティティがメンバーであるセキュリティ グループのみを返すように指定するには **true**、がメンバーであるすべてのグループとディレクトリ ロールを返すように指定するには **false** を設定します。**注**:パラメーターが **true** の場合、関数はユーザーでのみ呼び出せます。</span><span class="sxs-lookup"><span data-stu-id="ac7cf-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="ac7cf-139">応答</span><span class="sxs-lookup"><span data-stu-id="ac7cf-139">Response</span></span>

<span data-ttu-id="ac7cf-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ac7cf-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac7cf-141">例</span><span class="sxs-lookup"><span data-stu-id="ac7cf-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ac7cf-142">要求</span><span class="sxs-lookup"><span data-stu-id="ac7cf-142">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/me/getMemberObjects
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="ac7cf-143">応答</span><span class="sxs-lookup"><span data-stu-id="ac7cf-143">Response</span></span>
<span data-ttu-id="ac7cf-p106">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ac7cf-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ac7cf-146">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="ac7cf-146">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ac7cf-147">C#</span><span class="sxs-lookup"><span data-stu-id="ac7cf-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/directoryobject_getmemberobjects-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ac7cf-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="ac7cf-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/directoryobject_getmemberobjects-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ac7cf-149">目的-C</span><span class="sxs-lookup"><span data-stu-id="ac7cf-149">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/directoryobject_getmemberobjects-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryobject-getmemberobjects.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/directoryobject-getmemberobjects.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directoryobject-getmemberobjects.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
