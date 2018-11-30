---
title: ポリシーを更新します。
description: 既存のポリシーのプロパティを更新します。
ms.openlocfilehash: 426476b5545e511fe2da111acb1f47f38f32c96f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073614"
---
# <a name="update-policy"></a><span data-ttu-id="8bc19-103">ポリシーを更新します。</span><span class="sxs-lookup"><span data-stu-id="8bc19-103">Update Policy</span></span>

> <span data-ttu-id="8bc19-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8bc19-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8bc19-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8bc19-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8bc19-106">既存の[ポリシー](../resources/policy.md)のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8bc19-106">Update properties in a preexisting [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8bc19-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8bc19-107">Permissions</span></span>
<span data-ttu-id="8bc19-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8bc19-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bc19-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8bc19-110">Permission type</span></span>      | <span data-ttu-id="8bc19-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8bc19-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8bc19-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8bc19-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8bc19-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8bc19-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8bc19-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8bc19-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bc19-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8bc19-115">Not supported.</span></span>    |
|<span data-ttu-id="8bc19-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8bc19-116">Application</span></span> | <span data-ttu-id="8bc19-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8bc19-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8bc19-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8bc19-118">HTTP request</span></span>

```http
PATCH /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8bc19-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8bc19-119">Request headers</span></span>
| <span data-ttu-id="8bc19-120">名前</span><span class="sxs-lookup"><span data-stu-id="8bc19-120">Name</span></span>       | <span data-ttu-id="8bc19-121">型</span><span class="sxs-lookup"><span data-stu-id="8bc19-121">Type</span></span> | <span data-ttu-id="8bc19-122">説明</span><span class="sxs-lookup"><span data-stu-id="8bc19-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8bc19-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8bc19-123">Authorization</span></span>  | <span data-ttu-id="8bc19-124">string</span><span class="sxs-lookup"><span data-stu-id="8bc19-124">string</span></span>  | <span data-ttu-id="8bc19-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8bc19-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8bc19-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8bc19-127">Content-Type</span></span> | <span data-ttu-id="8bc19-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8bc19-128">application/json</span></span>  | <span data-ttu-id="8bc19-p104">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="8bc19-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8bc19-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="8bc19-131">Request body</span></span>
<span data-ttu-id="8bc19-132">要求の本文には、更新する必要があるパラメーターを使用して JSON オブジェクトを提供します。</span><span class="sxs-lookup"><span data-stu-id="8bc19-132">In the request body, provide a JSON object with the parameters that need to be updated.</span></span> <span data-ttu-id="8bc19-133">次の表は、使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="8bc19-133">The following table shows the possible parameters.</span></span>

| <span data-ttu-id="8bc19-134">パラメーター</span><span class="sxs-lookup"><span data-stu-id="8bc19-134">Parameter</span></span>    | <span data-ttu-id="8bc19-135">型</span><span class="sxs-lookup"><span data-stu-id="8bc19-135">Type</span></span>   |<span data-ttu-id="8bc19-136">説明</span><span class="sxs-lookup"><span data-stu-id="8bc19-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8bc19-137">definition</span><span class="sxs-lookup"><span data-stu-id="8bc19-137">definition</span></span>|<span data-ttu-id="8bc19-138">String</span><span class="sxs-lookup"><span data-stu-id="8bc19-138">String</span></span>|<span data-ttu-id="8bc19-139">Stringified[ポリシー](../resources/policy.md)オブジェクトのバージョンです。</span><span class="sxs-lookup"><span data-stu-id="8bc19-139">The stringified version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="8bc19-140">displayName</span><span class="sxs-lookup"><span data-stu-id="8bc19-140">displayName</span></span>|<span data-ttu-id="8bc19-141">String</span><span class="sxs-lookup"><span data-stu-id="8bc19-141">String</span></span>|<span data-ttu-id="8bc19-142">ポリシーに独自の名前です。</span><span class="sxs-lookup"><span data-stu-id="8bc19-142">A custom name for the policy.</span></span>|
|<span data-ttu-id="8bc19-143">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="8bc19-143">isOrganizationDefault</span></span>|<span data-ttu-id="8bc19-144">ブール値</span><span class="sxs-lookup"><span data-stu-id="8bc19-144">Boolean</span></span>|<span data-ttu-id="8bc19-145">既定でこのポリシーを適用するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8bc19-145">Specifies if this policy is applied by default.</span></span>|
|<span data-ttu-id="8bc19-146">type</span><span class="sxs-lookup"><span data-stu-id="8bc19-146">type</span></span>|<span data-ttu-id="8bc19-147">String</span><span class="sxs-lookup"><span data-stu-id="8bc19-147">String</span></span>|<span data-ttu-id="8bc19-148">ポリシーの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="8bc19-148">Specifies the type of policy.</span></span> <span data-ttu-id="8bc19-149">現在、"TokenLifetimePolicy"にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="8bc19-149">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="8bc19-150">応答</span><span class="sxs-lookup"><span data-stu-id="8bc19-150">Response</span></span>

<span data-ttu-id="8bc19-151">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="8bc19-151">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="8bc19-152">失敗した場合、`4xx`について、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="8bc19-152">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="8bc19-153">使用例</span><span class="sxs-lookup"><span data-stu-id="8bc19-153">Example</span></span>
<span data-ttu-id="8bc19-154">次の例では、トークンの有効期間ポリシーの定義を更新し、組織の既定値として設定します。</span><span class="sxs-lookup"><span data-stu-id="8bc19-154">The following example updates the definition of the token lifetime policy and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="8bc19-155">要求</span><span class="sxs-lookup"><span data-stu-id="8bc19-155">Request</span></span>
<span data-ttu-id="8bc19-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8bc19-156">Here is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/beta/policies/{id}
Content-Type: application/json
{
    "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\",\"MaxInactiveTime\":\"20:00:00\",}}"],
    "isOrganizationDefault":true
}
```

##### <a name="response"></a><span data-ttu-id="8bc19-157">応答</span><span class="sxs-lookup"><span data-stu-id="8bc19-157">Response</span></span>
<span data-ttu-id="8bc19-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8bc19-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
