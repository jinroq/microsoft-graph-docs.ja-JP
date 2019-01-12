---
title: directoryRole をアクティブにする
description: ディレクトリ ロールをアクティブ化します。ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。既定では、会社の管理者 (Company Administrators) とユーザー (Users) のディレクトリ ロールのみがアクティブ化されています。アクセスしてメンバーを別のディレクトリ ロールに割り当てるには、まずそのディレクトリ ロールを対応するディレクトリ ロール テンプレート (directoryRoleTemplate) でアクティブにする必要があります。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5d127580c0a4851c5a991ccc0646007ddf1298a5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924917"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="3ad74-106">directoryRole をアクティブにする</span><span class="sxs-lookup"><span data-stu-id="3ad74-106">Activate directoryRole</span></span>

<span data-ttu-id="3ad74-p102">ディレクトリ ロールをアクティブ化します。ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。既定では、会社の管理者 (Company Administrators) とユーザー (Users) のディレクトリ ロールのみがアクティブ化されています。アクセスしてメンバーを別のディレクトリ ロールに割り当てるには、まずそのディレクトリ ロールを対応するディレクトリ ロール テンプレート ([directoryRoleTemplate](../resources/directoryroletemplate.md)) でアクティブにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="3ad74-p102">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="3ad74-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3ad74-111">Permissions</span></span>
<span data-ttu-id="3ad74-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3ad74-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ad74-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3ad74-114">Permission type</span></span>      | <span data-ttu-id="3ad74-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3ad74-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ad74-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3ad74-116">Delegated (work or school account)</span></span> | <span data-ttu-id="3ad74-117">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3ad74-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3ad74-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3ad74-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ad74-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ad74-119">Not supported.</span></span>    |
|<span data-ttu-id="3ad74-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3ad74-120">Application</span></span> | <span data-ttu-id="3ad74-121">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ad74-121">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ad74-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3ad74-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="3ad74-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3ad74-123">Request headers</span></span>
| <span data-ttu-id="3ad74-124">名前</span><span class="sxs-lookup"><span data-stu-id="3ad74-124">Name</span></span>       | <span data-ttu-id="3ad74-125">種類</span><span class="sxs-lookup"><span data-stu-id="3ad74-125">Type</span></span> | <span data-ttu-id="3ad74-126">説明</span><span class="sxs-lookup"><span data-stu-id="3ad74-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3ad74-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ad74-127">Authorization</span></span>  | <span data-ttu-id="3ad74-128">string</span><span class="sxs-lookup"><span data-stu-id="3ad74-128">string</span></span>  | <span data-ttu-id="3ad74-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3ad74-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3ad74-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3ad74-131">Content-Type</span></span>  | <span data-ttu-id="3ad74-132">string</span><span class="sxs-lookup"><span data-stu-id="3ad74-132">string</span></span>  | <span data-ttu-id="3ad74-133">application/json</span><span class="sxs-lookup"><span data-stu-id="3ad74-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3ad74-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="3ad74-134">Request body</span></span>
<span data-ttu-id="3ad74-135">要求本文で、[directoryRole](../resources/directoryrole.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3ad74-135">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="3ad74-136">次の表に、ディレクトリ ロールをアクティブにする際に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3ad74-136">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="3ad74-137">Parameter</span><span class="sxs-lookup"><span data-stu-id="3ad74-137">Parameter</span></span> | <span data-ttu-id="3ad74-138">Type</span><span class="sxs-lookup"><span data-stu-id="3ad74-138">Type</span></span> | <span data-ttu-id="3ad74-139">説明</span><span class="sxs-lookup"><span data-stu-id="3ad74-139">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="3ad74-140">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="3ad74-140">roleTemplateId</span></span> | <span data-ttu-id="3ad74-141">文字列</span><span class="sxs-lookup"><span data-stu-id="3ad74-141">string</span></span> | <span data-ttu-id="3ad74-142">必須。</span><span class="sxs-lookup"><span data-stu-id="3ad74-142">Required.</span></span> <span data-ttu-id="3ad74-143">ロールは、に基づいて[directoryRoleTemplate](../resources/directoryroletemplate.md)の ID です。</span><span class="sxs-lookup"><span data-stu-id="3ad74-143">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on.</span></span> <span data-ttu-id="3ad74-144">これは、要求内で指定できる唯一のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="3ad74-144">This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="3ad74-145">応答</span><span class="sxs-lookup"><span data-stu-id="3ad74-145">Response</span></span>

<span data-ttu-id="3ad74-146">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [directoryRole](../resources/directoryrole.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3ad74-146">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ad74-147">例</span><span class="sxs-lookup"><span data-stu-id="3ad74-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3ad74-148">要求</span><span class="sxs-lookup"><span data-stu-id="3ad74-148">Request</span></span>

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
<span data-ttu-id="3ad74-149">要求本文で、[directoryRole](../resources/directoryrole.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3ad74-149">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3ad74-150">応答</span><span class="sxs-lookup"><span data-stu-id="3ad74-150">Response</span></span>
<span data-ttu-id="3ad74-p106">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3ad74-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
