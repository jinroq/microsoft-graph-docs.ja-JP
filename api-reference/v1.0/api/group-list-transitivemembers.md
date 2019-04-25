---
title: グループ推移性のメンバーを一覧表示する
description: グループのメンバーの一覧を取得します。 グループには、ユーザー、デバイス、およびその他のグループをメンバーとして含めることができます。 この操作は推移的であり、入れ子にされたすべてのメンバーのフラットな一覧も返します。
author: anchanda
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: dd6417916a7d1e2f79735db3dce4f1c3465d6577
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534711"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="2c1c1-105">グループ推移性のメンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2c1c1-105">List group transitive members</span></span>

<span data-ttu-id="2c1c1-106">グループのメンバーの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="2c1c1-106">Get a list of the group's members.</span></span> <span data-ttu-id="2c1c1-107">グループには、ユーザー、デバイス、およびその他のグループをメンバーとして含めることができます。</span><span class="sxs-lookup"><span data-stu-id="2c1c1-107">A group can have users, devices and other groups as members.</span></span> <span data-ttu-id="2c1c1-108">この操作は推移的であり、入れ子にされたすべてのメンバーのフラットな一覧も返します。</span><span class="sxs-lookup"><span data-stu-id="2c1c1-108">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c1c1-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2c1c1-109">Permissions</span></span>

<span data-ttu-id="2c1c1-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2c1c1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c1c1-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2c1c1-112">Permission type</span></span>      | <span data-ttu-id="2c1c1-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2c1c1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c1c1-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2c1c1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="2c1c1-115">directory.accessasuser.all。 all、user. all、all、all、all、all、user. all</span><span class="sxs-lookup"><span data-stu-id="2c1c1-115">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="2c1c1-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2c1c1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c1c1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2c1c1-117">Not supported.</span></span>    |
|<span data-ttu-id="2c1c1-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2c1c1-118">Application</span></span> | <span data-ttu-id="2c1c1-119">ディレクトリ。すべてのユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="2c1c1-119">Directory.Read.All, User.Read.All</span></span> |

><span data-ttu-id="2c1c1-120">**注:** 非表示のメンバーシップグループのメンバーを一覧表示するには、"hidden" アクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="2c1c1-120">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

## <a name="http-request"></a><span data-ttu-id="2c1c1-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2c1c1-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2c1c1-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2c1c1-122">Optional query parameters</span></span>

<span data-ttu-id="2c1c1-123">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2c1c1-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2c1c1-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2c1c1-124">Request headers</span></span>

| <span data-ttu-id="2c1c1-125">名前</span><span class="sxs-lookup"><span data-stu-id="2c1c1-125">Name</span></span>       | <span data-ttu-id="2c1c1-126">型</span><span class="sxs-lookup"><span data-stu-id="2c1c1-126">Type</span></span> | <span data-ttu-id="2c1c1-127">説明</span><span class="sxs-lookup"><span data-stu-id="2c1c1-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2c1c1-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c1c1-128">Authorization</span></span>  | <span data-ttu-id="2c1c1-129">string</span><span class="sxs-lookup"><span data-stu-id="2c1c1-129">string</span></span>  | <span data-ttu-id="2c1c1-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2c1c1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2c1c1-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="2c1c1-132">Request body</span></span>

<span data-ttu-id="2c1c1-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2c1c1-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c1c1-134">応答</span><span class="sxs-lookup"><span data-stu-id="2c1c1-134">Response</span></span>

<span data-ttu-id="2c1c1-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="2c1c1-135">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c1c1-136">例</span><span class="sxs-lookup"><span data-stu-id="2c1c1-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c1c1-137">要求</span><span class="sxs-lookup"><span data-stu-id="2c1c1-137">Request</span></span>

<span data-ttu-id="2c1c1-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2c1c1-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers
```

### <a name="response"></a><span data-ttu-id="2c1c1-139">応答</span><span class="sxs-lookup"><span data-stu-id="2c1c1-139">Response</span></span>

<span data-ttu-id="2c1c1-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2c1c1-140">The following is an example of the response.</span></span>
><span data-ttu-id="2c1c1-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2c1c1-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    {
      "@odata.type": "#microsoft.graph.user",
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
