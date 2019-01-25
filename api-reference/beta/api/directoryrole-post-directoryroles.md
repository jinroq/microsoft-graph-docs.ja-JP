---
title: directoryRole をアクティブにする
description: ディレクトリ ロールをアクティブ化します。ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。既定では、会社の管理者 (Company Administrators) とユーザー (Users) のディレクトリ ロールのみがアクティブ化されています。アクセスしてメンバーを別のディレクトリ ロールに割り当てるには、まずそのディレクトリ ロールを対応するディレクトリ ロール テンプレート (directoryRoleTemplate) でアクティブにする必要があります。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 094374dd8aa5d68e1adaad89e9a3b46987bc7c8f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522729"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="77f1e-106">directoryRole をアクティブにする</span><span class="sxs-lookup"><span data-stu-id="77f1e-106">Activate directoryRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77f1e-107">ディレクトリ ロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="77f1e-107">Activate a directory role.</span></span> <span data-ttu-id="77f1e-108">ディレクトリのロールの読み取りや、そのメンバーにする必要があります最初でアクティブにするテナントです。</span><span class="sxs-lookup"><span data-stu-id="77f1e-108">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="77f1e-109">会社の管理者とユーザー ディレクトリの暗黙の役割は、既定でアクティブ化されます。</span><span class="sxs-lookup"><span data-stu-id="77f1e-109">Only the Company Administrators  and the implicit Users directory roles are activated by default.</span></span> <span data-ttu-id="77f1e-110">アクセスし、ディレクトリの別のロールにメンバーを割り当てる、する必要があります最初をアクティブに対応するディレクトリのロール テンプレート ([directoryRoleTemplate](../resources/directoryroletemplate.md)) を使用。</span><span class="sxs-lookup"><span data-stu-id="77f1e-110">To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="77f1e-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="77f1e-111">Permissions</span></span>
<span data-ttu-id="77f1e-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="77f1e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77f1e-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="77f1e-114">Permission type</span></span>      | <span data-ttu-id="77f1e-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="77f1e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77f1e-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="77f1e-116">Delegated (work or school account)</span></span> | <span data-ttu-id="77f1e-117">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="77f1e-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="77f1e-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="77f1e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77f1e-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77f1e-119">Not supported.</span></span>    |
|<span data-ttu-id="77f1e-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="77f1e-120">Application</span></span> | <span data-ttu-id="77f1e-121">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77f1e-121">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="77f1e-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="77f1e-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="77f1e-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="77f1e-123">Request headers</span></span>
| <span data-ttu-id="77f1e-124">名前</span><span class="sxs-lookup"><span data-stu-id="77f1e-124">Name</span></span>       | <span data-ttu-id="77f1e-125">型</span><span class="sxs-lookup"><span data-stu-id="77f1e-125">Type</span></span> | <span data-ttu-id="77f1e-126">説明</span><span class="sxs-lookup"><span data-stu-id="77f1e-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="77f1e-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="77f1e-127">Authorization</span></span>  | <span data-ttu-id="77f1e-128">string</span><span class="sxs-lookup"><span data-stu-id="77f1e-128">string</span></span>  | <span data-ttu-id="77f1e-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="77f1e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="77f1e-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="77f1e-131">Request body</span></span>
<span data-ttu-id="77f1e-132">要求本文で、[directoryRole](../resources/directoryrole.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="77f1e-132">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="77f1e-133">次の表に、ディレクトリ ロールをアクティブにする際に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="77f1e-133">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="77f1e-134">必須のパラメーター</span><span class="sxs-lookup"><span data-stu-id="77f1e-134">Required parameter</span></span> | <span data-ttu-id="77f1e-135">種類</span><span class="sxs-lookup"><span data-stu-id="77f1e-135">Type</span></span> | <span data-ttu-id="77f1e-136">説明</span><span class="sxs-lookup"><span data-stu-id="77f1e-136">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="77f1e-137">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="77f1e-137">roleTemplateId</span></span> | <span data-ttu-id="77f1e-138">string</span><span class="sxs-lookup"><span data-stu-id="77f1e-138">string</span></span> | <span data-ttu-id="77f1e-p105">このロールが基づいている [directoryRoleTemplate](../resources/directoryroletemplate.md) の ID。これは要求で指定できる唯一のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="77f1e-p105">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="77f1e-141">応答</span><span class="sxs-lookup"><span data-stu-id="77f1e-141">Response</span></span>

<span data-ttu-id="77f1e-142">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [directoryRole](../resources/directoryrole.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="77f1e-142">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77f1e-143">例</span><span class="sxs-lookup"><span data-stu-id="77f1e-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="77f1e-144">要求</span><span class="sxs-lookup"><span data-stu-id="77f1e-144">Request</span></span>
<span data-ttu-id="77f1e-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="77f1e-145">Here is an example of the request.</span></span>
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
<span data-ttu-id="77f1e-146">要求本文で、[directoryRole](../resources/directoryrole.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="77f1e-146">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="77f1e-147">応答</span><span class="sxs-lookup"><span data-stu-id="77f1e-147">Response</span></span>
<span data-ttu-id="77f1e-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="77f1e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/directoryrole-post-directoryroles.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
