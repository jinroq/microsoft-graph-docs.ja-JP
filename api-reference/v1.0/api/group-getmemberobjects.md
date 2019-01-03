---
title: 'group: getMemberObjects'
description: このグループがメンバーであるすべてのグループを返します。チェックは推移的です。注:グループは、ディレクトリ ロールのメンバーになれないので、ディレクトリ ロールは返されません。
ms.openlocfilehash: 59f3408434c77290552080b6b7b99a20e6fe19db
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022337"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="be411-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="be411-105">group: getMemberObjects</span></span>
<span data-ttu-id="be411-p102">このグループがメンバーであるすべてのグループを返します。チェックは推移的です。注:グループは、ディレクトリ ロールのメンバーになれないので、ディレクトリ ロールは返されません。</span><span class="sxs-lookup"><span data-stu-id="be411-p102">Return all of the groups that this group is a member of. The check is transitive. Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="be411-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="be411-109">Permissions</span></span>
<span data-ttu-id="be411-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be411-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be411-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="be411-112">Permission type</span></span>      | <span data-ttu-id="be411-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="be411-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be411-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="be411-114">Delegated (work or school account)</span></span> | <span data-ttu-id="be411-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="be411-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="be411-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="be411-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be411-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be411-117">Not supported.</span></span>    |
|<span data-ttu-id="be411-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="be411-118">Application</span></span> | <span data-ttu-id="be411-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be411-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="be411-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="be411-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="be411-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="be411-121">Request headers</span></span>
| <span data-ttu-id="be411-122">名前</span><span class="sxs-lookup"><span data-stu-id="be411-122">Name</span></span>       | <span data-ttu-id="be411-123">型</span><span class="sxs-lookup"><span data-stu-id="be411-123">Type</span></span> | <span data-ttu-id="be411-124">説明</span><span class="sxs-lookup"><span data-stu-id="be411-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="be411-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="be411-125">Authorization</span></span>  | <span data-ttu-id="be411-126">string</span><span class="sxs-lookup"><span data-stu-id="be411-126">string</span></span>  | <span data-ttu-id="be411-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="be411-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be411-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="be411-129">Request body</span></span>
<span data-ttu-id="be411-130">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="be411-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="be411-131">パラメーター</span><span class="sxs-lookup"><span data-stu-id="be411-131">Parameter</span></span>    | <span data-ttu-id="be411-132">型</span><span class="sxs-lookup"><span data-stu-id="be411-132">Type</span></span>   |<span data-ttu-id="be411-133">説明</span><span class="sxs-lookup"><span data-stu-id="be411-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be411-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="be411-134">securityEnabledOnly</span></span>|<span data-ttu-id="be411-135">ブール値</span><span class="sxs-lookup"><span data-stu-id="be411-135">Boolean</span></span>| <span data-ttu-id="be411-p105">**false** に設定します。セキュリティが有効なグループのみを返すことは、ユーザーに対してのみサポートされます。</span><span class="sxs-lookup"><span data-stu-id="be411-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="be411-138">応答</span><span class="sxs-lookup"><span data-stu-id="be411-138">Response</span></span>
<span data-ttu-id="be411-139">成功した場合、このメソッドはグループがメンバーであるグループの ID を含んだ応答本文で `200 OK` 応答コードと文字列コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="be411-139">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="be411-140">例</span><span class="sxs-lookup"><span data-stu-id="be411-140">Example</span></span>
#### <a name="request"></a><span data-ttu-id="be411-141">要求</span><span class="sxs-lookup"><span data-stu-id="be411-141">Request</span></span>
<span data-ttu-id="be411-142">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="be411-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

#### <a name="response"></a><span data-ttu-id="be411-143">応答</span><span class="sxs-lookup"><span data-stu-id="be411-143">Response</span></span>
<span data-ttu-id="be411-144">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="be411-144">The following is an example of the response.</span></span>
><span data-ttu-id="be411-145">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="be411-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="be411-146">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="be411-146">All the properties will be returned from an actual call.</span></span>
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