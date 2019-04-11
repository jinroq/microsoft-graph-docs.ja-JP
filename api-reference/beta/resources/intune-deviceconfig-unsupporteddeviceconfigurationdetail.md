---
title: unsupportedDeviceConfigurationDetail リソースの種類
description: エンティティがサポートされていない理由の説明。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 660f73774025a065565fb72ca74c9674a4159fc0
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31795059"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="6b1a6-103">unsupportedDeviceConfigurationDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6b1a6-103">unsupportedDeviceConfigurationDetail resource type</span></span>

> <span data-ttu-id="6b1a6-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b1a6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b1a6-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6b1a6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b1a6-106">エンティティがサポートされていない理由の説明。</span><span class="sxs-lookup"><span data-stu-id="6b1a6-106">A description of why an entity is unsupported.</span></span>

## <a name="properties"></a><span data-ttu-id="6b1a6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b1a6-107">Properties</span></span>
|<span data-ttu-id="6b1a6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b1a6-108">Property</span></span>|<span data-ttu-id="6b1a6-109">型</span><span class="sxs-lookup"><span data-stu-id="6b1a6-109">Type</span></span>|<span data-ttu-id="6b1a6-110">説明</span><span class="sxs-lookup"><span data-stu-id="6b1a6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b1a6-111">メッセージ​​</span><span class="sxs-lookup"><span data-stu-id="6b1a6-111">message</span></span>|<span data-ttu-id="6b1a6-112">String</span><span class="sxs-lookup"><span data-stu-id="6b1a6-112">String</span></span>|<span data-ttu-id="6b1a6-113">エンティティがサポートされていない理由を説明するメッセージ。</span><span class="sxs-lookup"><span data-stu-id="6b1a6-113">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="6b1a6-114">propertyName</span><span class="sxs-lookup"><span data-stu-id="6b1a6-114">propertyName</span></span>|<span data-ttu-id="6b1a6-115">文字列</span><span class="sxs-lookup"><span data-stu-id="6b1a6-115">String</span></span>|<span data-ttu-id="6b1a6-116">メッセージが元のエンティティの特定のプロパティに関連付けられている場合は、そのプロパティの名前。</span><span class="sxs-lookup"><span data-stu-id="6b1a6-116">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b1a6-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6b1a6-117">Relationships</span></span>
<span data-ttu-id="6b1a6-118">なし</span><span class="sxs-lookup"><span data-stu-id="6b1a6-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b1a6-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6b1a6-119">JSON Representation</span></span>
<span data-ttu-id="6b1a6-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6b1a6-120">Here is a JSON representation of the resource.</span></span>
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





