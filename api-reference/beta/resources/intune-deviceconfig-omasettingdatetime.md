---
title: omaSettingDateTime リソースの種類
description: OMA 設定の DateTime の定義です。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d4abe8f9b22cdc75e8e560ddb9e15a75425cb3f2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011415"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="2c54e-103">omaSettingDateTime リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2c54e-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="2c54e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2c54e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c54e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2c54e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c54e-106">OMA 設定の DateTime の定義です。</span><span class="sxs-lookup"><span data-stu-id="2c54e-106">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="2c54e-107">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="2c54e-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2c54e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c54e-108">Properties</span></span>
|<span data-ttu-id="2c54e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c54e-109">Property</span></span>|<span data-ttu-id="2c54e-110">型</span><span class="sxs-lookup"><span data-stu-id="2c54e-110">Type</span></span>|<span data-ttu-id="2c54e-111">説明</span><span class="sxs-lookup"><span data-stu-id="2c54e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c54e-112">displayName</span><span class="sxs-lookup"><span data-stu-id="2c54e-112">displayName</span></span>|<span data-ttu-id="2c54e-113">String</span><span class="sxs-lookup"><span data-stu-id="2c54e-113">String</span></span>|<span data-ttu-id="2c54e-114">表示名。</span><span class="sxs-lookup"><span data-stu-id="2c54e-114">Display Name.</span></span> <span data-ttu-id="2c54e-115">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="2c54e-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="2c54e-116">description</span><span class="sxs-lookup"><span data-stu-id="2c54e-116">description</span></span>|<span data-ttu-id="2c54e-117">String</span><span class="sxs-lookup"><span data-stu-id="2c54e-117">String</span></span>|<span data-ttu-id="2c54e-118">説明。</span><span class="sxs-lookup"><span data-stu-id="2c54e-118">Description.</span></span> <span data-ttu-id="2c54e-119">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="2c54e-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="2c54e-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="2c54e-120">omaUri</span></span>|<span data-ttu-id="2c54e-121">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2c54e-121">String</span></span>|<span data-ttu-id="2c54e-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="2c54e-122">OMA.</span></span> <span data-ttu-id="2c54e-123">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="2c54e-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="2c54e-124">値</span><span class="sxs-lookup"><span data-stu-id="2c54e-124">value</span></span>|<span data-ttu-id="2c54e-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c54e-125">DateTimeOffset</span></span>|<span data-ttu-id="2c54e-126">値。</span><span class="sxs-lookup"><span data-stu-id="2c54e-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c54e-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2c54e-127">Relationships</span></span>
<span data-ttu-id="2c54e-128">なし</span><span class="sxs-lookup"><span data-stu-id="2c54e-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c54e-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2c54e-129">JSON Representation</span></span>
<span data-ttu-id="2c54e-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2c54e-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingDateTime"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingDateTime",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String (timestamp)"
}
```





