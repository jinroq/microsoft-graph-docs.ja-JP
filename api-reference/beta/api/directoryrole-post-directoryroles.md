---
title: directoryRole をアクティブにする
description: ディレクトリ ロールをアクティブにします。 ディレクトリのロールの読み取りや、そのメンバーにする必要があります最初でアクティブにするテナントです。 会社の管理者とユーザー ディレクトリの暗黙の役割は、既定でアクティブ化されます。 アクセスし、ディレクトリの別のロールにメンバーを割り当てる、する必要があります最初をアクティブに対応するディレクトリのロール テンプレート (directoryRoleTemplate) を使用。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 44c447515a8bc9600a708b3c4a41562bd15c4e59
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975450"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="d1d0e-106">directoryRole をアクティブにする</span><span class="sxs-lookup"><span data-stu-id="d1d0e-106">Activate directoryRole</span></span>

> <span data-ttu-id="d1d0e-107">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d1d0e-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1d0e-108">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1d0e-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d1d0e-109">ディレクトリ ロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="d1d0e-109">Activate a directory role.</span></span> <span data-ttu-id="d1d0e-110">ディレクトリのロールの読み取りや、そのメンバーにする必要があります最初でアクティブにするテナントです。</span><span class="sxs-lookup"><span data-stu-id="d1d0e-110">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="d1d0e-111">会社の管理者とユーザー ディレクトリの暗黙の役割は、既定でアクティブ化されます。</span><span class="sxs-lookup"><span data-stu-id="d1d0e-111">Only the Company Administrators  and the implicit Users directory roles are activated by default.</span></span> <span data-ttu-id="d1d0e-112">アクセスし、ディレクトリの別のロールにメンバーを割り当てる、する必要があります最初をアクティブに対応するディレクトリのロール テンプレート ([directoryRoleTemplate](../resources/directoryroletemplate.md)) を使用。</span><span class="sxs-lookup"><span data-stu-id="d1d0e-112">To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="d1d0e-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d1d0e-113">Permissions</span></span>
<span data-ttu-id="d1d0e-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d1d0e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1d0e-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d1d0e-116">Permission type</span></span>      | <span data-ttu-id="d1d0e-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d1d0e-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1d0e-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d1d0e-118">Delegated (work or school account)</span></span> | <span data-ttu-id="d1d0e-119">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d1d0e-119">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d1d0e-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d1d0e-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1d0e-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1d0e-121">Not supported.</span></span>    |
|<span data-ttu-id="d1d0e-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d1d0e-122">Application</span></span> | <span data-ttu-id="d1d0e-123">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1d0e-123">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1d0e-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d1d0e-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="d1d0e-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d1d0e-125">Request headers</span></span>
| <span data-ttu-id="d1d0e-126">名前</span><span class="sxs-lookup"><span data-stu-id="d1d0e-126">Name</span></span>       | <span data-ttu-id="d1d0e-127">種類</span><span class="sxs-lookup"><span data-stu-id="d1d0e-127">Type</span></span> | <span data-ttu-id="d1d0e-128">説明</span><span class="sxs-lookup"><span data-stu-id="d1d0e-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d1d0e-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1d0e-129">Authorization</span></span>  | <span data-ttu-id="d1d0e-130">string</span><span class="sxs-lookup"><span data-stu-id="d1d0e-130">string</span></span>  | <span data-ttu-id="d1d0e-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d1d0e-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1d0e-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="d1d0e-133">Request body</span></span>
<span data-ttu-id="d1d0e-134">要求本文で、[directoryRole](../resources/directoryrole.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d1d0e-134">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="d1d0e-135">次の表に、ディレクトリ ロールをアクティブにする際に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d1d0e-135">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="d1d0e-136">必須のパラメーター</span><span class="sxs-lookup"><span data-stu-id="d1d0e-136">Required parameter</span></span> | <span data-ttu-id="d1d0e-137">種類</span><span class="sxs-lookup"><span data-stu-id="d1d0e-137">Type</span></span> | <span data-ttu-id="d1d0e-138">説明</span><span class="sxs-lookup"><span data-stu-id="d1d0e-138">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="d1d0e-139">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="d1d0e-139">roleTemplateId</span></span> | <span data-ttu-id="d1d0e-140">string</span><span class="sxs-lookup"><span data-stu-id="d1d0e-140">string</span></span> | <span data-ttu-id="d1d0e-p106">このロールが基づいている [directoryRoleTemplate](../resources/directoryroletemplate.md) の ID。これは要求で指定できる唯一のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="d1d0e-p106">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="d1d0e-143">応答</span><span class="sxs-lookup"><span data-stu-id="d1d0e-143">Response</span></span>

<span data-ttu-id="d1d0e-144">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [directoryRole](../resources/directoryrole.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d1d0e-144">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1d0e-145">例</span><span class="sxs-lookup"><span data-stu-id="d1d0e-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d1d0e-146">要求</span><span class="sxs-lookup"><span data-stu-id="d1d0e-146">Request</span></span>
<span data-ttu-id="d1d0e-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d1d0e-147">Here is an example of the request.</span></span>
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
<span data-ttu-id="d1d0e-148">要求本文で、[directoryRole](../resources/directoryrole.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d1d0e-148">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d1d0e-149">応答</span><span class="sxs-lookup"><span data-stu-id="d1d0e-149">Response</span></span>
<span data-ttu-id="d1d0e-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d1d0e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
