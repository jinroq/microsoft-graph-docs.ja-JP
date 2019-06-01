---
title: メンバーを一覧表示する
description: この API を使用して、管理単位でメンバーリスト (ユーザーとグループ) を取得します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d48bf767e8d786002bb523e39970a3e77f72738e
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655307"
---
# <a name="list-members"></a><span data-ttu-id="08dc2-103">メンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="08dc2-103">List members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08dc2-104">この API を使用して、管理単位でメンバーリスト (ユーザーとグループ) を取得します。</span><span class="sxs-lookup"><span data-stu-id="08dc2-104">Use this API to get the members list (user and group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="08dc2-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="08dc2-105">Permissions</span></span>
<span data-ttu-id="08dc2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="08dc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="08dc2-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="08dc2-108">Permission type</span></span>      | <span data-ttu-id="08dc2-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="08dc2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08dc2-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="08dc2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="08dc2-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="08dc2-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="08dc2-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="08dc2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08dc2-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="08dc2-113">Not supported.</span></span>    |
|<span data-ttu-id="08dc2-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="08dc2-114">Application</span></span> | <span data-ttu-id="08dc2-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08dc2-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="08dc2-116">注: 管理単位の非表示のメンバーシップのメンバーを一覧表示するには、"Hidden" アクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="08dc2-116">Note: To list the members of a hidden membership in an administrative unit, the Member.Read.Hidden permission is required.</span></span>

## <a name="http-request"></a><span data-ttu-id="08dc2-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="08dc2-117">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members
GET /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="08dc2-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="08dc2-118">Request headers</span></span>
| <span data-ttu-id="08dc2-119">名前</span><span class="sxs-lookup"><span data-stu-id="08dc2-119">Name</span></span>      |<span data-ttu-id="08dc2-120">説明</span><span class="sxs-lookup"><span data-stu-id="08dc2-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="08dc2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="08dc2-121">Authorization</span></span>  | <span data-ttu-id="08dc2-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="08dc2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08dc2-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="08dc2-124">Request body</span></span>
<span data-ttu-id="08dc2-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="08dc2-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08dc2-126">応答</span><span class="sxs-lookup"><span data-stu-id="08dc2-126">Response</span></span>

<span data-ttu-id="08dc2-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[ユーザー](../resources/user.md)オブジェクトまたは[グループ](../resources/group.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="08dc2-127">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/user.md) and/or [group](../resources/group.md) objects in the response body.</span></span>  <span data-ttu-id="08dc2-128">代わりに、要求の最後`$ref`にを置くと、応答にはメンバーへのリンク/url `@odata.id`のコレクションが含まれます。</span><span class="sxs-lookup"><span data-stu-id="08dc2-128">Instead, if you put `$ref` at the end of the request, the response will contain a collection of `@odata.id` links/URLs to the members.</span></span>

## <a name="examples"></a><span data-ttu-id="08dc2-129">例</span><span class="sxs-lookup"><span data-stu-id="08dc2-129">Examples</span></span>
##### <a name="list-member-objects"></a><span data-ttu-id="08dc2-130">メンバーオブジェクトを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="08dc2-130">List member objects</span></span>
<span data-ttu-id="08dc2-131">次の要求は、管理単位のメンバーを一覧表示し、ユーザーまたはグループのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="08dc2-131">The following request will list the members of the administrative unit, returning a collection of users and/or groups.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members
```

<span data-ttu-id="08dc2-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="08dc2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "value":[
    {
      "@odata.type":"#microsoft.graph.user",
      "id":"492c5308-59fd-4740-9c83-4b3db07a6d70"
      "accountEnabled":true,
      "businessPhones":[],
      "companyName":null,
      "displayName":"Demo User"
    },
    {
      "@odata.type":"#microsoft.graph.group",
      "id":"07eaa5c7-c9b6-45cf-8ff7-3147d5122caa",
      "description":"This group is the best ever",
      "displayName":"Awesome group"
    }
  ]
}
```

##### <a name="list-member-references"></a><span data-ttu-id="08dc2-135">リストメンバーの参照</span><span class="sxs-lookup"><span data-stu-id="08dc2-135">List member references</span></span>
<span data-ttu-id="08dc2-136">次の要求では、管理単位のメンバ参照がリストされ、メンバー `@odata.id`への参照のコレクションが返されます。</span><span class="sxs-lookup"><span data-stu-id="08dc2-136">The following request will list the member references of the administrative unit, returning a collection of `@odata.id` references to the members.</span></span>
```
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
```
<span data-ttu-id="08dc2-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="08dc2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "value":[
    {
      "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/492c5308-59fd-4740-9c83-4b3db07a6d70"
    },
    {
      "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/07eaa5c7-c9b6-45cf-8ff7-3147d5122caa"
    }
  ]
}
```
