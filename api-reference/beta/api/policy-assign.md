---
title: ポリシーの割り当て
description: アプリケーションまたはサービスプリンシパルにポリシーを割り当てます。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: af128019d35838dd5873de713f011fd5b7f1c6ad
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978890"
---
# <a name="assign-policy"></a><span data-ttu-id="2a06c-103">ポリシーの割り当て</span><span class="sxs-lookup"><span data-stu-id="2a06c-103">Assign Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a06c-104">アプリケーションまたはサービスプリンシパルに[ポリシー](../resources/policy.md)を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="2a06c-104">Assigns a [policy](../resources/policy.md) to an application or service principal.</span></span>

><span data-ttu-id="2a06c-105">注: 現時点では、ポリシーの割り当てはトークンの有効期限ポリシーにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="2a06c-105">Note: Currently, policy assignment only applies to Token lifetime Policy.</span></span> <span data-ttu-id="2a06c-106">この種類のポリシーについては、「[ポリシー](../resources/policy.md)」で説明します。</span><span class="sxs-lookup"><span data-stu-id="2a06c-106">This type of policy is described in [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2a06c-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2a06c-107">Permissions</span></span>
<span data-ttu-id="2a06c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2a06c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a06c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2a06c-110">Permission type</span></span>      | <span data-ttu-id="2a06c-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2a06c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a06c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2a06c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2a06c-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2a06c-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2a06c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2a06c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a06c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2a06c-115">Not supported.</span></span>    |
|<span data-ttu-id="2a06c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2a06c-116">Application</span></span> | <span data-ttu-id="2a06c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2a06c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a06c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2a06c-118">HTTP request</span></span>

```http
POST /applications/{id}/policies/$ref
POST /serviceprincipals/{id}/policies/$ref
```

> <span data-ttu-id="2a06c-119">注: 要求の "id" は、"appid" プロパティではなく、アプリケーションまたはサービスプリンシパルの "id" プロパティです。</span><span class="sxs-lookup"><span data-stu-id="2a06c-119">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2a06c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2a06c-120">Request headers</span></span>
| <span data-ttu-id="2a06c-121">名前</span><span class="sxs-lookup"><span data-stu-id="2a06c-121">Name</span></span>       | <span data-ttu-id="2a06c-122">型</span><span class="sxs-lookup"><span data-stu-id="2a06c-122">Type</span></span> | <span data-ttu-id="2a06c-123">説明</span><span class="sxs-lookup"><span data-stu-id="2a06c-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2a06c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a06c-124">Authorization</span></span>  | <span data-ttu-id="2a06c-125">string</span><span class="sxs-lookup"><span data-stu-id="2a06c-125">string</span></span>  | <span data-ttu-id="2a06c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2a06c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2a06c-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2a06c-128">Content-Type</span></span> | <span data-ttu-id="2a06c-129">application/json</span><span class="sxs-lookup"><span data-stu-id="2a06c-129">application/json</span></span>  | <span data-ttu-id="2a06c-p104">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="2a06c-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a06c-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="2a06c-132">Request body</span></span>
<span data-ttu-id="2a06c-133">要求本文で、追加するポリシーオブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2a06c-133">In the request body, provide a JSON representation of the policy object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="2a06c-134">応答</span><span class="sxs-lookup"><span data-stu-id="2a06c-134">Response</span></span>

<span data-ttu-id="2a06c-135">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="2a06c-135">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="2a06c-136">失敗した場合、`4xx` エラーが詳細情報とともに返されます。</span><span class="sxs-lookup"><span data-stu-id="2a06c-136">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="2a06c-137">例</span><span class="sxs-lookup"><span data-stu-id="2a06c-137">Example</span></span>
<span data-ttu-id="2a06c-138">次の例では、アプリケーションにポリシーを割り当てます。</span><span class="sxs-lookup"><span data-stu-id="2a06c-138">The following example assigns a policy to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="2a06c-139">要求</span><span class="sxs-lookup"><span data-stu-id="2a06c-139">Request</span></span>
<span data-ttu-id="2a06c-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2a06c-140">Here is an example of the request.</span></span>

```http
POST /applications/{id}/policies/$ref
Content-type: application/json
{
    "@odata.id":"https://graph.microsoft.com/beta/policies/{policyid}"
}
```

##### <a name="response"></a><span data-ttu-id="2a06c-141">応答</span><span class="sxs-lookup"><span data-stu-id="2a06c-141">Response</span></span>
<span data-ttu-id="2a06c-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2a06c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
