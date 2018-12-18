---
title: メンバーを一覧表示する
description: この API を使用して、メンバーを取得する] ボックスの一覧 (ユーザーおよびグループ) の管理単位です。
author: lleonard-msft
ms.openlocfilehash: d373c8353928d8e8d5d8b398aa09e62d457ba665
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311663"
---
# <a name="list-members"></a><span data-ttu-id="f3924-103">メンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f3924-103">List members</span></span>

> <span data-ttu-id="f3924-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f3924-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3924-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3924-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f3924-106">この API を使用して、メンバーを取得する] ボックスの一覧 (ユーザーおよびグループ) の管理単位です。</span><span class="sxs-lookup"><span data-stu-id="f3924-106">Use this API to get the members list (user and group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3924-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f3924-107">Permissions</span></span>
<span data-ttu-id="f3924-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3924-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f3924-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f3924-110">Permission type</span></span>      | <span data-ttu-id="f3924-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f3924-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3924-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f3924-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f3924-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f3924-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f3924-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f3924-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3924-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3924-115">Not supported.</span></span>    |
|<span data-ttu-id="f3924-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f3924-116">Application</span></span> | <span data-ttu-id="f3924-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3924-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="f3924-118">注: 非表示のメンバーシップの管理単位のメンバーを列挙するには、Member.Read.Hidden アクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3924-118">Note: To list the members of a hidden membership in an administrative unit, the Member.Read.Hidden permission is required.</span></span>

## <a name="http-request"></a><span data-ttu-id="f3924-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f3924-119">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members
GET /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="f3924-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3924-120">Request headers</span></span>
| <span data-ttu-id="f3924-121">名前</span><span class="sxs-lookup"><span data-stu-id="f3924-121">Name</span></span>      |<span data-ttu-id="f3924-122">説明</span><span class="sxs-lookup"><span data-stu-id="f3924-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f3924-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3924-123">Authorization</span></span>  | <span data-ttu-id="f3924-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f3924-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f3924-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f3924-126">Request body</span></span>
<span data-ttu-id="f3924-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f3924-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3924-128">応答</span><span class="sxs-lookup"><span data-stu-id="f3924-128">Response</span></span>

<span data-ttu-id="f3924-129">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本体で[ユーザー](../resources/user.md)または[グループ](../resources/group.md)のオブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f3924-129">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/user.md) and/or [group](../resources/group.md) objects in the response body.</span></span>  <span data-ttu-id="f3924-130">代わりに、配置する場合は、`$ref`の応答には要求の最後のコレクションが含まれて`@odata.id`メンバーへのリンクと Url です。</span><span class="sxs-lookup"><span data-stu-id="f3924-130">Instead, if you put `$ref` at the end of the request, the response will contain a collection of `@odata.id` links/URLs to the members.</span></span>

## <a name="examples"></a><span data-ttu-id="f3924-131">例</span><span class="sxs-lookup"><span data-stu-id="f3924-131">Examples</span></span>
##### <a name="list-member-objects"></a><span data-ttu-id="f3924-132">メンバー オブジェクトのリスト</span><span class="sxs-lookup"><span data-stu-id="f3924-132">List member objects</span></span>
<span data-ttu-id="f3924-133">次のような要求には、ユーザーおよびグループのコレクションを取得、管理単位のメンバーが表示されます。</span><span class="sxs-lookup"><span data-stu-id="f3924-133">The following request will list the members of the administrative unit, returning a collection of users and/or groups.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members
```

<span data-ttu-id="f3924-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f3924-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 
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

##### <a name="list-member-references"></a><span data-ttu-id="f3924-137">リストのメンバーの参照</span><span class="sxs-lookup"><span data-stu-id="f3924-137">List member references</span></span>
<span data-ttu-id="f3924-138">次のような要求には、メンバーの参照のコレクションを取得、管理単位が一覧表示`@odata.id`メンバーへの参照。</span><span class="sxs-lookup"><span data-stu-id="f3924-138">The following request will list the member references of the administrative unit, returning a collection of `@odata.id` references to the members.</span></span>
```
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
```
<span data-ttu-id="f3924-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f3924-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 
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
