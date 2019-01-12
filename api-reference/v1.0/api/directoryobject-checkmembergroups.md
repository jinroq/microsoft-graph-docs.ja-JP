---
title: メンバー グループをチェックする
description: メンバーシップのグループ、およびそのリストから指定されたリスト内のそれらのグループを確認します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 99ebf38b8f230233b50fa642f7503302afd02b33
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941787"
---
# <a name="check-member-groups"></a><span data-ttu-id="a5beb-103">メンバー グループをチェックする</span><span class="sxs-lookup"><span data-stu-id="a5beb-103">Check member groups</span></span>

<span data-ttu-id="a5beb-p101">指定したグループのリスト内のメンバーシップを確認し、そのリストから指定したユーザー、グループまたはディレクトリ オブジェクトがメンバーであるグループを返します。この関数は、推移的です。</span><span class="sxs-lookup"><span data-stu-id="a5beb-p101">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, or directory object is a member. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5beb-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a5beb-106">Permissions</span></span>
<span data-ttu-id="a5beb-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a5beb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5beb-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a5beb-109">Permission type</span></span>      | <span data-ttu-id="a5beb-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a5beb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5beb-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a5beb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a5beb-112">User.Read.All、Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5beb-112">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="a5beb-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a5beb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5beb-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5beb-114">Not supported.</span></span>    |
|<span data-ttu-id="a5beb-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a5beb-115">Application</span></span> | <span data-ttu-id="a5beb-116">User.Read.All、Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5beb-116">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5beb-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a5beb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="a5beb-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a5beb-118">Request headers</span></span>
| <span data-ttu-id="a5beb-119">名前</span><span class="sxs-lookup"><span data-stu-id="a5beb-119">Name</span></span>       | <span data-ttu-id="a5beb-120">種類</span><span class="sxs-lookup"><span data-stu-id="a5beb-120">Type</span></span> | <span data-ttu-id="a5beb-121">説明</span><span class="sxs-lookup"><span data-stu-id="a5beb-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a5beb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5beb-122">Authorization</span></span>  | <span data-ttu-id="a5beb-123">string</span><span class="sxs-lookup"><span data-stu-id="a5beb-123">string</span></span>  | <span data-ttu-id="a5beb-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a5beb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a5beb-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a5beb-126">Content-Type</span></span>  | <span data-ttu-id="a5beb-127">string</span><span class="sxs-lookup"><span data-stu-id="a5beb-127">string</span></span> | <span data-ttu-id="a5beb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a5beb-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a5beb-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="a5beb-129">Request body</span></span>
<span data-ttu-id="a5beb-130">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="a5beb-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a5beb-131">パラメーター</span><span class="sxs-lookup"><span data-stu-id="a5beb-131">Parameter</span></span>    | <span data-ttu-id="a5beb-132">Type</span><span class="sxs-lookup"><span data-stu-id="a5beb-132">Type</span></span>   |<span data-ttu-id="a5beb-133">説明</span><span class="sxs-lookup"><span data-stu-id="a5beb-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5beb-134">groupIds</span><span class="sxs-lookup"><span data-stu-id="a5beb-134">groupIds</span></span>|<span data-ttu-id="a5beb-135">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a5beb-135">String collection</span></span>|<span data-ttu-id="a5beb-p104">メンバーシップを確認するためのグループのオブジェクト ID を含むコレクションです。最大 20 グループを指定することが可能です。</span><span class="sxs-lookup"><span data-stu-id="a5beb-p104">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="a5beb-138">応答</span><span class="sxs-lookup"><span data-stu-id="a5beb-138">Response</span></span>

<span data-ttu-id="a5beb-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a5beb-139">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5beb-140">例</span><span class="sxs-lookup"><span data-stu-id="a5beb-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a5beb-141">要求</span><span class="sxs-lookup"><span data-stu-id="a5beb-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{id}/checkMemberGroups
Content-type: application/json

{
  "groupIds": [
        "fee2c45b-915a-4a64b130f4eb9e75525e",
        "4fe90ae065a-478b9400e0a0e1cbd540"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="a5beb-142">応答</span><span class="sxs-lookup"><span data-stu-id="a5beb-142">Response</span></span>
<span data-ttu-id="a5beb-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a5beb-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
