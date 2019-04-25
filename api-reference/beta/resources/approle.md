---
title: approle リソースの種類
description: 別のアプリケーションを呼び出しているクライアントアプリケーションによって要求されるか、または指定されたアプリケーションロールのユーザーまたはグループにアプリケーションを割り当てるために使用される可能性があるアプリケーションロールを表します。 serviceprincipal エンティティおよび application エンティティの**approles**プロパティは、 **approles**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: 8a367406c64cf9d0d3da49716aeaf6ca3c1fa687
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535705"
---
# <a name="approle-resource-type"></a><span data-ttu-id="3c349-104">approle リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3c349-104">appRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c349-105">別のアプリケーションを呼び出しているクライアントアプリケーションによって要求されるか、または指定されたアプリケーションロールのユーザーまたはグループにアプリケーションを割り当てるために使用される可能性があるアプリケーションロールを表します。</span><span class="sxs-lookup"><span data-stu-id="3c349-105">Represents an application role that may be requested by a client application calling another application or that may be used to assign an application to users or groups in a specified application role.</span></span> <span data-ttu-id="3c349-106">[serviceprincipal](serviceprincipal.md)エンティティおよび[application](application.md)エンティティの**approles**プロパティは、 **approles**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="3c349-106">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **appRole**.</span></span>

> <span data-ttu-id="3c349-107">重要: この機能は現在のリリースでは無効になっています。</span><span class="sxs-lookup"><span data-stu-id="3c349-107">Important: This functionality is disabled in the current release.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c349-108">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3c349-108">JSON representation</span></span>

<span data-ttu-id="3c349-109">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="3c349-109">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="3c349-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3c349-110">Properties</span></span>
| <span data-ttu-id="3c349-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3c349-111">Property</span></span>     | <span data-ttu-id="3c349-112">型</span><span class="sxs-lookup"><span data-stu-id="3c349-112">Type</span></span>   |<span data-ttu-id="3c349-113">説明</span><span class="sxs-lookup"><span data-stu-id="3c349-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c349-114">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="3c349-114">allowedMemberTypes</span></span>|<span data-ttu-id="3c349-115">String collection</span><span class="sxs-lookup"><span data-stu-id="3c349-115">String collection</span></span>|<span data-ttu-id="3c349-116">"application" に設定するか、またはその両方に設定して、このアプリの役割定義をユーザーとグループに割り当てることができるようにするかどうかを指定します。 "User" に設定するか、または (デーモンサービスシナリオでこのアプリケーションにアクセスしている) 他のアプリケーションに割り当てます。</span><span class="sxs-lookup"><span data-stu-id="3c349-116">Specifies whether this app role definition can be assigned to users and groups by setting to “User”, or to other applications (that are accessing this application in daemon service scenarios) by setting to “Application”, or to both.</span></span>|
|<span data-ttu-id="3c349-117">description</span><span class="sxs-lookup"><span data-stu-id="3c349-117">description</span></span>|<span data-ttu-id="3c349-118">String</span><span class="sxs-lookup"><span data-stu-id="3c349-118">String</span></span>|<span data-ttu-id="3c349-119">管理者アプリの割り当てと同意エクスペリエンスに表示されるアクセス許可ヘルプテキスト。</span><span class="sxs-lookup"><span data-stu-id="3c349-119">Permission help text that appears in the admin app assignment and consent experiences.</span></span>|
|<span data-ttu-id="3c349-120">displayName</span><span class="sxs-lookup"><span data-stu-id="3c349-120">displayName</span></span>|<span data-ttu-id="3c349-121">String</span><span class="sxs-lookup"><span data-stu-id="3c349-121">String</span></span>|<span data-ttu-id="3c349-122">管理者の同意とアプリの割り当てエクスペリエンスに表示されるアクセス許可の表示名。</span><span class="sxs-lookup"><span data-stu-id="3c349-122">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="3c349-123">id</span><span class="sxs-lookup"><span data-stu-id="3c349-123">id</span></span>|<span data-ttu-id="3c349-124">Guid</span><span class="sxs-lookup"><span data-stu-id="3c349-124">Guid</span></span>|<span data-ttu-id="3c349-125">approles コレクション内の\*\*\*\* 一意のロール識別子。</span><span class="sxs-lookup"><span data-stu-id="3c349-125">Unique role identifier inside the **appRoles** collection.</span></span>|
|<span data-ttu-id="3c349-126">isEnabled</span><span class="sxs-lookup"><span data-stu-id="3c349-126">isEnabled</span></span>|<span data-ttu-id="3c349-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c349-127">Boolean</span></span>|<span data-ttu-id="3c349-128">ロール定義を作成または更新する場合は、 **true** (既定値) に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3c349-128">When creating or updating a role definition, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="3c349-129">役割を削除するには、最初に**false**に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3c349-129">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="3c349-130">その時点で、以降の呼び出しでは、この役割が削除される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="3c349-130">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="3c349-131">value</span><span class="sxs-lookup"><span data-stu-id="3c349-131">value</span></span>|<span data-ttu-id="3c349-132">文字列</span><span class="sxs-lookup"><span data-stu-id="3c349-132">String</span></span>|<span data-ttu-id="3c349-133">アプリケーションが認証トークンとアクセストークンで想定する必要があるロール要求の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="3c349-133">Specifies the value of the roles claim that the application should expect in the authentication and access tokens.</span></span>|

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
