---
title: appIdentity リソースの種類
description: アクションを実行するか、変更されているアプリケーションの id を示します。 アプリケーション Id、名、サービス ・ プリンシパルの ID および名前が含まれています。 このリソースは、directoryAudit API によって呼び出されます。
localization_priority: Normal
ms.openlocfilehash: ec61782fca0ab4004fab5a55bd4774c0d64afb3a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855784"
---
# <a name="appidentity-resource-type"></a><span data-ttu-id="42bd7-105">appIdentity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="42bd7-105">appIdentity resource type</span></span>
<span data-ttu-id="42bd7-106">アクションを実行するか、変更されているアプリケーションの id を示します。</span><span class="sxs-lookup"><span data-stu-id="42bd7-106">Indicates the identity of the application that performed the action or was changed.</span></span> <span data-ttu-id="42bd7-107">アプリケーション Id、名、サービス ・ プリンシパルの ID および名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="42bd7-107">Includes Application Id, Name, Service Principal ID and Name.</span></span> <span data-ttu-id="42bd7-108">このリソースは、 [directoryAudit](../api/directoryaudit-get.md) API によって呼び出されます。</span><span class="sxs-lookup"><span data-stu-id="42bd7-108">This resource is called by the [directoryAudit](../api/directoryaudit-get.md) API</span></span>


## <a name="properties"></a><span data-ttu-id="42bd7-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42bd7-109">Properties</span></span>
| <span data-ttu-id="42bd7-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42bd7-110">Property</span></span>     | <span data-ttu-id="42bd7-111">種類</span><span class="sxs-lookup"><span data-stu-id="42bd7-111">Type</span></span>   |<span data-ttu-id="42bd7-112">説明</span><span class="sxs-lookup"><span data-stu-id="42bd7-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42bd7-113">appId</span><span class="sxs-lookup"><span data-stu-id="42bd7-113">appId</span></span>|<span data-ttu-id="42bd7-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="42bd7-114">String</span></span>|<span data-ttu-id="42bd7-115">Azure Active Directory 内のアプリケーションの Id を表す一意の GUID を参照します。</span><span class="sxs-lookup"><span data-stu-id="42bd7-115">Refers to the Unique GUID representing Application Id in the Azure Active Directory.</span></span>|
|<span data-ttu-id="42bd7-116">displayName</span><span class="sxs-lookup"><span data-stu-id="42bd7-116">displayName</span></span>|<span data-ttu-id="42bd7-117">String</span><span class="sxs-lookup"><span data-stu-id="42bd7-117">String</span></span>|<span data-ttu-id="42bd7-118">Azure ポータルに表示されるアプリケーション名を参照します。</span><span class="sxs-lookup"><span data-stu-id="42bd7-118">Refers to the Application Name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="42bd7-119">servicePrincipalId</span><span class="sxs-lookup"><span data-stu-id="42bd7-119">servicePrincipalId</span></span>|<span data-ttu-id="42bd7-120">String</span><span class="sxs-lookup"><span data-stu-id="42bd7-120">String</span></span>|<span data-ttu-id="42bd7-121">Azure Active Directory 内のサービス ・ プリンシパルの Id を対応するアプリケーションを示す一意の GUID を参照します。</span><span class="sxs-lookup"><span data-stu-id="42bd7-121">Refers to the Unique GUID indicating Service Principal Id in Azure Active Directory for the corresponding App.</span></span>|
|<span data-ttu-id="42bd7-122">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="42bd7-122">servicePrincipalName</span></span>|<span data-ttu-id="42bd7-123">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="42bd7-123">String</span></span>|<span data-ttu-id="42bd7-124">参照して、サービス プリンシパル名は、テナントにアプリケーションの名前です。</span><span class="sxs-lookup"><span data-stu-id="42bd7-124">Refers to the Service Principal Name is the Application name in the tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="42bd7-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="42bd7-125">JSON representation</span></span>

<span data-ttu-id="42bd7-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="42bd7-126">Here is a JSON representation of the resource.</span></span>

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
