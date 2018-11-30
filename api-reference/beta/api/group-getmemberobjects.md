---
title: 'group: getMemberObjects'
description: 'すべてのグループとグループのメンバーである管理の単位を返します。 チェック、推移的です。 注: グループのメンバーではディレクトリの役割、ディレクトリの役割が返されないようにします。'
ms.openlocfilehash: e0ff719b58f13f036cbf8502725fb1e146cb1227
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069863"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="b2a4c-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="b2a4c-105">group: getMemberObjects</span></span>

> <span data-ttu-id="b2a4c-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b2a4c-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2a4c-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b2a4c-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b2a4c-108">すべてのグループとグループのメンバーである管理の単位を返します。</span><span class="sxs-lookup"><span data-stu-id="b2a4c-108">Return all of the groups and administrative units that the group is a member of.</span></span> <span data-ttu-id="b2a4c-109">チェック、推移的です。</span><span class="sxs-lookup"><span data-stu-id="b2a4c-109">The check is transitive.</span></span> <span data-ttu-id="b2a4c-110">注: グループのメンバーではディレクトリの役割、ディレクトリの役割が返されないようにします。</span><span class="sxs-lookup"><span data-stu-id="b2a4c-110">Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2a4c-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b2a4c-111">Permissions</span></span>
<span data-ttu-id="b2a4c-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b2a4c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2a4c-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b2a4c-114">Permission type</span></span>      | <span data-ttu-id="b2a4c-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b2a4c-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2a4c-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b2a4c-116">Delegated (work or school account)</span></span> | <span data-ttu-id="b2a4c-117">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b2a4c-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b2a4c-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b2a4c-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2a4c-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b2a4c-119">Not supported.</span></span>    |
|<span data-ttu-id="b2a4c-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b2a4c-120">Application</span></span> | <span data-ttu-id="b2a4c-121">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2a4c-121">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2a4c-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b2a4c-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="b2a4c-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b2a4c-123">Request headers</span></span>
| <span data-ttu-id="b2a4c-124">名前</span><span class="sxs-lookup"><span data-stu-id="b2a4c-124">Name</span></span>       | <span data-ttu-id="b2a4c-125">型</span><span class="sxs-lookup"><span data-stu-id="b2a4c-125">Type</span></span> | <span data-ttu-id="b2a4c-126">説明</span><span class="sxs-lookup"><span data-stu-id="b2a4c-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b2a4c-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2a4c-127">Authorization</span></span>  | <span data-ttu-id="b2a4c-128">string</span><span class="sxs-lookup"><span data-stu-id="b2a4c-128">string</span></span>  | <span data-ttu-id="b2a4c-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b2a4c-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b2a4c-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="b2a4c-131">Request body</span></span>
<span data-ttu-id="b2a4c-132">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="b2a4c-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b2a4c-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b2a4c-133">Parameter</span></span>    | <span data-ttu-id="b2a4c-134">型</span><span class="sxs-lookup"><span data-stu-id="b2a4c-134">Type</span></span>   |<span data-ttu-id="b2a4c-135">説明</span><span class="sxs-lookup"><span data-stu-id="b2a4c-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2a4c-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="b2a4c-136">securityEnabledOnly</span></span>|<span data-ttu-id="b2a4c-137">ブール値</span><span class="sxs-lookup"><span data-stu-id="b2a4c-137">Boolean</span></span>|<span data-ttu-id="b2a4c-p106">**false** に設定します。セキュリティが有効なグループのみを返すことは、ユーザーに対してのみサポートされます。</span><span class="sxs-lookup"><span data-stu-id="b2a4c-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="b2a4c-140">応答</span><span class="sxs-lookup"><span data-stu-id="b2a4c-140">Response</span></span>
<span data-ttu-id="b2a4c-141">成功した場合、このメソッドはグループがメンバーであるグループの ID を含んだ応答本文で `200 OK` 応答コードと文字列コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b2a4c-141">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="b2a4c-142">例</span><span class="sxs-lookup"><span data-stu-id="b2a4c-142">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b2a4c-143">要求</span><span class="sxs-lookup"><span data-stu-id="b2a4c-143">Request</span></span>
<span data-ttu-id="b2a4c-144">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b2a4c-144">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="b2a4c-145">応答</span><span class="sxs-lookup"><span data-stu-id="b2a4c-145">Response</span></span>
<span data-ttu-id="b2a4c-146">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b2a4c-146">The following is an example of the response.</span></span>
><span data-ttu-id="b2a4c-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b2a4c-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
