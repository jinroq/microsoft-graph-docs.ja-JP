---
title: managedDeviceModelsAndManufacturers リソースの種類
description: アカウントの管理対象デバイスのモデルと製造 meatadata
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 99291829bfa672a9ade85a0a015061e4f6ec8e10
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31782563"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="3426f-103">managedDeviceModelsAndManufacturers リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3426f-103">managedDeviceModelsAndManufacturers resource type</span></span>

> <span data-ttu-id="3426f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3426f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3426f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3426f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3426f-106">アカウントの管理対象デバイスのモデルと製造 meatadata</span><span class="sxs-lookup"><span data-stu-id="3426f-106">Models and Manufactures meatadata for managed devices in the account</span></span>

## <a name="properties"></a><span data-ttu-id="3426f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3426f-107">Properties</span></span>
|<span data-ttu-id="3426f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3426f-108">Property</span></span>|<span data-ttu-id="3426f-109">型</span><span class="sxs-lookup"><span data-stu-id="3426f-109">Type</span></span>|<span data-ttu-id="3426f-110">説明</span><span class="sxs-lookup"><span data-stu-id="3426f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3426f-111">devicemodels</span><span class="sxs-lookup"><span data-stu-id="3426f-111">deviceModels</span></span>|<span data-ttu-id="3426f-112">String コレクション</span><span class="sxs-lookup"><span data-stu-id="3426f-112">String collection</span></span>|<span data-ttu-id="3426f-113">アカウント内の管理されたデバイスのモデルの一覧</span><span class="sxs-lookup"><span data-stu-id="3426f-113">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="3426f-114">deviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="3426f-114">deviceManufacturers</span></span>|<span data-ttu-id="3426f-115">String コレクション</span><span class="sxs-lookup"><span data-stu-id="3426f-115">String collection</span></span>|<span data-ttu-id="3426f-116">アカウントで管理されているデバイスの製造元の一覧</span><span class="sxs-lookup"><span data-stu-id="3426f-116">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="3426f-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3426f-117">Relationships</span></span>
<span data-ttu-id="3426f-118">なし</span><span class="sxs-lookup"><span data-stu-id="3426f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3426f-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3426f-119">JSON Representation</span></span>
<span data-ttu-id="3426f-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3426f-120">Here is a JSON representation of the resource.</span></span>
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





