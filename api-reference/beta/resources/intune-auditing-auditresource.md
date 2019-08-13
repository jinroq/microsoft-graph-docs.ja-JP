---
title: auditResource リソースの種類
description: 監査のリソースのプロパティが含まれるクラス。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a390f43daca9d86320eea29eb139406ad52476fe
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335222"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="79d88-103">auditResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="79d88-103">auditResource resource type</span></span>

> <span data-ttu-id="79d88-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79d88-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79d88-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="79d88-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79d88-106">監査のリソースのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="79d88-106">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="79d88-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79d88-107">Properties</span></span>
|<span data-ttu-id="79d88-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79d88-108">Property</span></span>|<span data-ttu-id="79d88-109">型</span><span class="sxs-lookup"><span data-stu-id="79d88-109">Type</span></span>|<span data-ttu-id="79d88-110">説明</span><span class="sxs-lookup"><span data-stu-id="79d88-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79d88-111">displayName</span><span class="sxs-lookup"><span data-stu-id="79d88-111">displayName</span></span>|<span data-ttu-id="79d88-112">文字列</span><span class="sxs-lookup"><span data-stu-id="79d88-112">String</span></span>|<span data-ttu-id="79d88-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="79d88-113">Display name.</span></span>|
|<span data-ttu-id="79d88-114">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="79d88-114">modifiedProperties</span></span>|<span data-ttu-id="79d88-115">[auditProperty](../resources/intune-auditing-auditproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="79d88-115">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="79d88-116">変更されたプロパティの一覧。</span><span class="sxs-lookup"><span data-stu-id="79d88-116">List of modified properties.</span></span>|
|<span data-ttu-id="79d88-117">type</span><span class="sxs-lookup"><span data-stu-id="79d88-117">type</span></span>|<span data-ttu-id="79d88-118">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="79d88-118">String</span></span>|<span data-ttu-id="79d88-119">監査のリソースの種類。</span><span class="sxs-lookup"><span data-stu-id="79d88-119">Audit resource's type.</span></span>|
|<span data-ttu-id="79d88-120">resourceId</span><span class="sxs-lookup"><span data-stu-id="79d88-120">resourceId</span></span>|<span data-ttu-id="79d88-121">String</span><span class="sxs-lookup"><span data-stu-id="79d88-121">String</span></span>|<span data-ttu-id="79d88-122">監査のリソースの ID。</span><span class="sxs-lookup"><span data-stu-id="79d88-122">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="79d88-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="79d88-123">Relationships</span></span>
<span data-ttu-id="79d88-124">なし</span><span class="sxs-lookup"><span data-stu-id="79d88-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="79d88-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="79d88-125">JSON Representation</span></span>
<span data-ttu-id="79d88-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="79d88-126">Here is a JSON representation of the resource.</span></span>
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



