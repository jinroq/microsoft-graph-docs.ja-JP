---
title: リスト グループの推移的な memberOf
description: グループとグループのメンバーである管理の単位を取得します。  この操作では、推移的では、このグループの入れ子にされたメンバーであるすべてのグループにも含まれます。 ユーザーの Office 365 のグループを取得するとは異なり、グループのすべての種類を返しますこれだけではなく Office 365 のグループです。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: ec03ca6fce354f2a0b81cf0f81bf3061db504365
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921669"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="d2d99-105">リスト グループの推移的な memberOf</span><span class="sxs-lookup"><span data-stu-id="d2d99-105">List group transitive memberOf</span></span>

> <span data-ttu-id="d2d99-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d2d99-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2d99-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2d99-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d2d99-108">グループとグループのメンバーである管理の単位を取得します。</span><span class="sxs-lookup"><span data-stu-id="d2d99-108">Get groups and administrative units that the group is a member of.</span></span>  <span data-ttu-id="d2d99-109">この操作では、推移的では、このグループの入れ子にされたメンバーであるすべてのグループにも含まれます。</span><span class="sxs-lookup"><span data-stu-id="d2d99-109">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="d2d99-110">ユーザーの Office 365 のグループを取得するとは異なり、グループのすべての種類を返しますこれだけではなく Office 365 のグループです。</span><span class="sxs-lookup"><span data-stu-id="d2d99-110">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2d99-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d2d99-111">Permissions</span></span>

<span data-ttu-id="d2d99-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d2d99-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2d99-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d2d99-114">Permission type</span></span>      | <span data-ttu-id="d2d99-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d2d99-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2d99-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d2d99-116">Delegated (work or school account)</span></span> | <span data-ttu-id="d2d99-117">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d2d99-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d2d99-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d2d99-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2d99-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2d99-119">Not supported.</span></span>    |
|<span data-ttu-id="d2d99-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d2d99-120">Application</span></span> | <span data-ttu-id="d2d99-121">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2d99-121">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2d99-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d2d99-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d2d99-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d2d99-123">Optional query parameters</span></span>
<span data-ttu-id="d2d99-124">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d2d99-124">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2d99-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2d99-125">Request headers</span></span>
| <span data-ttu-id="d2d99-126">名前</span><span class="sxs-lookup"><span data-stu-id="d2d99-126">Name</span></span>       | <span data-ttu-id="d2d99-127">種類</span><span class="sxs-lookup"><span data-stu-id="d2d99-127">Type</span></span> | <span data-ttu-id="d2d99-128">説明</span><span class="sxs-lookup"><span data-stu-id="d2d99-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d2d99-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2d99-129">Authorization</span></span>  | <span data-ttu-id="d2d99-130">string</span><span class="sxs-lookup"><span data-stu-id="d2d99-130">string</span></span>  | <span data-ttu-id="d2d99-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d2d99-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2d99-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="d2d99-133">Request body</span></span>
<span data-ttu-id="d2d99-134">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d2d99-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2d99-135">応答</span><span class="sxs-lookup"><span data-stu-id="d2d99-135">Response</span></span>
<span data-ttu-id="d2d99-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d2d99-136">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2d99-137">例</span><span class="sxs-lookup"><span data-stu-id="d2d99-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2d99-138">要求</span><span class="sxs-lookup"><span data-stu-id="d2d99-138">Request</span></span>
<span data-ttu-id="d2d99-139">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d2d99-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="d2d99-140">応答</span><span class="sxs-lookup"><span data-stu-id="d2d99-140">Response</span></span>

<span data-ttu-id="d2d99-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d2d99-141">The following is an example of the response.</span></span>
><span data-ttu-id="d2d99-142">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="d2d99-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d2d99-143">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d2d99-143">All the properties will be returned from an actual call.</span></span>
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
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List group transitive memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
