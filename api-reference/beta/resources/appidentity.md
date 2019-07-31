---
title: appIdentity リソースの種類
description: アクションを実行した、または変更されたアプリケーションの id を示します。 アプリケーション Id、名前、サービスプリンシパル ID、名前が含まれます。 このリソースは、directoryAudit API によって呼び出されます。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 63cb9ed2fbbf9487af1e4d523a04defb7c78cb9e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974319"
---
# <a name="appidentity-resource-type"></a><span data-ttu-id="e16d8-105">appIdentity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e16d8-105">appIdentity resource type</span></span>
<span data-ttu-id="e16d8-106">アクションを実行した、または変更されたアプリケーションの id を示します。</span><span class="sxs-lookup"><span data-stu-id="e16d8-106">Indicates the identity of the application that performed the action or was changed.</span></span> <span data-ttu-id="e16d8-107">アプリケーション Id、名前、サービスプリンシパル ID、名前が含まれます。</span><span class="sxs-lookup"><span data-stu-id="e16d8-107">Includes Application Id, Name, Service Principal ID and Name.</span></span> <span data-ttu-id="e16d8-108">このリソースは、 [Directoryaudit](../api/directoryaudit-get.md) API によって呼び出されます。</span><span class="sxs-lookup"><span data-stu-id="e16d8-108">This resource is called by the [directoryAudit](../api/directoryaudit-get.md) API</span></span>


## <a name="properties"></a><span data-ttu-id="e16d8-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e16d8-109">Properties</span></span>
| <span data-ttu-id="e16d8-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e16d8-110">Property</span></span>     | <span data-ttu-id="e16d8-111">型</span><span class="sxs-lookup"><span data-stu-id="e16d8-111">Type</span></span>   |<span data-ttu-id="e16d8-112">説明</span><span class="sxs-lookup"><span data-stu-id="e16d8-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e16d8-113">appId</span><span class="sxs-lookup"><span data-stu-id="e16d8-113">appId</span></span>|<span data-ttu-id="e16d8-114">String</span><span class="sxs-lookup"><span data-stu-id="e16d8-114">String</span></span>|<span data-ttu-id="e16d8-115">Azure Active Directory でのアプリケーション ID を表す一意の GUID を参照します。</span><span class="sxs-lookup"><span data-stu-id="e16d8-115">Refers to the Unique GUID representing Application Id in the Azure Active Directory.</span></span>|
|<span data-ttu-id="e16d8-116">displayName</span><span class="sxs-lookup"><span data-stu-id="e16d8-116">displayName</span></span>|<span data-ttu-id="e16d8-117">文字列</span><span class="sxs-lookup"><span data-stu-id="e16d8-117">String</span></span>|<span data-ttu-id="e16d8-118">Azure Portal に表示されるアプリケーション名を参照します。</span><span class="sxs-lookup"><span data-stu-id="e16d8-118">Refers to the Application Name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="e16d8-119">servicePrincipalId</span><span class="sxs-lookup"><span data-stu-id="e16d8-119">servicePrincipalId</span></span>|<span data-ttu-id="e16d8-120">String</span><span class="sxs-lookup"><span data-stu-id="e16d8-120">String</span></span>|<span data-ttu-id="e16d8-121">対応するアプリの Azure Active Directory でサービスプリンシパル Id を示す一意の GUID を参照します。</span><span class="sxs-lookup"><span data-stu-id="e16d8-121">Refers to the Unique GUID indicating Service Principal Id in Azure Active Directory for the corresponding App.</span></span>|
|<span data-ttu-id="e16d8-122">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="e16d8-122">servicePrincipalName</span></span>|<span data-ttu-id="e16d8-123">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e16d8-123">String</span></span>|<span data-ttu-id="e16d8-124">サービスプリンシパル名がテナント内のアプリケーション名であることを示します。</span><span class="sxs-lookup"><span data-stu-id="e16d8-124">Refers to the Service Principal Name is the Application name in the tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e16d8-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e16d8-125">JSON representation</span></span>

<span data-ttu-id="e16d8-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e16d8-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appIdentity"
}-->

```json
{
  "appId": "String",
  "displayName": "String",
  "servicePrincipalId": "String",
  "servicePrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
