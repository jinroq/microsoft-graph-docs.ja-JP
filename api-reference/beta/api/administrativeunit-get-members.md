---
title: メンバーを取得します。
description: 管理単位で特定のメンバー (ユーザーまたはグループ) を取得するのにには、この API を使用します。
author: lleonard-msft
ms.openlocfilehash: 9e0e8bedc349511c59e304cacfc713d54a0f8335
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328393"
---
# <a name="get-a-member"></a><span data-ttu-id="972b8-103">メンバーを取得します。</span><span class="sxs-lookup"><span data-stu-id="972b8-103">Get a member</span></span>

> <span data-ttu-id="972b8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="972b8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="972b8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="972b8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="972b8-106">管理単位で特定のメンバー (ユーザーまたはグループ) を取得するのにには、この API を使用します。</span><span class="sxs-lookup"><span data-stu-id="972b8-106">Use this API to get a specific member (user or group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="972b8-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="972b8-107">Permissions</span></span>
<span data-ttu-id="972b8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="972b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="972b8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="972b8-110">Permission type</span></span>      | <span data-ttu-id="972b8-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="972b8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="972b8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="972b8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="972b8-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="972b8-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="972b8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="972b8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="972b8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="972b8-115">Not supported.</span></span>    |
|<span data-ttu-id="972b8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="972b8-116">Application</span></span> | <span data-ttu-id="972b8-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="972b8-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="972b8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="972b8-118">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members/{id}
```
## <a name="request-headers"></a><span data-ttu-id="972b8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="972b8-119">Request headers</span></span>
| <span data-ttu-id="972b8-120">名前</span><span class="sxs-lookup"><span data-stu-id="972b8-120">Name</span></span>      |<span data-ttu-id="972b8-121">説明</span><span class="sxs-lookup"><span data-stu-id="972b8-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="972b8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="972b8-122">Authorization</span></span>  | <span data-ttu-id="972b8-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="972b8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="972b8-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="972b8-125">Request body</span></span>
<span data-ttu-id="972b8-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="972b8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="972b8-127">応答</span><span class="sxs-lookup"><span data-stu-id="972b8-127">Response</span></span>

<span data-ttu-id="972b8-128">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に、[ユーザー](../resources/user.md)または[グループ](../resources/group.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="972b8-128">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) or [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="972b8-129">例</span><span class="sxs-lookup"><span data-stu-id="972b8-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="972b8-130">要求</span><span class="sxs-lookup"><span data-stu-id="972b8-130">Request</span></span>
<span data-ttu-id="972b8-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="972b8-131">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="972b8-132">応答</span><span class="sxs-lookup"><span data-stu-id="972b8-132">Response</span></span>
<span data-ttu-id="972b8-133">ここでは、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="972b8-133">Here is an example of the respone.</span></span> <span data-ttu-id="972b8-134">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="972b8-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="972b8-135">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="972b8-135">All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "@odata.type":"#microsoft.graph.user",
  "id":"492c5308-59fd-4740-9c83-4b3db07a6d70"
  "accountEnabled":true,
  "businessPhones":[],
  "companyName":null,
  "displayName":"Demo User"
}
```