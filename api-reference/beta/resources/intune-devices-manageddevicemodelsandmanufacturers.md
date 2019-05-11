---
title: managedDeviceModelsAndManufacturers リソースの種類
description: アカウントの管理対象デバイスのモデルと製造 meatadata
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d7218e25fc9d1ed0b53bf95cd25ca4b8e3a2e7d8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941941"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="1edb9-103">managedDeviceModelsAndManufacturers リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1edb9-103">managedDeviceModelsAndManufacturers resource type</span></span>

> <span data-ttu-id="1edb9-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1edb9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1edb9-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1edb9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1edb9-106">アカウントの管理対象デバイスのモデルと製造 meatadata</span><span class="sxs-lookup"><span data-stu-id="1edb9-106">Models and Manufactures meatadata for managed devices in the account</span></span>

## <a name="properties"></a><span data-ttu-id="1edb9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1edb9-107">Properties</span></span>
|<span data-ttu-id="1edb9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1edb9-108">Property</span></span>|<span data-ttu-id="1edb9-109">型</span><span class="sxs-lookup"><span data-stu-id="1edb9-109">Type</span></span>|<span data-ttu-id="1edb9-110">説明</span><span class="sxs-lookup"><span data-stu-id="1edb9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1edb9-111">deviceModels</span><span class="sxs-lookup"><span data-stu-id="1edb9-111">deviceModels</span></span>|<span data-ttu-id="1edb9-112">String collection</span><span class="sxs-lookup"><span data-stu-id="1edb9-112">String collection</span></span>|<span data-ttu-id="1edb9-113">アカウント内の管理されたデバイスのモデルの一覧</span><span class="sxs-lookup"><span data-stu-id="1edb9-113">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="1edb9-114">deviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="1edb9-114">deviceManufacturers</span></span>|<span data-ttu-id="1edb9-115">String collection</span><span class="sxs-lookup"><span data-stu-id="1edb9-115">String collection</span></span>|<span data-ttu-id="1edb9-116">アカウントで管理されているデバイスの製造元の一覧</span><span class="sxs-lookup"><span data-stu-id="1edb9-116">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="1edb9-117">関係</span><span class="sxs-lookup"><span data-stu-id="1edb9-117">Relationships</span></span>
<span data-ttu-id="1edb9-118">なし</span><span class="sxs-lookup"><span data-stu-id="1edb9-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1edb9-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1edb9-119">JSON Representation</span></span>
<span data-ttu-id="1edb9-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1edb9-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceModelsAndManufacturers",
  "deviceModels": [
    "String"
  ],
  "deviceManufacturers": [
    "String"
  ]
}
```




