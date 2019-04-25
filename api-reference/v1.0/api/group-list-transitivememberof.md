---
title: リストグループ推移的な memberOf
description: グループがメンバーであるグループを取得します。  この操作は推移的で、このグループがネストされたメンバーであるすべてのグループも含みます。 ユーザーの office 365 グループを取得する場合とは異なり、office 365 グループだけでなく、すべての種類のグループを返します。
author: anchanda
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 7134318471101309dcf8f2778106afa549e9aa62
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542019"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="f69be-105">リストグループ推移的な memberOf</span><span class="sxs-lookup"><span data-stu-id="f69be-105">List group transitive memberOf</span></span>

<span data-ttu-id="f69be-106">グループがメンバーであるグループを取得します。</span><span class="sxs-lookup"><span data-stu-id="f69be-106">Get groups that the group is a member of.</span></span>  <span data-ttu-id="f69be-107">この操作は推移的で、このグループがネストされたメンバーであるすべてのグループも含みます。</span><span class="sxs-lookup"><span data-stu-id="f69be-107">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="f69be-108">ユーザーの office 365 グループを取得する場合とは異なり、office 365 グループだけでなく、すべての種類のグループを返します。</span><span class="sxs-lookup"><span data-stu-id="f69be-108">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="f69be-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f69be-109">Permissions</span></span>

<span data-ttu-id="f69be-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f69be-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f69be-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f69be-112">Permission type</span></span>      | <span data-ttu-id="f69be-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f69be-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f69be-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f69be-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f69be-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f69be-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f69be-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f69be-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f69be-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f69be-117">Not supported.</span></span>    |
|<span data-ttu-id="f69be-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f69be-118">Application</span></span> | <span data-ttu-id="f69be-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f69be-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f69be-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f69be-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f69be-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f69be-121">Optional query parameters</span></span>
<span data-ttu-id="f69be-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f69be-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f69be-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f69be-123">Request headers</span></span>
| <span data-ttu-id="f69be-124">名前</span><span class="sxs-lookup"><span data-stu-id="f69be-124">Name</span></span>       | <span data-ttu-id="f69be-125">型</span><span class="sxs-lookup"><span data-stu-id="f69be-125">Type</span></span> | <span data-ttu-id="f69be-126">説明</span><span class="sxs-lookup"><span data-stu-id="f69be-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f69be-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="f69be-127">Authorization</span></span>  | <span data-ttu-id="f69be-128">string</span><span class="sxs-lookup"><span data-stu-id="f69be-128">string</span></span>  | <span data-ttu-id="f69be-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f69be-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f69be-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="f69be-131">Request body</span></span>
<span data-ttu-id="f69be-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f69be-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f69be-133">応答</span><span class="sxs-lookup"><span data-stu-id="f69be-133">Response</span></span>
<span data-ttu-id="f69be-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f69be-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f69be-135">例</span><span class="sxs-lookup"><span data-stu-id="f69be-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="f69be-136">要求</span><span class="sxs-lookup"><span data-stu-id="f69be-136">Request</span></span>
<span data-ttu-id="f69be-137">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f69be-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="f69be-138">応答</span><span class="sxs-lookup"><span data-stu-id="f69be-138">Response</span></span>

<span data-ttu-id="f69be-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f69be-139">The following is an example of the response.</span></span>
><span data-ttu-id="f69be-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f69be-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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