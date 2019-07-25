---
title: directoryRole をアクティブにする
description: ディレクトリ ロールをアクティブ化します。 ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。 既定では、会社の管理者 (Company Administrators) とユーザー (Users) のディレクトリ ロールのみがアクティブ化されています。 アクセスしてメンバーを別のディレクトリ ロールに割り当てるには、まずそのディレクトリ ロールを対応するディレクトリ ロール テンプレート (directoryRoleTemplate) でアクティブにする必要があります。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dd7c199f25f3e2fa324fd49cf46bad93c1cd0901
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865902"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="3ba04-106">directoryRole をアクティブにする</span><span class="sxs-lookup"><span data-stu-id="3ba04-106">Activate directoryRole</span></span>

<span data-ttu-id="3ba04-p102">ディレクトリ ロールをアクティブ化します。ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。既定では、会社の管理者 (Company Administrators) とユーザー (Users) のディレクトリ ロールのみがアクティブ化されています。アクセスしてメンバーを別のディレクトリ ロールに割り当てるには、まずそのディレクトリ ロールを対応するディレクトリ ロール テンプレート ([directoryRoleTemplate](../resources/directoryroletemplate.md)) でアクティブにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="3ba04-p102">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="3ba04-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3ba04-111">Permissions</span></span>
<span data-ttu-id="3ba04-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3ba04-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ba04-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3ba04-114">Permission type</span></span>      | <span data-ttu-id="3ba04-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3ba04-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ba04-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3ba04-116">Delegated (work or school account)</span></span> | <span data-ttu-id="3ba04-117">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3ba04-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3ba04-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3ba04-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ba04-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ba04-119">Not supported.</span></span>    |
|<span data-ttu-id="3ba04-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3ba04-120">Application</span></span> | <span data-ttu-id="3ba04-121">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ba04-121">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ba04-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3ba04-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="3ba04-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3ba04-123">Request headers</span></span>
| <span data-ttu-id="3ba04-124">名前</span><span class="sxs-lookup"><span data-stu-id="3ba04-124">Name</span></span>       | <span data-ttu-id="3ba04-125">型</span><span class="sxs-lookup"><span data-stu-id="3ba04-125">Type</span></span> | <span data-ttu-id="3ba04-126">説明</span><span class="sxs-lookup"><span data-stu-id="3ba04-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3ba04-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ba04-127">Authorization</span></span>  | <span data-ttu-id="3ba04-128">string</span><span class="sxs-lookup"><span data-stu-id="3ba04-128">string</span></span>  | <span data-ttu-id="3ba04-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3ba04-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3ba04-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3ba04-131">Content-Type</span></span>  | <span data-ttu-id="3ba04-132">string</span><span class="sxs-lookup"><span data-stu-id="3ba04-132">string</span></span>  | <span data-ttu-id="3ba04-133">application/json</span><span class="sxs-lookup"><span data-stu-id="3ba04-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3ba04-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="3ba04-134">Request body</span></span>
<span data-ttu-id="3ba04-135">要求本文で、[directoryRole](../resources/directoryrole.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3ba04-135">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="3ba04-136">次の表に、ディレクトリ ロールをアクティブにする際に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3ba04-136">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="3ba04-137">パラメーター</span><span class="sxs-lookup"><span data-stu-id="3ba04-137">Parameter</span></span> | <span data-ttu-id="3ba04-138">型</span><span class="sxs-lookup"><span data-stu-id="3ba04-138">Type</span></span> | <span data-ttu-id="3ba04-139">説明</span><span class="sxs-lookup"><span data-stu-id="3ba04-139">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="3ba04-140">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="3ba04-140">roleTemplateId</span></span> | <span data-ttu-id="3ba04-141">string</span><span class="sxs-lookup"><span data-stu-id="3ba04-141">string</span></span> | <span data-ttu-id="3ba04-142">必須です。</span><span class="sxs-lookup"><span data-stu-id="3ba04-142">Required.</span></span> <span data-ttu-id="3ba04-143">このロールが基づいている [directoryRoleTemplate](../resources/directoryroletemplate.md) の ID。</span><span class="sxs-lookup"><span data-stu-id="3ba04-143">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on.</span></span> <span data-ttu-id="3ba04-144">これは要求で指定できる唯一のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="3ba04-144">This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="3ba04-145">応答</span><span class="sxs-lookup"><span data-stu-id="3ba04-145">Response</span></span>

<span data-ttu-id="3ba04-146">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [directoryRole](../resources/directoryrole.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3ba04-146">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ba04-147">例</span><span class="sxs-lookup"><span data-stu-id="3ba04-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3ba04-148">要求</span><span class="sxs-lookup"><span data-stu-id="3ba04-148">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3ba04-149">プロトコル</span><span class="sxs-lookup"><span data-stu-id="3ba04-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryrole_from_directoryroles"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles
Content-type: application/json

{
  "roleTemplateId": "roleTemplateId-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3ba04-150">C#</span><span class="sxs-lookup"><span data-stu-id="3ba04-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryrole-from-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3ba04-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="3ba04-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryrole-from-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3ba04-152">目的-C</span><span class="sxs-lookup"><span data-stu-id="3ba04-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryrole-from-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3ba04-153">Java</span><span class="sxs-lookup"><span data-stu-id="3ba04-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryrole-from-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="3ba04-154">要求本文で、[directoryRole](../resources/directoryrole.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3ba04-154">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3ba04-155">応答</span><span class="sxs-lookup"><span data-stu-id="3ba04-155">Response</span></span>
<span data-ttu-id="3ba04-p106">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3ba04-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
