---
title: ポリシーを作成します。
description: 表示名、ポリシーの種類、およびポリシーの説明を指定することにより、新しいポリシー オブジェクトを作成します。
localization_priority: Normal
ms.openlocfilehash: 4850b2899bfd9add703af912f16602960b2657f4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831235"
---
# <a name="create-policy"></a><span data-ttu-id="c80b2-103">ポリシーを作成します。</span><span class="sxs-lookup"><span data-stu-id="c80b2-103">Create Policy</span></span>

> <span data-ttu-id="c80b2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c80b2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c80b2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c80b2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c80b2-106">表示名、ポリシーの種類、およびポリシーの説明を指定することにより、新しい[ポリシー](../resources/policy.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c80b2-106">Create a new [policy](../resources/policy.md) object by specifying display name, policy type, and policy description.</span></span>

><span data-ttu-id="c80b2-107">注: ポリシーの詳細が保存される前に検証されます。</span><span class="sxs-lookup"><span data-stu-id="c80b2-107">Note: The policy details will be validated before being stored.</span></span> <span data-ttu-id="c80b2-108">検証が合格しなかった場合、400 正しくない要求が返されます。</span><span class="sxs-lookup"><span data-stu-id="c80b2-108">If it does not pass validation, a 400 Bad Request will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="c80b2-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c80b2-109">Permissions</span></span>
<span data-ttu-id="c80b2-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c80b2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c80b2-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c80b2-112">Permission type</span></span>      | <span data-ttu-id="c80b2-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c80b2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c80b2-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c80b2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c80b2-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c80b2-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c80b2-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c80b2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c80b2-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c80b2-117">Not supported.</span></span>    |
|<span data-ttu-id="c80b2-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c80b2-118">Application</span></span> | <span data-ttu-id="c80b2-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c80b2-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c80b2-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c80b2-120">HTTP request</span></span>

```http
POST /policies
```
## <a name="request-headers"></a><span data-ttu-id="c80b2-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c80b2-121">Request headers</span></span>
| <span data-ttu-id="c80b2-122">名前</span><span class="sxs-lookup"><span data-stu-id="c80b2-122">Name</span></span>       | <span data-ttu-id="c80b2-123">種類</span><span class="sxs-lookup"><span data-stu-id="c80b2-123">Type</span></span> | <span data-ttu-id="c80b2-124">説明</span><span class="sxs-lookup"><span data-stu-id="c80b2-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c80b2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c80b2-125">Authorization</span></span>  | <span data-ttu-id="c80b2-126">string</span><span class="sxs-lookup"><span data-stu-id="c80b2-126">string</span></span>  | <span data-ttu-id="c80b2-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c80b2-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c80b2-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c80b2-129">Content-Type</span></span> | <span data-ttu-id="c80b2-130">application/json</span><span class="sxs-lookup"><span data-stu-id="c80b2-130">application/json</span></span>  | <span data-ttu-id="c80b2-p105">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="c80b2-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c80b2-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="c80b2-133">Request body</span></span>
<span data-ttu-id="c80b2-134">要求の本文には、[ポリシー](../resources/policy.md)オブジェクトの JSON 表現を提供します。</span><span class="sxs-lookup"><span data-stu-id="c80b2-134">In the request body, provide a JSON representation of [policy](../resources/policy.md) object.</span></span>

<span data-ttu-id="c80b2-135">ポリシーを作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="c80b2-135">The following table shows the properties that are required when you create a policy.</span></span>

| <span data-ttu-id="c80b2-136">Parameter</span><span class="sxs-lookup"><span data-stu-id="c80b2-136">Parameter</span></span>    | <span data-ttu-id="c80b2-137">Type</span><span class="sxs-lookup"><span data-stu-id="c80b2-137">Type</span></span>   |<span data-ttu-id="c80b2-138">説明</span><span class="sxs-lookup"><span data-stu-id="c80b2-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c80b2-139">definition</span><span class="sxs-lookup"><span data-stu-id="c80b2-139">definition</span></span>|<span data-ttu-id="c80b2-140">String</span><span class="sxs-lookup"><span data-stu-id="c80b2-140">String</span></span>|<span data-ttu-id="c80b2-141">[ポリシー](../resources/policy.md)オブジェクトの文字列形式。</span><span class="sxs-lookup"><span data-stu-id="c80b2-141">The string version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="c80b2-142">displayName</span><span class="sxs-lookup"><span data-stu-id="c80b2-142">displayName</span></span>|<span data-ttu-id="c80b2-143">String</span><span class="sxs-lookup"><span data-stu-id="c80b2-143">String</span></span>|<span data-ttu-id="c80b2-144">ポリシーに独自の名前です。</span><span class="sxs-lookup"><span data-stu-id="c80b2-144">A custom name for the policy.</span></span>|
|<span data-ttu-id="c80b2-145">type</span><span class="sxs-lookup"><span data-stu-id="c80b2-145">type</span></span>|<span data-ttu-id="c80b2-146">String</span><span class="sxs-lookup"><span data-stu-id="c80b2-146">String</span></span>|<span data-ttu-id="c80b2-147">ポリシーの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="c80b2-147">Specifies the type of policy.</span></span> <span data-ttu-id="c80b2-148">現在、"TokenLifetimePolicy"にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="c80b2-148">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="c80b2-149">応答</span><span class="sxs-lookup"><span data-stu-id="c80b2-149">Response</span></span>

<span data-ttu-id="c80b2-150">かどうかは成功すると、このメソッドを返します`201 Created`応答本体に応答コードおよび[ポリシー](../resources/policy.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c80b2-150">If successful, this method returns `201 Created` response code and [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="c80b2-151">失敗した場合、`4xx`について、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="c80b2-151">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>  

## <a name="example"></a><span data-ttu-id="c80b2-152">例</span><span class="sxs-lookup"><span data-stu-id="c80b2-152">Example</span></span>
<span data-ttu-id="c80b2-153">次の使用例は、新しいトークンの有効期間ポリシーを作成します。</span><span class="sxs-lookup"><span data-stu-id="c80b2-153">The following example creates a new token lifetime Policy.</span></span> <span data-ttu-id="c80b2-154">文字列定義のパラメーターは二重引用符をエスケープしたことを確認します。</span><span class="sxs-lookup"><span data-stu-id="c80b2-154">Notice the string definition parameter has escaped double quotes.</span></span>

##### <a name="request"></a><span data-ttu-id="c80b2-155">要求</span><span class="sxs-lookup"><span data-stu-id="c80b2-155">Request</span></span>
<span data-ttu-id="c80b2-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c80b2-156">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/policies
Content-Type: application/json

{
  "displayName":"CustomTokenLifetimePolicy",
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"],
  "type":"TokenLifetimePolicy"
}
```

##### <a name="response"></a><span data-ttu-id="c80b2-157">応答</span><span class="sxs-lookup"><span data-stu-id="c80b2-157">Response</span></span>
<span data-ttu-id="c80b2-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c80b2-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#policies/$entity",
  "id":"id-value",
  "alternativeIdentifier":null,
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"],
  "displayName":"name-value",
  "isOrganizationDefault":false,
  "keyCredentials",
  "type":"TokenLifetimePolicy"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
