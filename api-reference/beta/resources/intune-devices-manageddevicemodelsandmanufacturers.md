---
title: managedDeviceModelsAndManufacturers リソースの種類
description: アカウントの管理対象デバイスのモデルと製造 meatadata
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1e9846b9d551b7ae226fe13c32100c8cbfd049ee
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372266"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="79ded-103">managedDeviceModelsAndManufacturers リソースの種類</span><span class="sxs-lookup"><span data-stu-id="79ded-103">managedDeviceModelsAndManufacturers resource type</span></span>

> <span data-ttu-id="79ded-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79ded-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79ded-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="79ded-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79ded-106">アカウントの管理対象デバイスのモデルと製造 meatadata</span><span class="sxs-lookup"><span data-stu-id="79ded-106">Models and Manufactures meatadata for managed devices in the account</span></span>

## <a name="properties"></a><span data-ttu-id="79ded-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79ded-107">Properties</span></span>
|<span data-ttu-id="79ded-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79ded-108">Property</span></span>|<span data-ttu-id="79ded-109">型</span><span class="sxs-lookup"><span data-stu-id="79ded-109">Type</span></span>|<span data-ttu-id="79ded-110">説明</span><span class="sxs-lookup"><span data-stu-id="79ded-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79ded-111">deviceModels</span><span class="sxs-lookup"><span data-stu-id="79ded-111">deviceModels</span></span>|<span data-ttu-id="79ded-112">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="79ded-112">String collection</span></span>|<span data-ttu-id="79ded-113">アカウント内の管理されたデバイスのモデルの一覧</span><span class="sxs-lookup"><span data-stu-id="79ded-113">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="79ded-114">deviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="79ded-114">deviceManufacturers</span></span>|<span data-ttu-id="79ded-115">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="79ded-115">String collection</span></span>|<span data-ttu-id="79ded-116">アカウントで管理されているデバイスの製造元の一覧</span><span class="sxs-lookup"><span data-stu-id="79ded-116">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="79ded-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="79ded-117">Relationships</span></span>
<span data-ttu-id="79ded-118">なし</span><span class="sxs-lookup"><span data-stu-id="79ded-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="79ded-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="79ded-119">JSON Representation</span></span>
<span data-ttu-id="79ded-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="79ded-120">Here is a JSON representation of the resource.</span></span>
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



