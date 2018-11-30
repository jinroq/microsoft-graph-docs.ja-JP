---
title: エンティティ リソースの種類
description: 別のアプリケーションを呼び出すクライアント アプリケーションを要求することがまたは指定したアプリケーションのロールのユーザーまたはグループにアプリケーションを割り当てるに使用でき、アプリケーション ロールを表します。 ServicePrincipal エンティティおよびアプリケーション エンティティの**appRoles**プロパティは、**エンティティ**のコレクションです。
ms.openlocfilehash: f87ef6f40fbeb18ec4b3a2373fb2a19e14da84a4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067923"
---
# <a name="approle-resource-type"></a><span data-ttu-id="9c055-104">エンティティ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9c055-104">appRole resource type</span></span>

> <span data-ttu-id="9c055-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9c055-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c055-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9c055-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9c055-107">別のアプリケーションを呼び出すクライアント アプリケーションを要求することがまたは指定したアプリケーションのロールのユーザーまたはグループにアプリケーションを割り当てるに使用でき、アプリケーション ロールを表します。</span><span class="sxs-lookup"><span data-stu-id="9c055-107">Represents an application role that may be requested by a client application calling another application or that may be used to assign an application to users or groups in a specified application role.</span></span> <span data-ttu-id="9c055-108">[ServicePrincipal](serviceprincipal.md)エンティティおよび[アプリケーション](application.md)エンティティの**appRoles**プロパティは、**エンティティ**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="9c055-108">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **appRole**.</span></span>

> <span data-ttu-id="9c055-109">重要: この機能は現在のリリースでは無効です。</span><span class="sxs-lookup"><span data-stu-id="9c055-109">Important: This functionality is disabled in the current release.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c055-110">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9c055-110">JSON representation</span></span>

<span data-ttu-id="9c055-111">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="9c055-111">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approle"
}-->

```json
{
  "allowedMemberTypes": ["string"],
  "description": "string",
  "displayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "value": "string"
}

```
## <a name="properties"></a><span data-ttu-id="9c055-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9c055-112">Properties</span></span>
| <span data-ttu-id="9c055-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9c055-113">Property</span></span>     | <span data-ttu-id="9c055-114">型</span><span class="sxs-lookup"><span data-stu-id="9c055-114">Type</span></span>   |<span data-ttu-id="9c055-115">説明</span><span class="sxs-lookup"><span data-stu-id="9c055-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c055-116">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="9c055-116">allowedMemberTypes</span></span>|<span data-ttu-id="9c055-117">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9c055-117">String collection</span></span>|<span data-ttu-id="9c055-118">設定「アプリケーション」、またはその両方を設定を [ユーザー]、またはその他のアプリケーション (デーモン サービスのシナリオでは、このアプリケーションにアクセスしている) に、このアプリケーションの役割の定義ユーザーおよびグループに割り当てることができるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="9c055-118">Specifies whether this app role definition can be assigned to users and groups by setting to “User”, or to other applications (that are accessing this application in daemon service scenarios) by setting to “Application”, or to both.</span></span>|
|<span data-ttu-id="9c055-119">説明</span><span class="sxs-lookup"><span data-stu-id="9c055-119">description</span></span>|<span data-ttu-id="9c055-120">String</span><span class="sxs-lookup"><span data-stu-id="9c055-120">String</span></span>|<span data-ttu-id="9c055-121">アクセス許可は、ヘルプ テキストの割り当ての管理アプリケーションで表示されると、経験に同意するものです。</span><span class="sxs-lookup"><span data-stu-id="9c055-121">Permission help text that appears in the admin app assignment and consent experiences.</span></span>|
|<span data-ttu-id="9c055-122">displayName</span><span class="sxs-lookup"><span data-stu-id="9c055-122">displayName</span></span>|<span data-ttu-id="9c055-123">String</span><span class="sxs-lookup"><span data-stu-id="9c055-123">String</span></span>|<span data-ttu-id="9c055-124">管理者同意し、アプリケーションの割り当ての経験で表示されるアクセス許可の名前を表示します。</span><span class="sxs-lookup"><span data-stu-id="9c055-124">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="9c055-125">ID</span><span class="sxs-lookup"><span data-stu-id="9c055-125">id</span></span>|<span data-ttu-id="9c055-126">Guid</span><span class="sxs-lookup"><span data-stu-id="9c055-126">Guid</span></span>|<span data-ttu-id="9c055-127">**AppRoles**コレクション内のロールの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="9c055-127">Unique role identifier inside the **appRoles** collection.</span></span>|
|<span data-ttu-id="9c055-128">isEnabled</span><span class="sxs-lookup"><span data-stu-id="9c055-128">isEnabled</span></span>|<span data-ttu-id="9c055-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c055-129">Boolean</span></span>|<span data-ttu-id="9c055-130">作成するか、役割の定義の更新、これを**true** (既定値) に設定しなければなりません。</span><span class="sxs-lookup"><span data-stu-id="9c055-130">When creating or updating a role definition, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="9c055-131">ロールを削除するには、この必要があります最初設定**false を指定**します。</span><span class="sxs-lookup"><span data-stu-id="9c055-131">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="9c055-132">その時点で、後続の呼び出しでこのロールが削除されます。</span><span class="sxs-lookup"><span data-stu-id="9c055-132">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="9c055-133">value</span><span class="sxs-lookup"><span data-stu-id="9c055-133">value</span></span>|<span data-ttu-id="9c055-134">文字列</span><span class="sxs-lookup"><span data-stu-id="9c055-134">String</span></span>|<span data-ttu-id="9c055-135">認証とアクセス トークンでは、アプリケーションが期待する役割要求の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="9c055-135">Specifies the value of the roles claim that the application should expect in the authentication and access tokens.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->