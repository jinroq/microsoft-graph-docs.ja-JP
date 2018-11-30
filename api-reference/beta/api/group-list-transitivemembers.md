---
title: 推移的なメンバーのグループ一覧
description: グループのメンバーの一覧を取得します。 グループでは、メンバーとしてユーザー、連絡先、デバイス、サービス ・ プリンシパル、およびその他のグループを持つことができます。 この操作は推移的もすべての入れ子にされたメンバーの一覧を返します。
ms.openlocfilehash: a3cdc0048db3b3d1aa90b5d3426d22439a18b298
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069864"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="e74a4-105">推移的なメンバーのグループ一覧</span><span class="sxs-lookup"><span data-stu-id="e74a4-105">List group transitive members</span></span>

> <span data-ttu-id="e74a4-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e74a4-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e74a4-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e74a4-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e74a4-108">グループのメンバーの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="e74a4-108">Get a list of the group's members.</span></span> <span data-ttu-id="e74a4-109">グループでは、メンバーとしてユーザー、連絡先、デバイス、サービス ・ プリンシパル、およびその他のグループを持つことができます。</span><span class="sxs-lookup"><span data-stu-id="e74a4-109">A group can have users, contacts, devices, service principals and other groups as members.</span></span> <span data-ttu-id="e74a4-110">この操作は推移的もすべての入れ子にされたメンバーの一覧を返します。</span><span class="sxs-lookup"><span data-stu-id="e74a4-110">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="e74a4-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e74a4-111">Permissions</span></span>

<span data-ttu-id="e74a4-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e74a4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e74a4-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e74a4-114">Permission type</span></span>      | <span data-ttu-id="e74a4-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e74a4-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e74a4-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e74a4-116">Delegated (work or school account)</span></span> | <span data-ttu-id="e74a4-117">Directory.Read.All、Directory.AccessAsUser.All、User.ReadBasic.All、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e74a4-117">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="e74a4-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e74a4-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e74a4-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e74a4-119">Not supported.</span></span>    |
|<span data-ttu-id="e74a4-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e74a4-120">Application</span></span> | <span data-ttu-id="e74a4-121">Directory.Read.All、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e74a4-121">Directory.Read.All, User.Read.All</span></span> |

> <span data-ttu-id="e74a4-122">注: 非表示のメンバーシップのグループのメンバーを列挙するには、Member.Read.Hidden アクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="e74a4-122">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

## <a name="http-request"></a><span data-ttu-id="e74a4-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e74a4-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e74a4-124">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e74a4-124">Optional query parameters</span></span>

<span data-ttu-id="e74a4-125">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e74a4-125">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e74a4-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e74a4-126">Request headers</span></span>

| <span data-ttu-id="e74a4-127">名前</span><span class="sxs-lookup"><span data-stu-id="e74a4-127">Name</span></span>       | <span data-ttu-id="e74a4-128">型</span><span class="sxs-lookup"><span data-stu-id="e74a4-128">Type</span></span> | <span data-ttu-id="e74a4-129">説明</span><span class="sxs-lookup"><span data-stu-id="e74a4-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e74a4-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="e74a4-130">Authorization</span></span>  | <span data-ttu-id="e74a4-131">string</span><span class="sxs-lookup"><span data-stu-id="e74a4-131">string</span></span>  | <span data-ttu-id="e74a4-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e74a4-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e74a4-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="e74a4-134">Request body</span></span>

<span data-ttu-id="e74a4-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e74a4-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e74a4-136">応答</span><span class="sxs-lookup"><span data-stu-id="e74a4-136">Response</span></span>

<span data-ttu-id="e74a4-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e74a4-137">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e74a4-138">例</span><span class="sxs-lookup"><span data-stu-id="e74a4-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="e74a4-139">要求</span><span class="sxs-lookup"><span data-stu-id="e74a4-139">Request</span></span>

<span data-ttu-id="e74a4-140">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e74a4-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```http
GET https://graph.microsoft.com/beta/groups/{id}/tranisitiveMembers
```

### <a name="response"></a><span data-ttu-id="e74a4-141">応答</span><span class="sxs-lookup"><span data-stu-id="e74a4-141">Response</span></span>

<span data-ttu-id="e74a4-142">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e74a4-142">The following is an example of the response.</span></span>
><span data-ttu-id="e74a4-143">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="e74a4-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e74a4-144">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e74a4-144">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->