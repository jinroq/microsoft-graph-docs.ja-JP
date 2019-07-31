---
title: appRole リソースの種類
description: 別のアプリケーションを呼び出しているクライアントアプリケーションによって要求されるか、または指定されたアプリケーションロールのユーザーまたはグループにアプリケーションを割り当てるために使用される可能性があるアプリケーションロールを表します。 ServicePrincipal エンティティおよび application エンティティの**approles**プロパティは、 **approles**のコレクションです。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 35c26e52c5d7eb9529474d08a43b68fceddfc954
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013327"
---
# <a name="approle-resource-type"></a><span data-ttu-id="b7f08-104">appRole リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b7f08-104">appRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7f08-105">別のアプリケーションを呼び出しているクライアントアプリケーションによって要求されるか、または指定されたアプリケーションロールのユーザーまたはグループにアプリケーションを割り当てるために使用される可能性があるアプリケーションロールを表します。</span><span class="sxs-lookup"><span data-stu-id="b7f08-105">Represents an application role that may be requested by a client application calling another application or that may be used to assign an application to users or groups in a specified application role.</span></span> <span data-ttu-id="b7f08-106">[Serviceprincipal](serviceprincipal.md)エンティティおよび[Application](application.md)エンティティの**Approles**プロパティは、 **approles**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="b7f08-106">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **appRole**.</span></span>

> <span data-ttu-id="b7f08-107">重要: この機能は現在のリリースでは無効になっています。</span><span class="sxs-lookup"><span data-stu-id="b7f08-107">Important: This functionality is disabled in the current release.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7f08-108">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b7f08-108">JSON representation</span></span>

<span data-ttu-id="b7f08-109">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="b7f08-109">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appRole"
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
## <a name="properties"></a><span data-ttu-id="b7f08-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7f08-110">Properties</span></span>
| <span data-ttu-id="b7f08-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7f08-111">Property</span></span>     | <span data-ttu-id="b7f08-112">型</span><span class="sxs-lookup"><span data-stu-id="b7f08-112">Type</span></span>   |<span data-ttu-id="b7f08-113">説明</span><span class="sxs-lookup"><span data-stu-id="b7f08-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7f08-114">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="b7f08-114">allowedMemberTypes</span></span>|<span data-ttu-id="b7f08-115">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="b7f08-115">String collection</span></span>|<span data-ttu-id="b7f08-116">"Application" に設定するか、またはその両方に設定して、このアプリの役割定義をユーザーとグループに割り当てることができるようにするかどうかを指定します。 "User" に設定するか、または (デーモンサービスシナリオでこのアプリケーションにアクセスしている) 他のアプリケーションに割り当てます。</span><span class="sxs-lookup"><span data-stu-id="b7f08-116">Specifies whether this app role definition can be assigned to users and groups by setting to "User", or to other applications (that are accessing this application in daemon service scenarios) by setting to "Application", or to both.</span></span>|
|<span data-ttu-id="b7f08-117">description</span><span class="sxs-lookup"><span data-stu-id="b7f08-117">description</span></span>|<span data-ttu-id="b7f08-118">String</span><span class="sxs-lookup"><span data-stu-id="b7f08-118">String</span></span>|<span data-ttu-id="b7f08-119">管理者アプリの割り当てと同意エクスペリエンスに表示されるアクセス許可ヘルプテキスト。</span><span class="sxs-lookup"><span data-stu-id="b7f08-119">Permission help text that appears in the admin app assignment and consent experiences.</span></span>|
|<span data-ttu-id="b7f08-120">displayName</span><span class="sxs-lookup"><span data-stu-id="b7f08-120">displayName</span></span>|<span data-ttu-id="b7f08-121">String</span><span class="sxs-lookup"><span data-stu-id="b7f08-121">String</span></span>|<span data-ttu-id="b7f08-122">管理者の同意とアプリの割り当てエクスペリエンスに表示されるアクセス許可の表示名。</span><span class="sxs-lookup"><span data-stu-id="b7f08-122">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="b7f08-123">id</span><span class="sxs-lookup"><span data-stu-id="b7f08-123">id</span></span>|<span data-ttu-id="b7f08-124">Guid</span><span class="sxs-lookup"><span data-stu-id="b7f08-124">Guid</span></span>|<span data-ttu-id="b7f08-125">Approles コレクション内の\*\*\*\* 一意のロール識別子。</span><span class="sxs-lookup"><span data-stu-id="b7f08-125">Unique role identifier inside the **appRoles** collection.</span></span> <span data-ttu-id="b7f08-126">新しいアプリの役割を作成する場合は、新しい Guid 識別子を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b7f08-126">When creating a new app role, a new Guid identifier must be provided.</span></span> |
|<span data-ttu-id="b7f08-127">isEnabled</span><span class="sxs-lookup"><span data-stu-id="b7f08-127">isEnabled</span></span>|<span data-ttu-id="b7f08-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7f08-128">Boolean</span></span>|<span data-ttu-id="b7f08-129">アプリの役割を作成または更新する場合は、 **true** (既定値) に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b7f08-129">When creating or updating an app role, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="b7f08-130">役割を削除するには、最初に**false**に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b7f08-130">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="b7f08-131">その時点で、以降の呼び出しでは、この役割が削除される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="b7f08-131">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="b7f08-132">戻す</span><span class="sxs-lookup"><span data-stu-id="b7f08-132">origin</span></span>|<span data-ttu-id="b7f08-133">String</span><span class="sxs-lookup"><span data-stu-id="b7f08-133">String</span></span>| <span data-ttu-id="b7f08-134">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7f08-134">Read-only.</span></span> <span data-ttu-id="b7f08-135">アプリケーションオブジェクトまたは ServicePrincipal オブジェクトでアプリの役割が定義されているかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b7f08-135">Specifies if the app role is defined on the Application object or on the ServicePrincipal object.</span></span> <span data-ttu-id="b7f08-136">POST または PATCH 要求に含まれていてはなり_ません_。</span><span class="sxs-lookup"><span data-stu-id="b7f08-136">Must _not_ be included in any POST or PATCH requests.</span></span> |
|<span data-ttu-id="b7f08-137">value</span><span class="sxs-lookup"><span data-stu-id="b7f08-137">value</span></span>|<span data-ttu-id="b7f08-138">文字列</span><span class="sxs-lookup"><span data-stu-id="b7f08-138">String</span></span>|<span data-ttu-id="b7f08-139">認証とアクセストークンで`roles`クレームに含める値を指定します。</span><span class="sxs-lookup"><span data-stu-id="b7f08-139">Specifies the value which will be included in the `roles` claim in authentication and access tokens.</span></span> <span data-ttu-id="b7f08-140">長さが120文字を超えることはできません。</span><span class="sxs-lookup"><span data-stu-id="b7f08-140">Must not exceed 120 characters in length.</span></span> <span data-ttu-id="b7f08-141">許可される`:` `!` `#` `$` `%`文字`&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `0-9`内`A-Z`の文字、 `a-z`および。 `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`</span><span class="sxs-lookup"><span data-stu-id="b7f08-141">Allowed characters are `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`, as well as characters in the ranges `0-9`, `A-Z` and `a-z`.</span></span> <span data-ttu-id="b7f08-142">スペース文字を含むその他の文字は使用できません。</span><span class="sxs-lookup"><span data-stu-id="b7f08-142">Any other character, including the space character, are not allowed.</span></span>  |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
