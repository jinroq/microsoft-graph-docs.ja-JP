---
title: unsupportedDeviceConfigurationDetail リソースの種類
description: エンティティがサポートされていない理由の説明。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 53ca6773c3b5341c3f0aae07369b4af80643728d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969605"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="24182-103">unsupportedDeviceConfigurationDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="24182-103">unsupportedDeviceConfigurationDetail resource type</span></span>

> <span data-ttu-id="24182-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24182-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24182-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="24182-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24182-106">エンティティがサポートされていない理由の説明。</span><span class="sxs-lookup"><span data-stu-id="24182-106">A description of why an entity is unsupported.</span></span>

## <a name="properties"></a><span data-ttu-id="24182-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24182-107">Properties</span></span>
|<span data-ttu-id="24182-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24182-108">Property</span></span>|<span data-ttu-id="24182-109">型</span><span class="sxs-lookup"><span data-stu-id="24182-109">Type</span></span>|<span data-ttu-id="24182-110">説明</span><span class="sxs-lookup"><span data-stu-id="24182-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24182-111">メッセージ​​</span><span class="sxs-lookup"><span data-stu-id="24182-111">message</span></span>|<span data-ttu-id="24182-112">String</span><span class="sxs-lookup"><span data-stu-id="24182-112">String</span></span>|<span data-ttu-id="24182-113">エンティティがサポートされていない理由を説明するメッセージ。</span><span class="sxs-lookup"><span data-stu-id="24182-113">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="24182-114">propertyName</span><span class="sxs-lookup"><span data-stu-id="24182-114">propertyName</span></span>|<span data-ttu-id="24182-115">String</span><span class="sxs-lookup"><span data-stu-id="24182-115">String</span></span>|<span data-ttu-id="24182-116">メッセージが元のエンティティの特定のプロパティに関連付けられている場合は、そのプロパティの名前。</span><span class="sxs-lookup"><span data-stu-id="24182-116">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="24182-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="24182-117">Relationships</span></span>
<span data-ttu-id="24182-118">なし</span><span class="sxs-lookup"><span data-stu-id="24182-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="24182-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="24182-119">JSON Representation</span></span>
<span data-ttu-id="24182-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="24182-120">Here is a JSON representation of the resource.</span></span>
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





