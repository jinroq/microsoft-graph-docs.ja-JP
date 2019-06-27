---
title: directoryRole をアクティブにする
description: ディレクトリ ロールをアクティブ化します。 ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。 既定では、会社の管理者と暗黙的なユーザーディレクトリの役割のみがアクティブになっています。 アクセスしてメンバーを別のディレクトリ ロールに割り当てるには、まずそのディレクトリ ロールを対応するディレクトリ ロール テンプレート (directoryRoleTemplate) でアクティブにする必要があります。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 10689fa2902dc53aa3a3246aafb9bd923d5d2e89
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260677"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="b34e0-106">directoryRole をアクティブにする</span><span class="sxs-lookup"><span data-stu-id="b34e0-106">Activate directoryRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b34e0-107">ディレクトリ ロールをアクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="b34e0-107">Activate a directory role.</span></span> <span data-ttu-id="b34e0-108">ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="b34e0-108">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="b34e0-109">既定では、会社の管理者と暗黙的なユーザーディレクトリの役割のみがアクティブになっています。</span><span class="sxs-lookup"><span data-stu-id="b34e0-109">Only the Company Administrators  and the implicit Users directory roles are activated by default.</span></span> <span data-ttu-id="b34e0-110">アクセスしてメンバーを別のディレクトリ ロールに割り当てるには、まずそのディレクトリ ロールを対応するディレクトリ ロール テンプレート ([directoryRoleTemplate](../resources/directoryroletemplate.md)) でアクティブにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="b34e0-110">To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="b34e0-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b34e0-111">Permissions</span></span>
<span data-ttu-id="b34e0-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b34e0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b34e0-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b34e0-114">Permission type</span></span>      | <span data-ttu-id="b34e0-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b34e0-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b34e0-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b34e0-116">Delegated (work or school account)</span></span> | <span data-ttu-id="b34e0-117">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b34e0-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b34e0-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b34e0-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b34e0-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b34e0-119">Not supported.</span></span>    |
|<span data-ttu-id="b34e0-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b34e0-120">Application</span></span> | <span data-ttu-id="b34e0-121">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b34e0-121">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b34e0-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b34e0-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="b34e0-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b34e0-123">Request headers</span></span>
| <span data-ttu-id="b34e0-124">名前</span><span class="sxs-lookup"><span data-stu-id="b34e0-124">Name</span></span>       | <span data-ttu-id="b34e0-125">型</span><span class="sxs-lookup"><span data-stu-id="b34e0-125">Type</span></span> | <span data-ttu-id="b34e0-126">説明</span><span class="sxs-lookup"><span data-stu-id="b34e0-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b34e0-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b34e0-127">Authorization</span></span>  | <span data-ttu-id="b34e0-128">string</span><span class="sxs-lookup"><span data-stu-id="b34e0-128">string</span></span>  | <span data-ttu-id="b34e0-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b34e0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b34e0-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="b34e0-131">Request body</span></span>
<span data-ttu-id="b34e0-132">要求本文で、[directoryRole](../resources/directoryrole.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b34e0-132">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="b34e0-133">次の表に、ディレクトリ ロールをアクティブにする際に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b34e0-133">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="b34e0-134">必須のパラメーター</span><span class="sxs-lookup"><span data-stu-id="b34e0-134">Required parameter</span></span> | <span data-ttu-id="b34e0-135">型</span><span class="sxs-lookup"><span data-stu-id="b34e0-135">Type</span></span> | <span data-ttu-id="b34e0-136">説明</span><span class="sxs-lookup"><span data-stu-id="b34e0-136">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="b34e0-137">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="b34e0-137">roleTemplateId</span></span> | <span data-ttu-id="b34e0-138">string</span><span class="sxs-lookup"><span data-stu-id="b34e0-138">string</span></span> | <span data-ttu-id="b34e0-p105">このロールが基づいている [directoryRoleTemplate](../resources/directoryroletemplate.md) の ID。これは要求で指定できる唯一のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="b34e0-p105">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="b34e0-141">応答</span><span class="sxs-lookup"><span data-stu-id="b34e0-141">Response</span></span>

<span data-ttu-id="b34e0-142">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [directoryRole](../resources/directoryrole.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b34e0-142">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b34e0-143">例</span><span class="sxs-lookup"><span data-stu-id="b34e0-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b34e0-144">要求</span><span class="sxs-lookup"><span data-stu-id="b34e0-144">Request</span></span>
<span data-ttu-id="b34e0-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b34e0-145">Here is an example of the request.</span></span>
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
<span data-ttu-id="b34e0-146">要求本文で、[directoryRole](../resources/directoryrole.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b34e0-146">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b34e0-147">応答</span><span class="sxs-lookup"><span data-stu-id="b34e0-147">Response</span></span>
<span data-ttu-id="b34e0-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b34e0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b34e0-151">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="b34e0-151">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b34e0-152">C#</span><span class="sxs-lookup"><span data-stu-id="b34e0-152">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_directoryrole_from_directoryroles-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b34e0-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="b34e0-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryrole_from_directoryroles-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b34e0-154">目的-C</span><span class="sxs-lookup"><span data-stu-id="b34e0-154">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_directoryrole_from_directoryroles-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/directoryrole-post-directoryroles.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/directoryrole-post-directoryroles.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directoryrole-post-directoryroles.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
