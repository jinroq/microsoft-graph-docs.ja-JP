---
title: グループへの後方リンクの一覧
description: グループとグループの直接メンバーである管理の単位を取得します。
ms.openlocfilehash: 5c189571095676d0c52b8bb93a8d27136d4aaa3c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069490"
---
# <a name="list-group-memberof"></a><span data-ttu-id="73c4a-103">グループへの後方リンクの一覧</span><span class="sxs-lookup"><span data-stu-id="73c4a-103">List group memberOf</span></span>

> <span data-ttu-id="73c4a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="73c4a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73c4a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73c4a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="73c4a-106">グループとグループの直接メンバーである管理の単位を取得します。</span><span class="sxs-lookup"><span data-stu-id="73c4a-106">Get groups and administrative units that the group is a direct member of.</span></span>

<span data-ttu-id="73c4a-107">この操作は、推移的ではありません。</span><span class="sxs-lookup"><span data-stu-id="73c4a-107">This operation is not transitive.</span></span> <span data-ttu-id="73c4a-108">ユーザーの Office 365 のグループを取得するとは異なり、グループのすべての種類を返しますこれだけではなく Office 365 のグループです。</span><span class="sxs-lookup"><span data-stu-id="73c4a-108">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span> 

## <a name="permissions"></a><span data-ttu-id="73c4a-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="73c4a-109">Permissions</span></span>

<span data-ttu-id="73c4a-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="73c4a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73c4a-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="73c4a-112">Permission type</span></span>      | <span data-ttu-id="73c4a-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="73c4a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73c4a-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="73c4a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="73c4a-115">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="73c4a-115">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="73c4a-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="73c4a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73c4a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73c4a-117">Not supported.</span></span>    |
|<span data-ttu-id="73c4a-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="73c4a-118">Application</span></span> | <span data-ttu-id="73c4a-119">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73c4a-119">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="73c4a-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="73c4a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="73c4a-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="73c4a-121">Optional query parameters</span></span>
<span data-ttu-id="73c4a-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="73c4a-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="73c4a-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="73c4a-123">Request headers</span></span>
| <span data-ttu-id="73c4a-124">名前</span><span class="sxs-lookup"><span data-stu-id="73c4a-124">Name</span></span>       | <span data-ttu-id="73c4a-125">型</span><span class="sxs-lookup"><span data-stu-id="73c4a-125">Type</span></span> | <span data-ttu-id="73c4a-126">説明</span><span class="sxs-lookup"><span data-stu-id="73c4a-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="73c4a-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="73c4a-127">Authorization</span></span>  | <span data-ttu-id="73c4a-128">string</span><span class="sxs-lookup"><span data-stu-id="73c4a-128">string</span></span>  | <span data-ttu-id="73c4a-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="73c4a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73c4a-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="73c4a-131">Request body</span></span>
<span data-ttu-id="73c4a-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="73c4a-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73c4a-133">応答</span><span class="sxs-lookup"><span data-stu-id="73c4a-133">Response</span></span>
<span data-ttu-id="73c4a-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="73c4a-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73c4a-135">例</span><span class="sxs-lookup"><span data-stu-id="73c4a-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="73c4a-136">要求</span><span class="sxs-lookup"><span data-stu-id="73c4a-136">Request</span></span>

<span data-ttu-id="73c4a-137">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="73c4a-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="73c4a-138">応答</span><span class="sxs-lookup"><span data-stu-id="73c4a-138">Response</span></span>

<span data-ttu-id="73c4a-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="73c4a-139">The following is an example of the response.</span></span>
><span data-ttu-id="73c4a-140">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="73c4a-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="73c4a-141">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="73c4a-141">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->