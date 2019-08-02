---
title: appIdentity リソースの種類
description: アクションを実行した、または変更されたアプリケーションの id を示します。 アプリケーション Id、名前、サービスプリンシパル ID、名前が含まれます。 このリソースは、directoryAudit API によって呼び出されます。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3a8b2c9185f595bf4ab534dda5a73b1a5f40fd17
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030094"
---
# <a name="appidentity-resource-type"></a><span data-ttu-id="24be0-105">appIdentity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="24be0-105">appIdentity resource type</span></span>

<span data-ttu-id="24be0-106">アクションを実行した、または変更されたアプリケーションの id を示します。</span><span class="sxs-lookup"><span data-stu-id="24be0-106">Indicates the identity of the application that performed the action or was changed.</span></span> <span data-ttu-id="24be0-107">アプリケーション ID、名前、およびサービスプリンシパル ID と名前が含まれます。</span><span class="sxs-lookup"><span data-stu-id="24be0-107">Includes application ID, name, and service principal ID and name.</span></span> <span data-ttu-id="24be0-108">このリソースは、 [Get directoryAudit](../api/directoryaudit-get.md)操作で使用されます。</span><span class="sxs-lookup"><span data-stu-id="24be0-108">This resource is used by the [Get directoryAudit](../api/directoryaudit-get.md) operation.</span></span>

## <a name="properties"></a><span data-ttu-id="24be0-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24be0-109">Properties</span></span>

| <span data-ttu-id="24be0-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24be0-110">Property</span></span>     | <span data-ttu-id="24be0-111">型</span><span class="sxs-lookup"><span data-stu-id="24be0-111">Type</span></span>   |<span data-ttu-id="24be0-112">説明</span><span class="sxs-lookup"><span data-stu-id="24be0-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24be0-113">appId</span><span class="sxs-lookup"><span data-stu-id="24be0-113">appId</span></span>|<span data-ttu-id="24be0-114">String</span><span class="sxs-lookup"><span data-stu-id="24be0-114">String</span></span>|<span data-ttu-id="24be0-115">Azure Active Directory でのアプリケーション ID を表す一意の GUID を参照します。</span><span class="sxs-lookup"><span data-stu-id="24be0-115">Refers to the Unique GUID representing Application Id in the Azure Active Directory.</span></span>|
|<span data-ttu-id="24be0-116">displayName</span><span class="sxs-lookup"><span data-stu-id="24be0-116">displayName</span></span>|<span data-ttu-id="24be0-117">文字列</span><span class="sxs-lookup"><span data-stu-id="24be0-117">String</span></span>|<span data-ttu-id="24be0-118">Azure Portal に表示されるアプリケーション名を参照します。</span><span class="sxs-lookup"><span data-stu-id="24be0-118">Refers to the Application Name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="24be0-119">servicePrincipalId</span><span class="sxs-lookup"><span data-stu-id="24be0-119">servicePrincipalId</span></span>|<span data-ttu-id="24be0-120">String</span><span class="sxs-lookup"><span data-stu-id="24be0-120">String</span></span>|<span data-ttu-id="24be0-121">対応するアプリの Azure Active Directory でサービスプリンシパル Id を示す一意の GUID を参照します。</span><span class="sxs-lookup"><span data-stu-id="24be0-121">Refers to the Unique GUID indicating Service Principal Id in Azure Active Directory for the corresponding App.</span></span>|
|<span data-ttu-id="24be0-122">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="24be0-122">servicePrincipalName</span></span>|<span data-ttu-id="24be0-123">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="24be0-123">String</span></span>|<span data-ttu-id="24be0-124">サービスプリンシパル名がテナント内のアプリケーション名であることを示します。</span><span class="sxs-lookup"><span data-stu-id="24be0-124">Refers to the Service Principal Name is the Application name in the tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="24be0-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="24be0-125">JSON representation</span></span>

<span data-ttu-id="24be0-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="24be0-126">Here is a JSON representation of the resource.</span></span>

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
