---
title: 推移的なメンバーのグループ一覧
description: グループのメンバーの一覧を取得します。 グループでは、メンバーとしてユーザー、連絡先、デバイス、サービス ・ プリンシパル、およびその他のグループを持つことができます。 この操作は推移的もすべての入れ子にされたメンバーの一覧を返します。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: e1dc5c2b89305373b22b6ef87cfaee25d6669750
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523625"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="5f56c-105">推移的なメンバーのグループ一覧</span><span class="sxs-lookup"><span data-stu-id="5f56c-105">List group transitive members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f56c-106">グループのメンバーの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="5f56c-106">Get a list of the group's members.</span></span> <span data-ttu-id="5f56c-107">グループでは、メンバーとしてユーザー、連絡先、デバイス、サービス ・ プリンシパル、およびその他のグループを持つことができます。</span><span class="sxs-lookup"><span data-stu-id="5f56c-107">A group can have users, contacts, devices, service principals and other groups as members.</span></span> <span data-ttu-id="5f56c-108">この操作は推移的もすべての入れ子にされたメンバーの一覧を返します。</span><span class="sxs-lookup"><span data-stu-id="5f56c-108">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f56c-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5f56c-109">Permissions</span></span>

<span data-ttu-id="5f56c-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5f56c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f56c-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5f56c-112">Permission type</span></span>      | <span data-ttu-id="5f56c-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5f56c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f56c-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5f56c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5f56c-115">Directory.Read.All、Directory.AccessAsUser.All、User.ReadBasic.All、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f56c-115">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="5f56c-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5f56c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f56c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f56c-117">Not supported.</span></span>    |
|<span data-ttu-id="5f56c-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5f56c-118">Application</span></span> | <span data-ttu-id="5f56c-119">Directory.Read.All、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f56c-119">Directory.Read.All, User.Read.All</span></span> |

> <span data-ttu-id="5f56c-120">注: 非表示のメンバーシップのグループのメンバーを列挙するには、Member.Read.Hidden アクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="5f56c-120">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

## <a name="http-request"></a><span data-ttu-id="5f56c-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5f56c-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5f56c-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5f56c-122">Optional query parameters</span></span>

<span data-ttu-id="5f56c-123">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5f56c-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f56c-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5f56c-124">Request headers</span></span>

| <span data-ttu-id="5f56c-125">名前</span><span class="sxs-lookup"><span data-stu-id="5f56c-125">Name</span></span>       | <span data-ttu-id="5f56c-126">型</span><span class="sxs-lookup"><span data-stu-id="5f56c-126">Type</span></span> | <span data-ttu-id="5f56c-127">説明</span><span class="sxs-lookup"><span data-stu-id="5f56c-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5f56c-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f56c-128">Authorization</span></span>  | <span data-ttu-id="5f56c-129">string</span><span class="sxs-lookup"><span data-stu-id="5f56c-129">string</span></span>  | <span data-ttu-id="5f56c-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5f56c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f56c-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="5f56c-132">Request body</span></span>

<span data-ttu-id="5f56c-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5f56c-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f56c-134">応答</span><span class="sxs-lookup"><span data-stu-id="5f56c-134">Response</span></span>

<span data-ttu-id="5f56c-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="5f56c-135">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f56c-136">例</span><span class="sxs-lookup"><span data-stu-id="5f56c-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f56c-137">要求</span><span class="sxs-lookup"><span data-stu-id="5f56c-137">Request</span></span>

<span data-ttu-id="5f56c-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5f56c-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```http
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers
```

### <a name="response"></a><span data-ttu-id="5f56c-139">応答</span><span class="sxs-lookup"><span data-stu-id="5f56c-139">Response</span></span>

<span data-ttu-id="5f56c-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5f56c-140">The following is an example of the response.</span></span>
><span data-ttu-id="5f56c-141">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="5f56c-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5f56c-142">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5f56c-142">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    "@odata.type": "#microsoft.graph.user",
    {
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-transitivemembers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
