---
title: managedDeviceModelsAndManufacturers リソースの種類
description: モデルと、アカウントで管理されているデバイスのメーカーの meatadata
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: afcf64cb0e8db4e24ce061490ecc593595690930
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396792"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="9cb5a-103">managedDeviceModelsAndManufacturers リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9cb5a-103">managedDeviceModelsAndManufacturers resource type</span></span>

> <span data-ttu-id="9cb5a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9cb5a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9cb5a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9cb5a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9cb5a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9cb5a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cb5a-107">モデルと、アカウントで管理されているデバイスのメーカーの meatadata</span><span class="sxs-lookup"><span data-stu-id="9cb5a-107">Models and Manufactures meatadata for managed devices in the account</span></span>

## <a name="properties"></a><span data-ttu-id="9cb5a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9cb5a-108">Properties</span></span>
|<span data-ttu-id="9cb5a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9cb5a-109">Property</span></span>|<span data-ttu-id="9cb5a-110">型</span><span class="sxs-lookup"><span data-stu-id="9cb5a-110">Type</span></span>|<span data-ttu-id="9cb5a-111">説明</span><span class="sxs-lookup"><span data-stu-id="9cb5a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cb5a-112">deviceModels</span><span class="sxs-lookup"><span data-stu-id="9cb5a-112">deviceModels</span></span>|<span data-ttu-id="9cb5a-113">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9cb5a-113">String collection</span></span>|<span data-ttu-id="9cb5a-114">アカウントで管理されているデバイスのモデルの一覧</span><span class="sxs-lookup"><span data-stu-id="9cb5a-114">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="9cb5a-115">deviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="9cb5a-115">deviceManufacturers</span></span>|<span data-ttu-id="9cb5a-116">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9cb5a-116">String collection</span></span>|<span data-ttu-id="9cb5a-117">アカウントで管理されているデバイスの製造元の一覧</span><span class="sxs-lookup"><span data-stu-id="9cb5a-117">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="9cb5a-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9cb5a-118">Relationships</span></span>
<span data-ttu-id="9cb5a-119">なし</span><span class="sxs-lookup"><span data-stu-id="9cb5a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9cb5a-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9cb5a-120">JSON Representation</span></span>
<span data-ttu-id="9cb5a-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9cb5a-121">Here is a JSON representation of the resource.</span></span>
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




