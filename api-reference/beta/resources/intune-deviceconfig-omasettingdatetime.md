---
title: omaSettingDateTime リソースの種類
description: OMA 設定の DateTime の定義です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8a237f36a209e2fa1d552c8f50207770429a0c53
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554493"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="a9daf-103">omaSettingDateTime リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a9daf-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="a9daf-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9daf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9daf-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a9daf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9daf-106">OMA 設定の DateTime の定義です。</span><span class="sxs-lookup"><span data-stu-id="a9daf-106">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="a9daf-107">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="a9daf-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a9daf-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9daf-108">Properties</span></span>
|<span data-ttu-id="a9daf-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9daf-109">Property</span></span>|<span data-ttu-id="a9daf-110">型</span><span class="sxs-lookup"><span data-stu-id="a9daf-110">Type</span></span>|<span data-ttu-id="a9daf-111">説明</span><span class="sxs-lookup"><span data-stu-id="a9daf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9daf-112">displayName</span><span class="sxs-lookup"><span data-stu-id="a9daf-112">displayName</span></span>|<span data-ttu-id="a9daf-113">String</span><span class="sxs-lookup"><span data-stu-id="a9daf-113">String</span></span>|<span data-ttu-id="a9daf-114">表示名。</span><span class="sxs-lookup"><span data-stu-id="a9daf-114">Display Name.</span></span> <span data-ttu-id="a9daf-115">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="a9daf-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a9daf-116">description</span><span class="sxs-lookup"><span data-stu-id="a9daf-116">description</span></span>|<span data-ttu-id="a9daf-117">String</span><span class="sxs-lookup"><span data-stu-id="a9daf-117">String</span></span>|<span data-ttu-id="a9daf-118">説明。</span><span class="sxs-lookup"><span data-stu-id="a9daf-118">Description.</span></span> <span data-ttu-id="a9daf-119">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="a9daf-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a9daf-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="a9daf-120">omaUri</span></span>|<span data-ttu-id="a9daf-121">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="a9daf-121">String</span></span>|<span data-ttu-id="a9daf-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="a9daf-122">OMA.</span></span> <span data-ttu-id="a9daf-123">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="a9daf-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a9daf-124">値</span><span class="sxs-lookup"><span data-stu-id="a9daf-124">value</span></span>|<span data-ttu-id="a9daf-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9daf-125">DateTimeOffset</span></span>|<span data-ttu-id="a9daf-126">値。</span><span class="sxs-lookup"><span data-stu-id="a9daf-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9daf-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a9daf-127">Relationships</span></span>
<span data-ttu-id="a9daf-128">なし</span><span class="sxs-lookup"><span data-stu-id="a9daf-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9daf-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a9daf-129">JSON Representation</span></span>
<span data-ttu-id="a9daf-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a9daf-130">Here is a JSON representation of the resource.</span></span>
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





