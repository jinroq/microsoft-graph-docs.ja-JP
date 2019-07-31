---
title: ポリシーの更新
description: 既存のポリシーのプロパティを更新します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 85104248d840478a9595382b54d3eaa7ea7e1e5b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978862"
---
# <a name="update-policy"></a><span data-ttu-id="cb947-103">ポリシーの更新</span><span class="sxs-lookup"><span data-stu-id="cb947-103">Update Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb947-104">既存の[ポリシー](../resources/policy.md)のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cb947-104">Update properties in a preexisting [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cb947-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cb947-105">Permissions</span></span>
<span data-ttu-id="cb947-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cb947-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb947-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cb947-108">Permission type</span></span>      | <span data-ttu-id="cb947-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cb947-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb947-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cb947-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cb947-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cb947-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cb947-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cb947-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb947-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cb947-113">Not supported.</span></span>    |
|<span data-ttu-id="cb947-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cb947-114">Application</span></span> | <span data-ttu-id="cb947-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cb947-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb947-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cb947-116">HTTP request</span></span>

```http
PATCH /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="cb947-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cb947-117">Request headers</span></span>
| <span data-ttu-id="cb947-118">名前</span><span class="sxs-lookup"><span data-stu-id="cb947-118">Name</span></span>       | <span data-ttu-id="cb947-119">種類</span><span class="sxs-lookup"><span data-stu-id="cb947-119">Type</span></span> | <span data-ttu-id="cb947-120">説明</span><span class="sxs-lookup"><span data-stu-id="cb947-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cb947-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb947-121">Authorization</span></span>  | <span data-ttu-id="cb947-122">string</span><span class="sxs-lookup"><span data-stu-id="cb947-122">string</span></span>  | <span data-ttu-id="cb947-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cb947-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cb947-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cb947-125">Content-Type</span></span> | <span data-ttu-id="cb947-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cb947-126">application/json</span></span>  | <span data-ttu-id="cb947-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="cb947-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb947-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="cb947-129">Request body</span></span>
<span data-ttu-id="cb947-130">要求本文で、更新する必要があるパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="cb947-130">In the request body, provide a JSON object with the parameters that need to be updated.</span></span> <span data-ttu-id="cb947-131">次の表に、使用可能なパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="cb947-131">The following table shows the possible parameters.</span></span>

| <span data-ttu-id="cb947-132">パラメーター</span><span class="sxs-lookup"><span data-stu-id="cb947-132">Parameter</span></span>    | <span data-ttu-id="cb947-133">型</span><span class="sxs-lookup"><span data-stu-id="cb947-133">Type</span></span>   |<span data-ttu-id="cb947-134">説明</span><span class="sxs-lookup"><span data-stu-id="cb947-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb947-135">definition</span><span class="sxs-lookup"><span data-stu-id="cb947-135">definition</span></span>|<span data-ttu-id="cb947-136">String</span><span class="sxs-lookup"><span data-stu-id="cb947-136">String</span></span>|<span data-ttu-id="cb947-137">文字列バージョンの[ポリシー](../resources/policy.md)オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="cb947-137">The stringified version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="cb947-138">displayName</span><span class="sxs-lookup"><span data-stu-id="cb947-138">displayName</span></span>|<span data-ttu-id="cb947-139">文字列</span><span class="sxs-lookup"><span data-stu-id="cb947-139">String</span></span>|<span data-ttu-id="cb947-140">ポリシーのカスタム名。</span><span class="sxs-lookup"><span data-stu-id="cb947-140">A custom name for the policy.</span></span>|
|<span data-ttu-id="cb947-141">Is組織既定</span><span class="sxs-lookup"><span data-stu-id="cb947-141">isOrganizationDefault</span></span>|<span data-ttu-id="cb947-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb947-142">Boolean</span></span>|<span data-ttu-id="cb947-143">このポリシーを既定で適用するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="cb947-143">Specifies if this policy is applied by default.</span></span>|
|<span data-ttu-id="cb947-144">type</span><span class="sxs-lookup"><span data-stu-id="cb947-144">type</span></span>|<span data-ttu-id="cb947-145">String</span><span class="sxs-lookup"><span data-stu-id="cb947-145">String</span></span>|<span data-ttu-id="cb947-146">ポリシーの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="cb947-146">Specifies the type of policy.</span></span> <span data-ttu-id="cb947-147">現在、"TokenLifetimePolicy" である必要があります。</span><span class="sxs-lookup"><span data-stu-id="cb947-147">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="cb947-148">応答</span><span class="sxs-lookup"><span data-stu-id="cb947-148">Response</span></span>

<span data-ttu-id="cb947-149">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="cb947-149">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="cb947-150">失敗した場合、`4xx` エラーが詳細情報とともに返されます。</span><span class="sxs-lookup"><span data-stu-id="cb947-150">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="cb947-151">例</span><span class="sxs-lookup"><span data-stu-id="cb947-151">Example</span></span>
<span data-ttu-id="cb947-152">次の例では、トークン有効期限ポリシーの定義を更新し、それを組織の既定値として設定します。</span><span class="sxs-lookup"><span data-stu-id="cb947-152">The following example updates the definition of the token lifetime policy and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="cb947-153">要求</span><span class="sxs-lookup"><span data-stu-id="cb947-153">Request</span></span>
<span data-ttu-id="cb947-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cb947-154">Here is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/beta/policies/{id}
Content-Type: application/json
{
    "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\",\"MaxInactiveTime\":\"20:00:00\",}}"],
    "isOrganizationDefault":true
}
```

##### <a name="response"></a><span data-ttu-id="cb947-155">応答</span><span class="sxs-lookup"><span data-stu-id="cb947-155">Response</span></span>
<span data-ttu-id="cb947-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cb947-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
