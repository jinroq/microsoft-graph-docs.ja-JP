---
title: auditResource リソースの種類
description: 監査のリソースのプロパティが含まれるクラス。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 14ecd6e4772e6d694707bd047899bd6b75720252
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028862"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="26910-103">auditResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="26910-103">auditResource resource type</span></span>

> <span data-ttu-id="26910-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="26910-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26910-105">監査のリソースのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="26910-105">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="26910-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26910-106">Properties</span></span>
|<span data-ttu-id="26910-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26910-107">Property</span></span>|<span data-ttu-id="26910-108">型</span><span class="sxs-lookup"><span data-stu-id="26910-108">Type</span></span>|<span data-ttu-id="26910-109">説明</span><span class="sxs-lookup"><span data-stu-id="26910-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26910-110">displayName</span><span class="sxs-lookup"><span data-stu-id="26910-110">displayName</span></span>|<span data-ttu-id="26910-111">文字列</span><span class="sxs-lookup"><span data-stu-id="26910-111">String</span></span>|<span data-ttu-id="26910-112">表示名。</span><span class="sxs-lookup"><span data-stu-id="26910-112">Display name.</span></span>|
|<span data-ttu-id="26910-113">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="26910-113">modifiedProperties</span></span>|<span data-ttu-id="26910-114">[auditProperty](../resources/intune-auditing-auditproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="26910-114">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="26910-115">変更されたプロパティの一覧。</span><span class="sxs-lookup"><span data-stu-id="26910-115">List of modified properties.</span></span>|
|<span data-ttu-id="26910-116">type</span><span class="sxs-lookup"><span data-stu-id="26910-116">type</span></span>|<span data-ttu-id="26910-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="26910-117">String</span></span>|<span data-ttu-id="26910-118">監査のリソースの種類。</span><span class="sxs-lookup"><span data-stu-id="26910-118">Audit resource's type.</span></span>|
|<span data-ttu-id="26910-119">resourceId</span><span class="sxs-lookup"><span data-stu-id="26910-119">resourceId</span></span>|<span data-ttu-id="26910-120">String</span><span class="sxs-lookup"><span data-stu-id="26910-120">String</span></span>|<span data-ttu-id="26910-121">監査のリソースの ID。</span><span class="sxs-lookup"><span data-stu-id="26910-121">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26910-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="26910-122">Relationships</span></span>
<span data-ttu-id="26910-123">なし</span><span class="sxs-lookup"><span data-stu-id="26910-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="26910-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="26910-124">JSON Representation</span></span>
<span data-ttu-id="26910-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="26910-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditResource",
  "displayName": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.auditProperty",
      "displayName": "String",
      "oldValue": "String",
      "newValue": "String"
    }
  ],
  "type": "String",
  "resourceId": "String"
}
```



