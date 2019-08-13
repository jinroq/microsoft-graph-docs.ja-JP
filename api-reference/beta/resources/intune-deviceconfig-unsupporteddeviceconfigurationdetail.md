---
title: unsupportedDeviceConfigurationDetail リソースの種類
description: エンティティがサポートされていない理由の説明。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7d628fb6c7bc8adfab97b401d9ebc8879435502c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367821"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="48a4d-103">unsupportedDeviceConfigurationDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="48a4d-103">unsupportedDeviceConfigurationDetail resource type</span></span>

> <span data-ttu-id="48a4d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="48a4d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48a4d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="48a4d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48a4d-106">エンティティがサポートされていない理由の説明。</span><span class="sxs-lookup"><span data-stu-id="48a4d-106">A description of why an entity is unsupported.</span></span>

## <a name="properties"></a><span data-ttu-id="48a4d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48a4d-107">Properties</span></span>
|<span data-ttu-id="48a4d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48a4d-108">Property</span></span>|<span data-ttu-id="48a4d-109">型</span><span class="sxs-lookup"><span data-stu-id="48a4d-109">Type</span></span>|<span data-ttu-id="48a4d-110">説明</span><span class="sxs-lookup"><span data-stu-id="48a4d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48a4d-111">メッセージ​​</span><span class="sxs-lookup"><span data-stu-id="48a4d-111">message</span></span>|<span data-ttu-id="48a4d-112">String</span><span class="sxs-lookup"><span data-stu-id="48a4d-112">String</span></span>|<span data-ttu-id="48a4d-113">エンティティがサポートされていない理由を説明するメッセージ。</span><span class="sxs-lookup"><span data-stu-id="48a4d-113">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="48a4d-114">propertyName</span><span class="sxs-lookup"><span data-stu-id="48a4d-114">propertyName</span></span>|<span data-ttu-id="48a4d-115">String</span><span class="sxs-lookup"><span data-stu-id="48a4d-115">String</span></span>|<span data-ttu-id="48a4d-116">メッセージが元のエンティティの特定のプロパティに関連付けられている場合は、そのプロパティの名前。</span><span class="sxs-lookup"><span data-stu-id="48a4d-116">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48a4d-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="48a4d-117">Relationships</span></span>
<span data-ttu-id="48a4d-118">なし</span><span class="sxs-lookup"><span data-stu-id="48a4d-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="48a4d-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="48a4d-119">JSON Representation</span></span>
<span data-ttu-id="48a4d-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="48a4d-120">Here is a JSON representation of the resource.</span></span>
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



