---
title: エンティティ リソースの種類
description: 別のアプリケーションを呼び出すクライアント アプリケーションを要求することがまたは指定したアプリケーションのロールのユーザーまたはグループにアプリケーションを割り当てるに使用でき、アプリケーション ロールを表します。 ServicePrincipal エンティティおよびアプリケーション エンティティの**appRoles**プロパティは、**エンティティ**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: 8a367406c64cf9d0d3da49716aeaf6ca3c1fa687
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640414"
---
# <a name="approle-resource-type"></a><span data-ttu-id="150a0-104">エンティティ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="150a0-104">appRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="150a0-105">別のアプリケーションを呼び出すクライアント アプリケーションを要求することがまたは指定したアプリケーションのロールのユーザーまたはグループにアプリケーションを割り当てるに使用でき、アプリケーション ロールを表します。</span><span class="sxs-lookup"><span data-stu-id="150a0-105">Represents an application role that may be requested by a client application calling another application or that may be used to assign an application to users or groups in a specified application role.</span></span> <span data-ttu-id="150a0-106">[ServicePrincipal](serviceprincipal.md)エンティティおよび[アプリケーション](application.md)エンティティの**appRoles**プロパティは、**エンティティ**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="150a0-106">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **appRole**.</span></span>

> <span data-ttu-id="150a0-107">重要: この機能は現在のリリースでは無効です。</span><span class="sxs-lookup"><span data-stu-id="150a0-107">Important: This functionality is disabled in the current release.</span></span>

## <a name="json-representation"></a><span data-ttu-id="150a0-108">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="150a0-108">JSON representation</span></span>

<span data-ttu-id="150a0-109">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="150a0-109">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="150a0-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="150a0-110">Properties</span></span>
| <span data-ttu-id="150a0-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="150a0-111">Property</span></span>     | <span data-ttu-id="150a0-112">型</span><span class="sxs-lookup"><span data-stu-id="150a0-112">Type</span></span>   |<span data-ttu-id="150a0-113">説明</span><span class="sxs-lookup"><span data-stu-id="150a0-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="150a0-114">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="150a0-114">allowedMemberTypes</span></span>|<span data-ttu-id="150a0-115">String コレクション</span><span class="sxs-lookup"><span data-stu-id="150a0-115">String collection</span></span>|<span data-ttu-id="150a0-116">設定「アプリケーション」、またはその両方を設定を [ユーザー]、またはその他のアプリケーション (デーモン サービスのシナリオでは、このアプリケーションにアクセスしている) に、このアプリケーションの役割の定義ユーザーおよびグループに割り当てることができるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="150a0-116">Specifies whether this app role definition can be assigned to users and groups by setting to “User”, or to other applications (that are accessing this application in daemon service scenarios) by setting to “Application”, or to both.</span></span>|
|<span data-ttu-id="150a0-117">説明</span><span class="sxs-lookup"><span data-stu-id="150a0-117">description</span></span>|<span data-ttu-id="150a0-118">String</span><span class="sxs-lookup"><span data-stu-id="150a0-118">String</span></span>|<span data-ttu-id="150a0-119">アクセス許可は、ヘルプ テキストの割り当ての管理アプリケーションで表示されると、経験に同意するものです。</span><span class="sxs-lookup"><span data-stu-id="150a0-119">Permission help text that appears in the admin app assignment and consent experiences.</span></span>|
|<span data-ttu-id="150a0-120">displayName</span><span class="sxs-lookup"><span data-stu-id="150a0-120">displayName</span></span>|<span data-ttu-id="150a0-121">String</span><span class="sxs-lookup"><span data-stu-id="150a0-121">String</span></span>|<span data-ttu-id="150a0-122">管理者同意し、アプリケーションの割り当ての経験で表示されるアクセス許可の名前を表示します。</span><span class="sxs-lookup"><span data-stu-id="150a0-122">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="150a0-123">id</span><span class="sxs-lookup"><span data-stu-id="150a0-123">id</span></span>|<span data-ttu-id="150a0-124">Guid</span><span class="sxs-lookup"><span data-stu-id="150a0-124">Guid</span></span>|<span data-ttu-id="150a0-125">**AppRoles**コレクション内のロールの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="150a0-125">Unique role identifier inside the **appRoles** collection.</span></span>|
|<span data-ttu-id="150a0-126">isEnabled</span><span class="sxs-lookup"><span data-stu-id="150a0-126">isEnabled</span></span>|<span data-ttu-id="150a0-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="150a0-127">Boolean</span></span>|<span data-ttu-id="150a0-128">作成するか、役割の定義の更新、これを**true** (既定値) に設定しなければなりません。</span><span class="sxs-lookup"><span data-stu-id="150a0-128">When creating or updating a role definition, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="150a0-129">ロールを削除するには、この必要があります最初設定**false を指定**します。</span><span class="sxs-lookup"><span data-stu-id="150a0-129">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="150a0-130">その時点で、後続の呼び出しでこのロールが削除されます。</span><span class="sxs-lookup"><span data-stu-id="150a0-130">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="150a0-131">value</span><span class="sxs-lookup"><span data-stu-id="150a0-131">value</span></span>|<span data-ttu-id="150a0-132">文字列</span><span class="sxs-lookup"><span data-stu-id="150a0-132">String</span></span>|<span data-ttu-id="150a0-133">認証とアクセス トークンでは、アプリケーションが期待する役割要求の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="150a0-133">Specifies the value of the roles claim that the application should expect in the authentication and access tokens.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/approle.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
