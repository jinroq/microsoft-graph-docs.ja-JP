---
title: 'user: getMemberObjects　'
description: ユーザーがメンバーになっているすべてのグループ、ディレクトリ ロール、および管理単位を返します。チェックは推移的です。
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6b737ee5115060d02ee476b9bd0f1af4a6424e12
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567920"
---
# <a name="user-getmemberobjects"></a><span data-ttu-id="c5055-104">user: getMemberObjects　</span><span class="sxs-lookup"><span data-stu-id="c5055-104">user: getMemberObjects</span></span>
<span data-ttu-id="c5055-p102">ユーザーがメンバーになっているすべてのグループ、ディレクトリ ロール、管理単位を返します。チェックは推移的です。</span><span class="sxs-lookup"><span data-stu-id="c5055-p102">Return all of the groups, directory roles and administrative units that the user is a member of. The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5055-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c5055-107">Permissions</span></span>
<span data-ttu-id="c5055-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c5055-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c5055-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c5055-110">Permission type</span></span>      | <span data-ttu-id="c5055-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c5055-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5055-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c5055-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c5055-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c5055-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c5055-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c5055-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5055-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c5055-115">Not supported.</span></span>    |
|<span data-ttu-id="c5055-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c5055-116">Application</span></span> | <span data-ttu-id="c5055-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5055-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5055-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c5055-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="c5055-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c5055-119">Request headers</span></span>
| <span data-ttu-id="c5055-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c5055-120">Header</span></span>       | <span data-ttu-id="c5055-121">値</span><span class="sxs-lookup"><span data-stu-id="c5055-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c5055-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5055-122">Authorization</span></span>  | <span data-ttu-id="c5055-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c5055-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c5055-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c5055-125">Content-Type</span></span>  | <span data-ttu-id="c5055-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5055-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c5055-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c5055-127">Request body</span></span>
<span data-ttu-id="c5055-128">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="c5055-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c5055-129">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c5055-129">Parameter</span></span>    | <span data-ttu-id="c5055-130">型</span><span class="sxs-lookup"><span data-stu-id="c5055-130">Type</span></span>   |<span data-ttu-id="c5055-131">説明</span><span class="sxs-lookup"><span data-stu-id="c5055-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5055-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="c5055-132">securityEnabledOnly</span></span>|<span data-ttu-id="c5055-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5055-133">Boolean</span></span>|<span data-ttu-id="c5055-p105">ユーザーがメンバーであるセキュリティ グループのみを返すように指定するには **true**、ユーザーがメンバーであるすべてのグループとディレクトリ ロールを返すように指定するには **false** を設定します。注:このパラメーターの **true** 設定は、ユーザーに対してこのメソッドを呼び出したときにのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="c5055-p105">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups and directory roles that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="c5055-136">応答</span><span class="sxs-lookup"><span data-stu-id="c5055-136">Response</span></span>

<span data-ttu-id="c5055-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクションを返します。応答本文には、ユーザーがメンバーであるグループとディレクトリ ロールの ID が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c5055-137">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups and directory roles that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="c5055-138">例</span><span class="sxs-lookup"><span data-stu-id="c5055-138">Example</span></span>
<span data-ttu-id="c5055-139">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="c5055-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c5055-140">要求</span><span class="sxs-lookup"><span data-stu-id="c5055-140">Request</span></span>
<span data-ttu-id="c5055-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c5055-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="c5055-142">応答</span><span class="sxs-lookup"><span data-stu-id="c5055-142">Response</span></span>
<span data-ttu-id="c5055-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c5055-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
