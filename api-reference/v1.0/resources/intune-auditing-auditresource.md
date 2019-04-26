---
title: auditResource リソースの種類
description: 監査のリソースのプロパティが含まれるクラス。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9e2a6b2309e831a872c4cde04a951819cac292ec
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534347"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="a3f9f-103">auditResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a3f9f-103">auditResource resource type</span></span>

> <span data-ttu-id="a3f9f-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a3f9f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3f9f-105">監査のリソースのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="a3f9f-105">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="a3f9f-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a3f9f-106">Properties</span></span>
|<span data-ttu-id="a3f9f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a3f9f-107">Property</span></span>|<span data-ttu-id="a3f9f-108">型</span><span class="sxs-lookup"><span data-stu-id="a3f9f-108">Type</span></span>|<span data-ttu-id="a3f9f-109">説明</span><span class="sxs-lookup"><span data-stu-id="a3f9f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3f9f-110">displayName</span><span class="sxs-lookup"><span data-stu-id="a3f9f-110">displayName</span></span>|<span data-ttu-id="a3f9f-111">String</span><span class="sxs-lookup"><span data-stu-id="a3f9f-111">String</span></span>|<span data-ttu-id="a3f9f-112">表示名。</span><span class="sxs-lookup"><span data-stu-id="a3f9f-112">Display name.</span></span>|
|<span data-ttu-id="a3f9f-113">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="a3f9f-113">modifiedProperties</span></span>|<span data-ttu-id="a3f9f-114">[auditProperty](../resources/intune-auditing-auditproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a3f9f-114">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="a3f9f-115">変更されたプロパティの一覧。</span><span class="sxs-lookup"><span data-stu-id="a3f9f-115">List of modified properties.</span></span>|
|<span data-ttu-id="a3f9f-116">type</span><span class="sxs-lookup"><span data-stu-id="a3f9f-116">type</span></span>|<span data-ttu-id="a3f9f-117">String</span><span class="sxs-lookup"><span data-stu-id="a3f9f-117">String</span></span>|<span data-ttu-id="a3f9f-118">監査のリソースの種類。</span><span class="sxs-lookup"><span data-stu-id="a3f9f-118">Audit resource's type.</span></span>|
|<span data-ttu-id="a3f9f-119">resourceId</span><span class="sxs-lookup"><span data-stu-id="a3f9f-119">resourceId</span></span>|<span data-ttu-id="a3f9f-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="a3f9f-120">String</span></span>|<span data-ttu-id="a3f9f-121">監査のリソースの ID。</span><span class="sxs-lookup"><span data-stu-id="a3f9f-121">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3f9f-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a3f9f-122">Relationships</span></span>
<span data-ttu-id="a3f9f-123">なし</span><span class="sxs-lookup"><span data-stu-id="a3f9f-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3f9f-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a3f9f-124">JSON Representation</span></span>
<span data-ttu-id="a3f9f-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a3f9f-125">Here is a JSON representation of the resource.</span></span>
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



