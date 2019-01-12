---
title: グループ メンバーの一覧
description: グループの直接メンバーの一覧を取得します。 グループでは、メンバーとしてユーザー、連絡先、デバイス、サービス ・ プリンシパル、およびその他のグループを持つことができます。 この操作は、推移的ではありません。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 8fd082773c1661c182801eac67738165fff48490
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936159"
---
# <a name="list-group-members"></a><span data-ttu-id="d2896-105">グループ メンバーの一覧</span><span class="sxs-lookup"><span data-stu-id="d2896-105">List group members</span></span>

> <span data-ttu-id="d2896-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d2896-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2896-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2896-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d2896-108">グループの直接メンバーの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="d2896-108">Get a list of the group's direct members.</span></span> <span data-ttu-id="d2896-109">グループでは、メンバーとしてユーザー、連絡先、デバイス、サービス ・ プリンシパル、およびその他のグループを持つことができます。</span><span class="sxs-lookup"><span data-stu-id="d2896-109">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="d2896-110">この操作は、推移的ではありません。</span><span class="sxs-lookup"><span data-stu-id="d2896-110">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2896-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d2896-111">Permissions</span></span>

<span data-ttu-id="d2896-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d2896-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2896-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d2896-114">Permission type</span></span>      | <span data-ttu-id="d2896-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d2896-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2896-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d2896-116">Delegated (work or school account)</span></span> | <span data-ttu-id="d2896-117">Directory.Read.All、Directory.AccessAsUser.All、User.ReadBasic.All、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2896-117">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="d2896-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d2896-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2896-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2896-119">Not supported.</span></span>    |
|<span data-ttu-id="d2896-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d2896-120">Application</span></span> | <span data-ttu-id="d2896-121">Directory.Read.All、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2896-121">Directory.Read.All, User.Read.All</span></span> |

> <span data-ttu-id="d2896-122">注: 非表示のメンバーシップのグループのメンバーを列挙するには、Member.Read.Hidden アクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="d2896-122">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>
 
## <a name="http-request"></a><span data-ttu-id="d2896-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d2896-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d2896-124">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d2896-124">Optional query parameters</span></span>
<span data-ttu-id="d2896-125">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d2896-125">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2896-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2896-126">Request headers</span></span>
| <span data-ttu-id="d2896-127">名前</span><span class="sxs-lookup"><span data-stu-id="d2896-127">Name</span></span>       | <span data-ttu-id="d2896-128">型</span><span class="sxs-lookup"><span data-stu-id="d2896-128">Type</span></span> | <span data-ttu-id="d2896-129">説明</span><span class="sxs-lookup"><span data-stu-id="d2896-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d2896-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2896-130">Authorization</span></span>  | <span data-ttu-id="d2896-131">string</span><span class="sxs-lookup"><span data-stu-id="d2896-131">string</span></span>  | <span data-ttu-id="d2896-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d2896-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2896-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="d2896-134">Request body</span></span>
<span data-ttu-id="d2896-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d2896-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2896-136">応答</span><span class="sxs-lookup"><span data-stu-id="d2896-136">Response</span></span>
<span data-ttu-id="d2896-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d2896-137">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2896-138">例</span><span class="sxs-lookup"><span data-stu-id="d2896-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d2896-139">要求</span><span class="sxs-lookup"><span data-stu-id="d2896-139">Request</span></span>
<span data-ttu-id="d2896-140">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d2896-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/members
```

#### <a name="response"></a><span data-ttu-id="d2896-141">応答</span><span class="sxs-lookup"><span data-stu-id="d2896-141">Response</span></span>
<span data-ttu-id="d2896-142">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d2896-142">The following is an example of the response.</span></span>
><span data-ttu-id="d2896-143">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="d2896-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d2896-144">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d2896-144">All the properties will be returned from an actual call.</span></span>
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
  "description": "List group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
