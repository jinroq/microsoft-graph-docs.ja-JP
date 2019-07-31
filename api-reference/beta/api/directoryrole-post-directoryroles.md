---
title: directoryRole をアクティブにする
description: ディレクトリ ロールをアクティブ化します。 ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。 既定では、会社の管理者と暗黙的なユーザーディレクトリの役割のみがアクティブになっています。 アクセスしてメンバーを別のディレクトリ ロールに割り当てるには、まずそのディレクトリ ロールを対応するディレクトリ ロール テンプレート (directoryRoleTemplate) でアクティブにする必要があります。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ef4e7ed1661309ea40a3a573fe5b830f65da7c88
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957655"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="b3473-106">directoryRole をアクティブにする</span><span class="sxs-lookup"><span data-stu-id="b3473-106">Activate directoryRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3473-107">ディレクトリ ロールをアクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="b3473-107">Activate a directory role.</span></span> <span data-ttu-id="b3473-108">ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="b3473-108">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="b3473-109">既定では、会社の管理者と暗黙的なユーザーディレクトリの役割のみがアクティブになっています。</span><span class="sxs-lookup"><span data-stu-id="b3473-109">Only the Company Administrators  and the implicit Users directory roles are activated by default.</span></span> <span data-ttu-id="b3473-110">アクセスしてメンバーを別のディレクトリ ロールに割り当てるには、まずそのディレクトリ ロールを対応するディレクトリ ロール テンプレート ([directoryRoleTemplate](../resources/directoryroletemplate.md)) でアクティブにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="b3473-110">To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="b3473-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b3473-111">Permissions</span></span>
<span data-ttu-id="b3473-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b3473-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3473-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b3473-114">Permission type</span></span>      | <span data-ttu-id="b3473-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b3473-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3473-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b3473-116">Delegated (work or school account)</span></span> | <span data-ttu-id="b3473-117">RoleManagement、Directory.accessasuser.all、およびすべてのディレクトリ</span><span class="sxs-lookup"><span data-stu-id="b3473-117">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b3473-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b3473-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3473-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3473-119">Not supported.</span></span>    |
|<span data-ttu-id="b3473-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b3473-120">Application</span></span> | <span data-ttu-id="b3473-121">RoleManagement</span><span class="sxs-lookup"><span data-stu-id="b3473-121">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3473-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b3473-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="b3473-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b3473-123">Request headers</span></span>
| <span data-ttu-id="b3473-124">名前</span><span class="sxs-lookup"><span data-stu-id="b3473-124">Name</span></span>       | <span data-ttu-id="b3473-125">型</span><span class="sxs-lookup"><span data-stu-id="b3473-125">Type</span></span> | <span data-ttu-id="b3473-126">説明</span><span class="sxs-lookup"><span data-stu-id="b3473-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b3473-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3473-127">Authorization</span></span>  | <span data-ttu-id="b3473-128">string</span><span class="sxs-lookup"><span data-stu-id="b3473-128">string</span></span>  | <span data-ttu-id="b3473-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b3473-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3473-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="b3473-131">Request body</span></span>
<span data-ttu-id="b3473-132">要求本文で、[directoryRole](../resources/directoryrole.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b3473-132">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="b3473-133">次の表に、ディレクトリ ロールをアクティブにする際に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b3473-133">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="b3473-134">必須のパラメーター</span><span class="sxs-lookup"><span data-stu-id="b3473-134">Required parameter</span></span> | <span data-ttu-id="b3473-135">型</span><span class="sxs-lookup"><span data-stu-id="b3473-135">Type</span></span> | <span data-ttu-id="b3473-136">説明</span><span class="sxs-lookup"><span data-stu-id="b3473-136">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="b3473-137">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="b3473-137">roleTemplateId</span></span> | <span data-ttu-id="b3473-138">string</span><span class="sxs-lookup"><span data-stu-id="b3473-138">string</span></span> | <span data-ttu-id="b3473-p105">このロールが基づいている [directoryRoleTemplate](../resources/directoryroletemplate.md) の ID。これは要求で指定できる唯一のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="b3473-p105">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="b3473-141">応答</span><span class="sxs-lookup"><span data-stu-id="b3473-141">Response</span></span>

<span data-ttu-id="b3473-142">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [directoryRole](../resources/directoryrole.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b3473-142">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3473-143">例</span><span class="sxs-lookup"><span data-stu-id="b3473-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b3473-144">要求</span><span class="sxs-lookup"><span data-stu-id="b3473-144">Request</span></span>
<span data-ttu-id="b3473-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b3473-145">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b3473-146">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b3473-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryrole_from_directoryroles"
}-->
```http
POST https://graph.microsoft.com/beta/directoryRoles
Content-type: application/json
Content-length: 153

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b3473-147">C#</span><span class="sxs-lookup"><span data-stu-id="b3473-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryrole-from-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b3473-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="b3473-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryrole-from-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b3473-149">目的-C</span><span class="sxs-lookup"><span data-stu-id="b3473-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryrole-from-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b3473-150">Java</span><span class="sxs-lookup"><span data-stu-id="b3473-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryrole-from-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="b3473-151">要求本文で、[directoryRole](../resources/directoryrole.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b3473-151">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b3473-152">応答</span><span class="sxs-lookup"><span data-stu-id="b3473-152">Response</span></span>
<span data-ttu-id="b3473-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b3473-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 175

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
