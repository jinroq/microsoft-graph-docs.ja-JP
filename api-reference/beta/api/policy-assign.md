---
title: ポリシーを割り当てる
description: アプリケーションまたはサービス主体にポリシーを割り当てます。
localization_priority: Normal
ms.openlocfilehash: 30ba92c1d0308f9c4846702008a203821ae2b7b0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865458"
---
# <a name="assign-policy"></a><span data-ttu-id="d6052-103">ポリシーを割り当てる</span><span class="sxs-lookup"><span data-stu-id="d6052-103">Assign Policy</span></span>

> <span data-ttu-id="d6052-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d6052-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6052-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6052-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d6052-106">アプリケーションまたはサービス主体に[ポリシー](../resources/policy.md)を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="d6052-106">Assigns a [policy](../resources/policy.md) to an application or service principal.</span></span>

><span data-ttu-id="d6052-107">注意: 現時点では、ポリシーの割り当てにのみ適用されますトークンの有効期限ポリシー。</span><span class="sxs-lookup"><span data-stu-id="d6052-107">Note: Currently, policy assignment only applies to Token lifetime Policy.</span></span> <span data-ttu-id="d6052-108">この種類のポリシーは、[ポリシー](../resources/policy.md)の説明です。</span><span class="sxs-lookup"><span data-stu-id="d6052-108">This type of policy is described in [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d6052-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d6052-109">Permissions</span></span>
<span data-ttu-id="d6052-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d6052-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6052-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d6052-112">Permission type</span></span>      | <span data-ttu-id="d6052-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d6052-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6052-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d6052-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d6052-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d6052-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d6052-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d6052-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6052-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6052-117">Not supported.</span></span>    |
|<span data-ttu-id="d6052-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d6052-118">Application</span></span> | <span data-ttu-id="d6052-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6052-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6052-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d6052-120">HTTP request</span></span>

```http
POST /applications/{id}/policies/$ref
POST /serviceprincipals/{id}/policies/$ref
```

> <span data-ttu-id="d6052-121">注意: 要求で"id"は、アプリケーションまたはサービス ・ プリンシパル"appid"プロパティではなく"id"プロパティです。</span><span class="sxs-lookup"><span data-stu-id="d6052-121">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6052-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d6052-122">Request headers</span></span>
| <span data-ttu-id="d6052-123">名前</span><span class="sxs-lookup"><span data-stu-id="d6052-123">Name</span></span>       | <span data-ttu-id="d6052-124">種類</span><span class="sxs-lookup"><span data-stu-id="d6052-124">Type</span></span> | <span data-ttu-id="d6052-125">説明</span><span class="sxs-lookup"><span data-stu-id="d6052-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d6052-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6052-126">Authorization</span></span>  | <span data-ttu-id="d6052-127">string</span><span class="sxs-lookup"><span data-stu-id="d6052-127">string</span></span>  | <span data-ttu-id="d6052-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d6052-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d6052-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d6052-130">Content-Type</span></span> | <span data-ttu-id="d6052-131">application/json</span><span class="sxs-lookup"><span data-stu-id="d6052-131">application/json</span></span>  | <span data-ttu-id="d6052-p105">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="d6052-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6052-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="d6052-134">Request body</span></span>
<span data-ttu-id="d6052-135">要求の本文に追加するポリシー オブジェクトの JSON 表現を提供します。</span><span class="sxs-lookup"><span data-stu-id="d6052-135">In the request body, provide a JSON representation of the policy object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="d6052-136">応答</span><span class="sxs-lookup"><span data-stu-id="d6052-136">Response</span></span>

<span data-ttu-id="d6052-137">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="d6052-137">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="d6052-138">失敗した場合、`4xx`について、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="d6052-138">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="d6052-139">例</span><span class="sxs-lookup"><span data-stu-id="d6052-139">Example</span></span>
<span data-ttu-id="d6052-140">次の例では、アプリケーションにポリシーが割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="d6052-140">The following example assigns a policy to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="d6052-141">要求</span><span class="sxs-lookup"><span data-stu-id="d6052-141">Request</span></span>
<span data-ttu-id="d6052-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d6052-142">Here is an example of the request.</span></span>

```http
POST /applications/{id}/policies/$ref
Content-type: application/json
{
    "@odata.id":"https://graph.microsoft.com/beta/policies/{policyid}"
}
```

##### <a name="response"></a><span data-ttu-id="d6052-143">応答</span><span class="sxs-lookup"><span data-stu-id="d6052-143">Response</span></span>
<span data-ttu-id="d6052-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d6052-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
