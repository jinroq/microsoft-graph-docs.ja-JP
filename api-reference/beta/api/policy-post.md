---
title: ポリシーの作成
description: 表示名、ポリシーの種類、およびポリシーの説明を指定して、新しいポリシーオブジェクトを作成します。
localization_priority: Normal
ms.openlocfilehash: 30a311b45f9705a07b62541a4f3a110daade09fa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546844"
---
# <a name="create-policy"></a><span data-ttu-id="ee4dd-103">ポリシーの作成</span><span class="sxs-lookup"><span data-stu-id="ee4dd-103">Create Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee4dd-104">表示名、ポリシーの種類、およびポリシーの説明を指定して、新しい[ポリシー](../resources/policy.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ee4dd-104">Create a new [policy](../resources/policy.md) object by specifying display name, policy type, and policy description.</span></span>

><span data-ttu-id="ee4dd-105">注: ポリシーの詳細は、保存される前に検証されます。</span><span class="sxs-lookup"><span data-stu-id="ee4dd-105">Note: The policy details will be validated before being stored.</span></span> <span data-ttu-id="ee4dd-106">検証に合格しない場合は、400不良要求が返されます。</span><span class="sxs-lookup"><span data-stu-id="ee4dd-106">If it does not pass validation, a 400 Bad Request will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee4dd-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ee4dd-107">Permissions</span></span>
<span data-ttu-id="ee4dd-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ee4dd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee4dd-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ee4dd-110">Permission type</span></span>      | <span data-ttu-id="ee4dd-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ee4dd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee4dd-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ee4dd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ee4dd-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ee4dd-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ee4dd-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ee4dd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee4dd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee4dd-115">Not supported.</span></span>    |
|<span data-ttu-id="ee4dd-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ee4dd-116">Application</span></span> | <span data-ttu-id="ee4dd-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee4dd-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee4dd-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ee4dd-118">HTTP request</span></span>

```http
POST /policies
```
## <a name="request-headers"></a><span data-ttu-id="ee4dd-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee4dd-119">Request headers</span></span>
| <span data-ttu-id="ee4dd-120">名前</span><span class="sxs-lookup"><span data-stu-id="ee4dd-120">Name</span></span>       | <span data-ttu-id="ee4dd-121">種類</span><span class="sxs-lookup"><span data-stu-id="ee4dd-121">Type</span></span> | <span data-ttu-id="ee4dd-122">説明</span><span class="sxs-lookup"><span data-stu-id="ee4dd-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ee4dd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee4dd-123">Authorization</span></span>  | <span data-ttu-id="ee4dd-124">string</span><span class="sxs-lookup"><span data-stu-id="ee4dd-124">string</span></span>  | <span data-ttu-id="ee4dd-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ee4dd-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ee4dd-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ee4dd-127">Content-Type</span></span> | <span data-ttu-id="ee4dd-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ee4dd-128">application/json</span></span>  | <span data-ttu-id="ee4dd-p104">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="ee4dd-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee4dd-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="ee4dd-131">Request body</span></span>
<span data-ttu-id="ee4dd-132">要求本文で、 [policy](../resources/policy.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ee4dd-132">In the request body, provide a JSON representation of [policy](../resources/policy.md) object.</span></span>

<span data-ttu-id="ee4dd-133">次の表に、ポリシーの作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ee4dd-133">The following table shows the properties that are required when you create a policy.</span></span>

| <span data-ttu-id="ee4dd-134">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ee4dd-134">Parameter</span></span>    | <span data-ttu-id="ee4dd-135">型</span><span class="sxs-lookup"><span data-stu-id="ee4dd-135">Type</span></span>   |<span data-ttu-id="ee4dd-136">説明</span><span class="sxs-lookup"><span data-stu-id="ee4dd-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee4dd-137">definition</span><span class="sxs-lookup"><span data-stu-id="ee4dd-137">definition</span></span>|<span data-ttu-id="ee4dd-138">String</span><span class="sxs-lookup"><span data-stu-id="ee4dd-138">String</span></span>|<span data-ttu-id="ee4dd-139">[ポリシー](../resources/policy.md)オブジェクトの文字列バージョン。</span><span class="sxs-lookup"><span data-stu-id="ee4dd-139">The string version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="ee4dd-140">displayName</span><span class="sxs-lookup"><span data-stu-id="ee4dd-140">displayName</span></span>|<span data-ttu-id="ee4dd-141">String</span><span class="sxs-lookup"><span data-stu-id="ee4dd-141">String</span></span>|<span data-ttu-id="ee4dd-142">ポリシーのカスタム名。</span><span class="sxs-lookup"><span data-stu-id="ee4dd-142">A custom name for the policy.</span></span>|
|<span data-ttu-id="ee4dd-143">type</span><span class="sxs-lookup"><span data-stu-id="ee4dd-143">type</span></span>|<span data-ttu-id="ee4dd-144">String</span><span class="sxs-lookup"><span data-stu-id="ee4dd-144">String</span></span>|<span data-ttu-id="ee4dd-145">ポリシーの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="ee4dd-145">Specifies the type of policy.</span></span> <span data-ttu-id="ee4dd-146">現在、"TokenLifetimePolicy" である必要があります。</span><span class="sxs-lookup"><span data-stu-id="ee4dd-146">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="ee4dd-147">応答</span><span class="sxs-lookup"><span data-stu-id="ee4dd-147">Response</span></span>

<span data-ttu-id="ee4dd-148">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[ポリシー](../resources/policy.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ee4dd-148">If successful, this method returns `201 Created` response code and [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="ee4dd-149">失敗した場合、`4xx` エラーが詳細情報とともに返されます。</span><span class="sxs-lookup"><span data-stu-id="ee4dd-149">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>  

## <a name="example"></a><span data-ttu-id="ee4dd-150">例</span><span class="sxs-lookup"><span data-stu-id="ee4dd-150">Example</span></span>
<span data-ttu-id="ee4dd-151">次の例では、新しいトークンの有効期間ポリシーを作成します。</span><span class="sxs-lookup"><span data-stu-id="ee4dd-151">The following example creates a new token lifetime Policy.</span></span> <span data-ttu-id="ee4dd-152">文字列定義パラメーターには二重引用符がエスケープされていることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="ee4dd-152">Notice the string definition parameter has escaped double quotes.</span></span>

##### <a name="request"></a><span data-ttu-id="ee4dd-153">要求</span><span class="sxs-lookup"><span data-stu-id="ee4dd-153">Request</span></span>
<span data-ttu-id="ee4dd-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ee4dd-154">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/policies
Content-Type: application/json

{
  "displayName":"CustomTokenLifetimePolicy",
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"],
  "type":"TokenLifetimePolicy"
}
```

##### <a name="response"></a><span data-ttu-id="ee4dd-155">応答</span><span class="sxs-lookup"><span data-stu-id="ee4dd-155">Response</span></span>
<span data-ttu-id="ee4dd-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ee4dd-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
