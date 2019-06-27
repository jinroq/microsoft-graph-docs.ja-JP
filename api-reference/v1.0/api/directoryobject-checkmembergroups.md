---
title: メンバー グループをチェックする
description: 指定したグループの一覧のメンバーシップを確認し、それらのグループをリストから返します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bc858afd18430635d991ce5e564b1a7c7976ad86
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275594"
---
# <a name="check-member-groups"></a><span data-ttu-id="ddd27-103">メンバー グループをチェックする</span><span class="sxs-lookup"><span data-stu-id="ddd27-103">Check member groups</span></span>

<span data-ttu-id="ddd27-p101">指定したグループのリスト内のメンバーシップを確認し、そのリストから指定したユーザー、グループまたはディレクトリ オブジェクトがメンバーであるグループを返します。この関数は、推移的です。</span><span class="sxs-lookup"><span data-stu-id="ddd27-p101">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, or directory object is a member. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="ddd27-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ddd27-106">Permissions</span></span>
<span data-ttu-id="ddd27-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ddd27-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddd27-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ddd27-109">Permission type</span></span>      | <span data-ttu-id="ddd27-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ddd27-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ddd27-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ddd27-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ddd27-112">User.Read.All、Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ddd27-112">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="ddd27-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ddd27-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddd27-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ddd27-114">Not supported.</span></span>    |
|<span data-ttu-id="ddd27-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ddd27-115">Application</span></span> | <span data-ttu-id="ddd27-116">User.Read.All、Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ddd27-116">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ddd27-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ddd27-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="ddd27-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ddd27-118">Request headers</span></span>
| <span data-ttu-id="ddd27-119">名前</span><span class="sxs-lookup"><span data-stu-id="ddd27-119">Name</span></span>       | <span data-ttu-id="ddd27-120">型</span><span class="sxs-lookup"><span data-stu-id="ddd27-120">Type</span></span> | <span data-ttu-id="ddd27-121">説明</span><span class="sxs-lookup"><span data-stu-id="ddd27-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ddd27-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddd27-122">Authorization</span></span>  | <span data-ttu-id="ddd27-123">string</span><span class="sxs-lookup"><span data-stu-id="ddd27-123">string</span></span>  | <span data-ttu-id="ddd27-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ddd27-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ddd27-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ddd27-126">Content-Type</span></span>  | <span data-ttu-id="ddd27-127">string</span><span class="sxs-lookup"><span data-stu-id="ddd27-127">string</span></span> | <span data-ttu-id="ddd27-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ddd27-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ddd27-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="ddd27-129">Request body</span></span>
<span data-ttu-id="ddd27-130">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="ddd27-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ddd27-131">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ddd27-131">Parameter</span></span>    | <span data-ttu-id="ddd27-132">型</span><span class="sxs-lookup"><span data-stu-id="ddd27-132">Type</span></span>   |<span data-ttu-id="ddd27-133">説明</span><span class="sxs-lookup"><span data-stu-id="ddd27-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ddd27-134">groupIds</span><span class="sxs-lookup"><span data-stu-id="ddd27-134">groupIds</span></span>|<span data-ttu-id="ddd27-135">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="ddd27-135">String collection</span></span>|<span data-ttu-id="ddd27-p104">メンバーシップを確認するためのグループのオブジェクト ID を含むコレクションです。最大 20 グループを指定することが可能です。</span><span class="sxs-lookup"><span data-stu-id="ddd27-p104">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="ddd27-138">応答</span><span class="sxs-lookup"><span data-stu-id="ddd27-138">Response</span></span>

<span data-ttu-id="ddd27-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ddd27-139">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddd27-140">例</span><span class="sxs-lookup"><span data-stu-id="ddd27-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ddd27-141">要求</span><span class="sxs-lookup"><span data-stu-id="ddd27-141">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="ddd27-142">応答</span><span class="sxs-lookup"><span data-stu-id="ddd27-142">Response</span></span>
<span data-ttu-id="ddd27-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ddd27-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ddd27-145">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="ddd27-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ddd27-146">C#</span><span class="sxs-lookup"><span data-stu-id="ddd27-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/directoryobject_checkmembergroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ddd27-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="ddd27-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/directoryobject_checkmembergroups-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ddd27-148">目的-C</span><span class="sxs-lookup"><span data-stu-id="ddd27-148">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/directoryobject_checkmembergroups-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/directoryobject-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/directoryobject-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/directoryobject-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
