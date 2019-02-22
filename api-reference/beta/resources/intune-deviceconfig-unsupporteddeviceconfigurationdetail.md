---
title: unsupportedDeviceConfigurationDetail リソースの種類
description: エンティティがサポートされていない理由の説明。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6ebdb6eb91dd64c1605288cc0cb1260f8fe7440a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148469"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="e7ebd-103">unsupportedDeviceConfigurationDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e7ebd-103">unsupportedDeviceConfigurationDetail resource type</span></span>

> <span data-ttu-id="e7ebd-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7ebd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7ebd-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e7ebd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7ebd-106">エンティティがサポートされていない理由の説明。</span><span class="sxs-lookup"><span data-stu-id="e7ebd-106">A description of why an entity is unsupported.</span></span>

## <a name="properties"></a><span data-ttu-id="e7ebd-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e7ebd-107">Properties</span></span>
|<span data-ttu-id="e7ebd-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e7ebd-108">Property</span></span>|<span data-ttu-id="e7ebd-109">型</span><span class="sxs-lookup"><span data-stu-id="e7ebd-109">Type</span></span>|<span data-ttu-id="e7ebd-110">説明</span><span class="sxs-lookup"><span data-stu-id="e7ebd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7ebd-111">message</span><span class="sxs-lookup"><span data-stu-id="e7ebd-111">message</span></span>|<span data-ttu-id="e7ebd-112">String</span><span class="sxs-lookup"><span data-stu-id="e7ebd-112">String</span></span>|<span data-ttu-id="e7ebd-113">エンティティがサポートされていない理由を説明するメッセージ。</span><span class="sxs-lookup"><span data-stu-id="e7ebd-113">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="e7ebd-114">propertyName</span><span class="sxs-lookup"><span data-stu-id="e7ebd-114">propertyName</span></span>|<span data-ttu-id="e7ebd-115">String</span><span class="sxs-lookup"><span data-stu-id="e7ebd-115">String</span></span>|<span data-ttu-id="e7ebd-116">メッセージが元のエンティティの特定のプロパティに関連付けられている場合は、そのプロパティの名前。</span><span class="sxs-lookup"><span data-stu-id="e7ebd-116">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7ebd-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e7ebd-117">Relationships</span></span>
<span data-ttu-id="e7ebd-118">なし</span><span class="sxs-lookup"><span data-stu-id="e7ebd-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7ebd-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e7ebd-119">JSON Representation</span></span>
<span data-ttu-id="e7ebd-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e7ebd-120">Here is a JSON representation of the resource.</span></span>
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




