---
title: deviceManagementSettingComparison リソースの種類
description: 比較結果の設定を表すエンティティ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f68ffd08945662fc291fb5489de67967d3cd1cbf
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002001"
---
# <a name="devicemanagementsettingcomparison-resource-type"></a><span data-ttu-id="cc272-103">deviceManagementSettingComparison リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cc272-103">deviceManagementSettingComparison resource type</span></span>

> <span data-ttu-id="cc272-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc272-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc272-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cc272-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc272-106">比較結果の設定を表すエンティティ</span><span class="sxs-lookup"><span data-stu-id="cc272-106">Entity representing setting comparison result</span></span>

## <a name="properties"></a><span data-ttu-id="cc272-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc272-107">Properties</span></span>
|<span data-ttu-id="cc272-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc272-108">Property</span></span>|<span data-ttu-id="cc272-109">型</span><span class="sxs-lookup"><span data-stu-id="cc272-109">Type</span></span>|<span data-ttu-id="cc272-110">説明</span><span class="sxs-lookup"><span data-stu-id="cc272-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc272-111">id</span><span class="sxs-lookup"><span data-stu-id="cc272-111">id</span></span>|<span data-ttu-id="cc272-112">文字列</span><span class="sxs-lookup"><span data-stu-id="cc272-112">String</span></span>|<span data-ttu-id="cc272-113">設定 ID</span><span class="sxs-lookup"><span data-stu-id="cc272-113">The setting ID</span></span>|
|<span data-ttu-id="cc272-114">displayName</span><span class="sxs-lookup"><span data-stu-id="cc272-114">displayName</span></span>|<span data-ttu-id="cc272-115">String</span><span class="sxs-lookup"><span data-stu-id="cc272-115">String</span></span>|<span data-ttu-id="cc272-116">設定の表示名</span><span class="sxs-lookup"><span data-stu-id="cc272-116">The setting's display name</span></span>|
|<span data-ttu-id="cc272-117">definitionId</span><span class="sxs-lookup"><span data-stu-id="cc272-117">definitionId</span></span>|<span data-ttu-id="cc272-118">String</span><span class="sxs-lookup"><span data-stu-id="cc272-118">String</span></span>|<span data-ttu-id="cc272-119">このインスタンスの設定定義の ID</span><span class="sxs-lookup"><span data-stu-id="cc272-119">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="cc272-120">currentValueJson</span><span class="sxs-lookup"><span data-stu-id="cc272-120">currentValueJson</span></span>|<span data-ttu-id="cc272-121">String</span><span class="sxs-lookup"><span data-stu-id="cc272-121">String</span></span>|<span data-ttu-id="cc272-122">現在のインテント (または) テンプレート設定の値の JSON 表現</span><span class="sxs-lookup"><span data-stu-id="cc272-122">JSON representation of current intent (or) template setting's value</span></span>|
|<span data-ttu-id="cc272-123">newValueJson</span><span class="sxs-lookup"><span data-stu-id="cc272-123">newValueJson</span></span>|<span data-ttu-id="cc272-124">String</span><span class="sxs-lookup"><span data-stu-id="cc272-124">String</span></span>|<span data-ttu-id="cc272-125">新しいテンプレート設定の値の JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cc272-125">JSON representation of new template setting's value</span></span>|
|<span data-ttu-id="cc272-126">comparisonResult</span><span class="sxs-lookup"><span data-stu-id="cc272-126">comparisonResult</span></span>|[<span data-ttu-id="cc272-127">deviceManagementComparisonResult</span><span class="sxs-lookup"><span data-stu-id="cc272-127">deviceManagementComparisonResult</span></span>](../resources/intune-deviceintent-devicemanagementcomparisonresult.md)|<span data-ttu-id="cc272-128">比較結果を設定します。</span><span class="sxs-lookup"><span data-stu-id="cc272-128">Setting comparison result.</span></span> <span data-ttu-id="cc272-129">可能な値は、`unknown`、`equal`、`notEqual`、`added`、`removed` です。</span><span class="sxs-lookup"><span data-stu-id="cc272-129">Possible values are: `unknown`, `equal`, `notEqual`, `added`, `removed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc272-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cc272-130">Relationships</span></span>
<span data-ttu-id="cc272-131">なし</span><span class="sxs-lookup"><span data-stu-id="cc272-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc272-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cc272-132">JSON Representation</span></span>
<span data-ttu-id="cc272-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cc272-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingComparison"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingComparison",
  "id": "String (identifier)",
  "displayName": "String",
  "definitionId": "String",
  "currentValueJson": "String",
  "newValueJson": "String",
  "comparisonResult": "String"
}
```





