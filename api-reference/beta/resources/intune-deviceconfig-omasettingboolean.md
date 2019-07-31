---
title: omaSettingBoolean リソースの種類
description: OMA 設定のブール定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5e5bfbd19f4899b7ef3cdb788b4d7a7fe1b55252
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969941"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="eea0d-103">omaSettingBoolean リソースの種類</span><span class="sxs-lookup"><span data-stu-id="eea0d-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="eea0d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eea0d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eea0d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="eea0d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eea0d-106">OMA 設定のブール定義。</span><span class="sxs-lookup"><span data-stu-id="eea0d-106">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="eea0d-107">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="eea0d-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eea0d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eea0d-108">Properties</span></span>
|<span data-ttu-id="eea0d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eea0d-109">Property</span></span>|<span data-ttu-id="eea0d-110">型</span><span class="sxs-lookup"><span data-stu-id="eea0d-110">Type</span></span>|<span data-ttu-id="eea0d-111">説明</span><span class="sxs-lookup"><span data-stu-id="eea0d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eea0d-112">displayName</span><span class="sxs-lookup"><span data-stu-id="eea0d-112">displayName</span></span>|<span data-ttu-id="eea0d-113">String</span><span class="sxs-lookup"><span data-stu-id="eea0d-113">String</span></span>|<span data-ttu-id="eea0d-114">表示名。</span><span class="sxs-lookup"><span data-stu-id="eea0d-114">Display Name.</span></span> <span data-ttu-id="eea0d-115">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="eea0d-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="eea0d-116">description</span><span class="sxs-lookup"><span data-stu-id="eea0d-116">description</span></span>|<span data-ttu-id="eea0d-117">String</span><span class="sxs-lookup"><span data-stu-id="eea0d-117">String</span></span>|<span data-ttu-id="eea0d-118">説明。</span><span class="sxs-lookup"><span data-stu-id="eea0d-118">Description.</span></span> <span data-ttu-id="eea0d-119">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="eea0d-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="eea0d-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="eea0d-120">omaUri</span></span>|<span data-ttu-id="eea0d-121">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="eea0d-121">String</span></span>|<span data-ttu-id="eea0d-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="eea0d-122">OMA.</span></span> <span data-ttu-id="eea0d-123">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="eea0d-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="eea0d-124">value</span><span class="sxs-lookup"><span data-stu-id="eea0d-124">value</span></span>|<span data-ttu-id="eea0d-125">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="eea0d-125">Boolean</span></span>|<span data-ttu-id="eea0d-126">値。</span><span class="sxs-lookup"><span data-stu-id="eea0d-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eea0d-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="eea0d-127">Relationships</span></span>
<span data-ttu-id="eea0d-128">なし</span><span class="sxs-lookup"><span data-stu-id="eea0d-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eea0d-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eea0d-129">JSON Representation</span></span>
<span data-ttu-id="eea0d-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="eea0d-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBoolean"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBoolean",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": true
}
```





