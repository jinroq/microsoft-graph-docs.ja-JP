---
title: auditResource リソースの種類
description: 監査のリソースのプロパティが含まれるクラス。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bba8aa9cfe10d17cefdcfe28d25c4d8c2dfa429f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412479"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="c1ac0-103">auditResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c1ac0-103">auditResource resource type</span></span>

> <span data-ttu-id="c1ac0-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c1ac0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c1ac0-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c1ac0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1ac0-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c1ac0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1ac0-107">監査のリソースのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="c1ac0-107">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="c1ac0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1ac0-108">Properties</span></span>
|<span data-ttu-id="c1ac0-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1ac0-109">Property</span></span>|<span data-ttu-id="c1ac0-110">型</span><span class="sxs-lookup"><span data-stu-id="c1ac0-110">Type</span></span>|<span data-ttu-id="c1ac0-111">説明</span><span class="sxs-lookup"><span data-stu-id="c1ac0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1ac0-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c1ac0-112">displayName</span></span>|<span data-ttu-id="c1ac0-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c1ac0-113">String</span></span>|<span data-ttu-id="c1ac0-114">表示名。</span><span class="sxs-lookup"><span data-stu-id="c1ac0-114">Display name.</span></span>|
|<span data-ttu-id="c1ac0-115">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="c1ac0-115">modifiedProperties</span></span>|<span data-ttu-id="c1ac0-116">[auditProperty](../resources/intune-auditing-auditproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c1ac0-116">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="c1ac0-117">変更されたプロパティの一覧。</span><span class="sxs-lookup"><span data-stu-id="c1ac0-117">List of modified properties.</span></span>|
|<span data-ttu-id="c1ac0-118">type</span><span class="sxs-lookup"><span data-stu-id="c1ac0-118">type</span></span>|<span data-ttu-id="c1ac0-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c1ac0-119">String</span></span>|<span data-ttu-id="c1ac0-120">監査のリソースの種類。</span><span class="sxs-lookup"><span data-stu-id="c1ac0-120">Audit resource's type.</span></span>|
|<span data-ttu-id="c1ac0-121">resourceId</span><span class="sxs-lookup"><span data-stu-id="c1ac0-121">resourceId</span></span>|<span data-ttu-id="c1ac0-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c1ac0-122">String</span></span>|<span data-ttu-id="c1ac0-123">監査のリソースの ID。</span><span class="sxs-lookup"><span data-stu-id="c1ac0-123">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1ac0-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c1ac0-124">Relationships</span></span>
<span data-ttu-id="c1ac0-125">なし</span><span class="sxs-lookup"><span data-stu-id="c1ac0-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1ac0-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c1ac0-126">JSON Representation</span></span>
<span data-ttu-id="c1ac0-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c1ac0-127">Here is a JSON representation of the resource.</span></span>
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




