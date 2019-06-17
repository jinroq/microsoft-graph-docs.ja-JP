---
title: omaSettingBoolean リソースの種類
description: OMA 設定のブール定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7269b8c61603601d0932a000f7f90e63d7cbc44e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993733"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="62c08-103">omaSettingBoolean リソースの種類</span><span class="sxs-lookup"><span data-stu-id="62c08-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="62c08-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62c08-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62c08-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="62c08-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62c08-106">OMA 設定のブール定義。</span><span class="sxs-lookup"><span data-stu-id="62c08-106">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="62c08-107">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="62c08-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="62c08-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62c08-108">Properties</span></span>
|<span data-ttu-id="62c08-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62c08-109">Property</span></span>|<span data-ttu-id="62c08-110">型</span><span class="sxs-lookup"><span data-stu-id="62c08-110">Type</span></span>|<span data-ttu-id="62c08-111">説明</span><span class="sxs-lookup"><span data-stu-id="62c08-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62c08-112">displayName</span><span class="sxs-lookup"><span data-stu-id="62c08-112">displayName</span></span>|<span data-ttu-id="62c08-113">String</span><span class="sxs-lookup"><span data-stu-id="62c08-113">String</span></span>|<span data-ttu-id="62c08-114">表示名。</span><span class="sxs-lookup"><span data-stu-id="62c08-114">Display Name.</span></span> <span data-ttu-id="62c08-115">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="62c08-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="62c08-116">description</span><span class="sxs-lookup"><span data-stu-id="62c08-116">description</span></span>|<span data-ttu-id="62c08-117">String</span><span class="sxs-lookup"><span data-stu-id="62c08-117">String</span></span>|<span data-ttu-id="62c08-118">説明。</span><span class="sxs-lookup"><span data-stu-id="62c08-118">Description.</span></span> <span data-ttu-id="62c08-119">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="62c08-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="62c08-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="62c08-120">omaUri</span></span>|<span data-ttu-id="62c08-121">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="62c08-121">String</span></span>|<span data-ttu-id="62c08-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="62c08-122">OMA.</span></span> <span data-ttu-id="62c08-123">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="62c08-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="62c08-124">value</span><span class="sxs-lookup"><span data-stu-id="62c08-124">value</span></span>|<span data-ttu-id="62c08-125">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="62c08-125">Boolean</span></span>|<span data-ttu-id="62c08-126">値。</span><span class="sxs-lookup"><span data-stu-id="62c08-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="62c08-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="62c08-127">Relationships</span></span>
<span data-ttu-id="62c08-128">なし</span><span class="sxs-lookup"><span data-stu-id="62c08-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="62c08-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="62c08-129">JSON Representation</span></span>
<span data-ttu-id="62c08-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="62c08-130">Here is a JSON representation of the resource.</span></span>
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





