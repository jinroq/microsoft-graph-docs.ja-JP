---
title: 'group: getMemberObjects'
description: 'すべてのグループとグループのメンバーである管理の単位を返します。 チェック、推移的です。 注: グループのメンバーではディレクトリの役割、ディレクトリの役割が返されないようにします。'
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: a83987a15f384cf17e268a8bdbd6791164484f7e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935928"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="5c95f-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="5c95f-105">group: getMemberObjects</span></span>

> <span data-ttu-id="5c95f-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5c95f-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c95f-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c95f-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5c95f-108">すべてのグループとグループのメンバーである管理の単位を返します。</span><span class="sxs-lookup"><span data-stu-id="5c95f-108">Return all of the groups and administrative units that the group is a member of.</span></span> <span data-ttu-id="5c95f-109">チェック、推移的です。</span><span class="sxs-lookup"><span data-stu-id="5c95f-109">The check is transitive.</span></span> <span data-ttu-id="5c95f-110">注: グループのメンバーではディレクトリの役割、ディレクトリの役割が返されないようにします。</span><span class="sxs-lookup"><span data-stu-id="5c95f-110">Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c95f-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5c95f-111">Permissions</span></span>
<span data-ttu-id="5c95f-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5c95f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c95f-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5c95f-114">Permission type</span></span>      | <span data-ttu-id="5c95f-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5c95f-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c95f-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5c95f-116">Delegated (work or school account)</span></span> | <span data-ttu-id="5c95f-117">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5c95f-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5c95f-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5c95f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c95f-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c95f-119">Not supported.</span></span>    |
|<span data-ttu-id="5c95f-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5c95f-120">Application</span></span> | <span data-ttu-id="5c95f-121">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c95f-121">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c95f-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5c95f-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="5c95f-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5c95f-123">Request headers</span></span>
| <span data-ttu-id="5c95f-124">名前</span><span class="sxs-lookup"><span data-stu-id="5c95f-124">Name</span></span>       | <span data-ttu-id="5c95f-125">型</span><span class="sxs-lookup"><span data-stu-id="5c95f-125">Type</span></span> | <span data-ttu-id="5c95f-126">説明</span><span class="sxs-lookup"><span data-stu-id="5c95f-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5c95f-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c95f-127">Authorization</span></span>  | <span data-ttu-id="5c95f-128">string</span><span class="sxs-lookup"><span data-stu-id="5c95f-128">string</span></span>  | <span data-ttu-id="5c95f-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5c95f-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c95f-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="5c95f-131">Request body</span></span>
<span data-ttu-id="5c95f-132">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="5c95f-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5c95f-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="5c95f-133">Parameter</span></span>    | <span data-ttu-id="5c95f-134">型</span><span class="sxs-lookup"><span data-stu-id="5c95f-134">Type</span></span>   |<span data-ttu-id="5c95f-135">説明</span><span class="sxs-lookup"><span data-stu-id="5c95f-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c95f-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="5c95f-136">securityEnabledOnly</span></span>|<span data-ttu-id="5c95f-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c95f-137">Boolean</span></span>|<span data-ttu-id="5c95f-p106">**false** に設定します。セキュリティが有効なグループのみを返すことは、ユーザーに対してのみサポートされます。</span><span class="sxs-lookup"><span data-stu-id="5c95f-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="5c95f-140">応答</span><span class="sxs-lookup"><span data-stu-id="5c95f-140">Response</span></span>
<span data-ttu-id="5c95f-141">成功した場合、このメソッドはグループがメンバーであるグループの ID を含んだ応答本文で `200 OK` 応答コードと文字列コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="5c95f-141">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="5c95f-142">例</span><span class="sxs-lookup"><span data-stu-id="5c95f-142">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5c95f-143">要求</span><span class="sxs-lookup"><span data-stu-id="5c95f-143">Request</span></span>
<span data-ttu-id="5c95f-144">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5c95f-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

#### <a name="response"></a><span data-ttu-id="5c95f-145">応答</span><span class="sxs-lookup"><span data-stu-id="5c95f-145">Response</span></span>
<span data-ttu-id="5c95f-146">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5c95f-146">The following is an example of the response.</span></span>
><span data-ttu-id="5c95f-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5c95f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
