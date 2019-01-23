---
title: unsupportedDeviceConfigurationDetail リソースの種類
description: エンティティがサポートされている理由の説明です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c03bdb20fc4c48fa7820e09b9212bf73250599aa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400390"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="173ec-103">unsupportedDeviceConfigurationDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="173ec-103">unsupportedDeviceConfigurationDetail resource type</span></span>

> <span data-ttu-id="173ec-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="173ec-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="173ec-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="173ec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="173ec-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="173ec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="173ec-107">エンティティがサポートされている理由の説明です。</span><span class="sxs-lookup"><span data-stu-id="173ec-107">A description of why an entity is unsupported.</span></span>

## <a name="properties"></a><span data-ttu-id="173ec-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="173ec-108">Properties</span></span>
|<span data-ttu-id="173ec-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="173ec-109">Property</span></span>|<span data-ttu-id="173ec-110">型</span><span class="sxs-lookup"><span data-stu-id="173ec-110">Type</span></span>|<span data-ttu-id="173ec-111">説明</span><span class="sxs-lookup"><span data-stu-id="173ec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="173ec-112">message</span><span class="sxs-lookup"><span data-stu-id="173ec-112">message</span></span>|<span data-ttu-id="173ec-113">String</span><span class="sxs-lookup"><span data-stu-id="173ec-113">String</span></span>|<span data-ttu-id="173ec-114">エンティティがサポートされている理由を説明するメッセージ。</span><span class="sxs-lookup"><span data-stu-id="173ec-114">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="173ec-115">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="173ec-115">propertyName</span></span>|<span data-ttu-id="173ec-116">String</span><span class="sxs-lookup"><span data-stu-id="173ec-116">String</span></span>|<span data-ttu-id="173ec-117">メッセージが元のエンティティでは、そのプロパティの名前に特定のプロパティに関連しています。</span><span class="sxs-lookup"><span data-stu-id="173ec-117">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="173ec-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="173ec-118">Relationships</span></span>
<span data-ttu-id="173ec-119">なし</span><span class="sxs-lookup"><span data-stu-id="173ec-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="173ec-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="173ec-120">JSON Representation</span></span>
<span data-ttu-id="173ec-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="173ec-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfigurationDetail",
  "message": "String",
  "propertyName": "String"
}
```




