---
title: omaSettingString リソースの種類
description: OMA 設定の文字列の定義です。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dc59c22933b888227678db70d9a48d601d699a8e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990247"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="72784-103">omaSettingString リソースの種類</span><span class="sxs-lookup"><span data-stu-id="72784-103">omaSettingString resource type</span></span>

> <span data-ttu-id="72784-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="72784-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72784-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="72784-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72784-106">OMA 設定の文字列の定義です。</span><span class="sxs-lookup"><span data-stu-id="72784-106">OMA Settings String definition.</span></span>


<span data-ttu-id="72784-107">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="72784-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="72784-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="72784-108">Properties</span></span>
|<span data-ttu-id="72784-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="72784-109">Property</span></span>|<span data-ttu-id="72784-110">型</span><span class="sxs-lookup"><span data-stu-id="72784-110">Type</span></span>|<span data-ttu-id="72784-111">説明</span><span class="sxs-lookup"><span data-stu-id="72784-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72784-112">displayName</span><span class="sxs-lookup"><span data-stu-id="72784-112">displayName</span></span>|<span data-ttu-id="72784-113">String</span><span class="sxs-lookup"><span data-stu-id="72784-113">String</span></span>|<span data-ttu-id="72784-114">表示名。</span><span class="sxs-lookup"><span data-stu-id="72784-114">Display Name.</span></span> <span data-ttu-id="72784-115">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="72784-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="72784-116">description</span><span class="sxs-lookup"><span data-stu-id="72784-116">description</span></span>|<span data-ttu-id="72784-117">String</span><span class="sxs-lookup"><span data-stu-id="72784-117">String</span></span>|<span data-ttu-id="72784-118">説明。</span><span class="sxs-lookup"><span data-stu-id="72784-118">Description.</span></span> <span data-ttu-id="72784-119">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="72784-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="72784-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="72784-120">omaUri</span></span>|<span data-ttu-id="72784-121">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="72784-121">String</span></span>|<span data-ttu-id="72784-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="72784-122">OMA.</span></span> <span data-ttu-id="72784-123">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="72784-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="72784-124">value</span><span class="sxs-lookup"><span data-stu-id="72784-124">value</span></span>|<span data-ttu-id="72784-125">文字列</span><span class="sxs-lookup"><span data-stu-id="72784-125">String</span></span>|<span data-ttu-id="72784-126">値。</span><span class="sxs-lookup"><span data-stu-id="72784-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72784-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="72784-127">Relationships</span></span>
<span data-ttu-id="72784-128">なし</span><span class="sxs-lookup"><span data-stu-id="72784-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="72784-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="72784-129">JSON Representation</span></span>
<span data-ttu-id="72784-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="72784-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String"
}
```





