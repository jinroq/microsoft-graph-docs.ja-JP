---
title: appidentity リソースの種類
description: アクションを実行した、または変更されたアプリケーションの id を示します。 アプリケーション Id、名前、サービスプリンシパル Id、名前が含まれます。 このリソースは、directoryaudit API によって呼び出されます。
localization_priority: Normal
ms.openlocfilehash: ec61782fca0ab4004fab5a55bd4774c0d64afb3a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535677"
---
# <a name="appidentity-resource-type"></a><span data-ttu-id="1d394-105">appidentity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1d394-105">appIdentity resource type</span></span>
<span data-ttu-id="1d394-106">アクションを実行した、または変更されたアプリケーションの id を示します。</span><span class="sxs-lookup"><span data-stu-id="1d394-106">Indicates the identity of the application that performed the action or was changed.</span></span> <span data-ttu-id="1d394-107">アプリケーション Id、名前、サービスプリンシパル Id、名前が含まれます。</span><span class="sxs-lookup"><span data-stu-id="1d394-107">Includes Application Id, Name, Service Principal ID and Name.</span></span> <span data-ttu-id="1d394-108">このリソースは、 [directoryaudit](../api/directoryaudit-get.md) API によって呼び出されます。</span><span class="sxs-lookup"><span data-stu-id="1d394-108">This resource is called by the [directoryAudit](../api/directoryaudit-get.md) API</span></span>


## <a name="properties"></a><span data-ttu-id="1d394-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d394-109">Properties</span></span>
| <span data-ttu-id="1d394-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d394-110">Property</span></span>     | <span data-ttu-id="1d394-111">型</span><span class="sxs-lookup"><span data-stu-id="1d394-111">Type</span></span>   |<span data-ttu-id="1d394-112">説明</span><span class="sxs-lookup"><span data-stu-id="1d394-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d394-113">appId</span><span class="sxs-lookup"><span data-stu-id="1d394-113">appId</span></span>|<span data-ttu-id="1d394-114">String</span><span class="sxs-lookup"><span data-stu-id="1d394-114">String</span></span>|<span data-ttu-id="1d394-115">Azure Active Directory でのアプリケーション ID を表す一意の GUID を参照します。</span><span class="sxs-lookup"><span data-stu-id="1d394-115">Refers to the Unique GUID representing Application Id in the Azure Active Directory.</span></span>|
|<span data-ttu-id="1d394-116">displayName</span><span class="sxs-lookup"><span data-stu-id="1d394-116">displayName</span></span>|<span data-ttu-id="1d394-117">String</span><span class="sxs-lookup"><span data-stu-id="1d394-117">String</span></span>|<span data-ttu-id="1d394-118">Azure Portal に表示されるアプリケーション名を参照します。</span><span class="sxs-lookup"><span data-stu-id="1d394-118">Refers to the Application Name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="1d394-119">servicePrincipalId</span><span class="sxs-lookup"><span data-stu-id="1d394-119">servicePrincipalId</span></span>|<span data-ttu-id="1d394-120">String</span><span class="sxs-lookup"><span data-stu-id="1d394-120">String</span></span>|<span data-ttu-id="1d394-121">対応するアプリの Azure Active Directory でサービスプリンシパル Id を示す一意の GUID を参照します。</span><span class="sxs-lookup"><span data-stu-id="1d394-121">Refers to the Unique GUID indicating Service Principal Id in Azure Active Directory for the corresponding App.</span></span>|
|<span data-ttu-id="1d394-122">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="1d394-122">servicePrincipalName</span></span>|<span data-ttu-id="1d394-123">String</span><span class="sxs-lookup"><span data-stu-id="1d394-123">String</span></span>|<span data-ttu-id="1d394-124">サービスプリンシパル名がテナント内のアプリケーション名であることを示します。</span><span class="sxs-lookup"><span data-stu-id="1d394-124">Refers to the Service Principal Name is the Application name in the tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1d394-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1d394-125">JSON representation</span></span>

<span data-ttu-id="1d394-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1d394-126">Here is a JSON representation of the resource.</span></span>

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
