---
title: omaSettingInteger リソースの種類
description: OMA 設定の整数の定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 58e668baadc854d2f73a3c9f9e52614905fe1a9f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011401"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="08503-103">omaSettingInteger リソースの種類</span><span class="sxs-lookup"><span data-stu-id="08503-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="08503-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="08503-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08503-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="08503-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08503-106">OMA 設定の整数の定義。</span><span class="sxs-lookup"><span data-stu-id="08503-106">OMA Settings Integer definition.</span></span>


<span data-ttu-id="08503-107">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="08503-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="08503-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="08503-108">Properties</span></span>
|<span data-ttu-id="08503-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="08503-109">Property</span></span>|<span data-ttu-id="08503-110">型</span><span class="sxs-lookup"><span data-stu-id="08503-110">Type</span></span>|<span data-ttu-id="08503-111">説明</span><span class="sxs-lookup"><span data-stu-id="08503-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08503-112">displayName</span><span class="sxs-lookup"><span data-stu-id="08503-112">displayName</span></span>|<span data-ttu-id="08503-113">String</span><span class="sxs-lookup"><span data-stu-id="08503-113">String</span></span>|<span data-ttu-id="08503-114">表示名。</span><span class="sxs-lookup"><span data-stu-id="08503-114">Display Name.</span></span> <span data-ttu-id="08503-115">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="08503-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="08503-116">description</span><span class="sxs-lookup"><span data-stu-id="08503-116">description</span></span>|<span data-ttu-id="08503-117">String</span><span class="sxs-lookup"><span data-stu-id="08503-117">String</span></span>|<span data-ttu-id="08503-118">説明。</span><span class="sxs-lookup"><span data-stu-id="08503-118">Description.</span></span> <span data-ttu-id="08503-119">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="08503-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="08503-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="08503-120">omaUri</span></span>|<span data-ttu-id="08503-121">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="08503-121">String</span></span>|<span data-ttu-id="08503-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="08503-122">OMA.</span></span> <span data-ttu-id="08503-123">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="08503-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="08503-124">値</span><span class="sxs-lookup"><span data-stu-id="08503-124">value</span></span>|<span data-ttu-id="08503-125">Int32</span><span class="sxs-lookup"><span data-stu-id="08503-125">Int32</span></span>|<span data-ttu-id="08503-126">値。</span><span class="sxs-lookup"><span data-stu-id="08503-126">Value.</span></span>|
|<span data-ttu-id="08503-127">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="08503-127">isReadOnly</span></span>|<span data-ttu-id="08503-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="08503-128">Boolean</span></span>|<span data-ttu-id="08503-129">True に設定すると、OMA-URI で指定された CSP (構成サービスプロバイダー) は、を設定するのではなく、get を実行します。</span><span class="sxs-lookup"><span data-stu-id="08503-129">By setting to true, the CSP (configuration service provider) specified in the OMA-URI will perform a get, instead of set</span></span>|

## <a name="relationships"></a><span data-ttu-id="08503-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="08503-130">Relationships</span></span>
<span data-ttu-id="08503-131">なし</span><span class="sxs-lookup"><span data-stu-id="08503-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="08503-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="08503-132">JSON Representation</span></span>
<span data-ttu-id="08503-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="08503-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024,
  "isReadOnly": true
}
```





