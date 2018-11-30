---
title: 'user: getMemberObjects　'
description: ユーザーがメンバーになっているすべてのグループ、ディレクトリ ロール、管理単位を返します。チェックは推移的です。
ms.openlocfilehash: 337bf806be40b5e0af3600ea5fbeab5e94c079b7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066267"
---
# <a name="user-getmemberobjects"></a><span data-ttu-id="67389-104">user: getMemberObjects　</span><span class="sxs-lookup"><span data-stu-id="67389-104">user: getMemberObjects</span></span>

> <span data-ttu-id="67389-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="67389-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67389-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67389-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="67389-p103">ユーザーがメンバーになっているすべてのグループ、ディレクトリ ロール、管理単位を返します。チェックは推移的です。</span><span class="sxs-lookup"><span data-stu-id="67389-p103">Return all of the groups, directory roles and administrative units that the user is a member of. The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="67389-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="67389-109">Permissions</span></span>
<span data-ttu-id="67389-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="67389-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="67389-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="67389-112">Permission type</span></span>      | <span data-ttu-id="67389-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="67389-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67389-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="67389-114">Delegated (work or school account)</span></span> | <span data-ttu-id="67389-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="67389-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="67389-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="67389-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67389-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67389-117">Not supported.</span></span>    |
|<span data-ttu-id="67389-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="67389-118">Application</span></span> | <span data-ttu-id="67389-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67389-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="67389-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="67389-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="67389-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67389-121">Request headers</span></span>
| <span data-ttu-id="67389-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67389-122">Header</span></span>       | <span data-ttu-id="67389-123">値</span><span class="sxs-lookup"><span data-stu-id="67389-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="67389-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="67389-124">Authorization</span></span>  | <span data-ttu-id="67389-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="67389-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="67389-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="67389-127">Content-Type</span></span>  | <span data-ttu-id="67389-128">application/json</span><span class="sxs-lookup"><span data-stu-id="67389-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="67389-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="67389-129">Request body</span></span>
<span data-ttu-id="67389-130">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="67389-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="67389-131">パラメーター</span><span class="sxs-lookup"><span data-stu-id="67389-131">Parameter</span></span>    | <span data-ttu-id="67389-132">型</span><span class="sxs-lookup"><span data-stu-id="67389-132">Type</span></span>   |<span data-ttu-id="67389-133">説明</span><span class="sxs-lookup"><span data-stu-id="67389-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67389-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="67389-134">securityEnabledOnly</span></span>|<span data-ttu-id="67389-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="67389-135">Boolean</span></span>|<span data-ttu-id="67389-p106">ユーザーがメンバーであるセキュリティ グループのみを返すように指定するには **true**、ユーザーがメンバーであるすべてのグループとディレクトリ ロールを返すように指定するには **false** を設定します。注:このパラメーターの **true** 設定は、ユーザーに対してこのメソッドを呼び出したときにのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="67389-p106">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="67389-138">応答</span><span class="sxs-lookup"><span data-stu-id="67389-138">Response</span></span>

<span data-ttu-id="67389-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクションを返します。応答本文には、ユーザーがメンバーであるグループとディレクトリ ロールの ID が含まれています。</span><span class="sxs-lookup"><span data-stu-id="67389-139">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups and directory roles that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="67389-140">例</span><span class="sxs-lookup"><span data-stu-id="67389-140">Example</span></span>
<span data-ttu-id="67389-141">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="67389-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="67389-142">要求</span><span class="sxs-lookup"><span data-stu-id="67389-142">Request</span></span>
<span data-ttu-id="67389-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="67389-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/me/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="67389-144">応答</span><span class="sxs-lookup"><span data-stu-id="67389-144">Response</span></span>
<span data-ttu-id="67389-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="67389-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "user: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
