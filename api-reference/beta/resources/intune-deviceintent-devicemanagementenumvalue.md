---
title: deviceManagementEnumValue リソースの種類
description: 列挙値の定義情報
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ade5c3c10354d8697ca40f553c0941751cd26c1a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366624"
---
# <a name="devicemanagementenumvalue-resource-type"></a><span data-ttu-id="2170d-103">deviceManagementEnumValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2170d-103">deviceManagementEnumValue resource type</span></span>

> <span data-ttu-id="2170d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2170d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2170d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2170d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2170d-106">列挙値の定義情報</span><span class="sxs-lookup"><span data-stu-id="2170d-106">Definition information for an enum value</span></span>

## <a name="properties"></a><span data-ttu-id="2170d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2170d-107">Properties</span></span>
|<span data-ttu-id="2170d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2170d-108">Property</span></span>|<span data-ttu-id="2170d-109">型</span><span class="sxs-lookup"><span data-stu-id="2170d-109">Type</span></span>|<span data-ttu-id="2170d-110">説明</span><span class="sxs-lookup"><span data-stu-id="2170d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2170d-111">value</span><span class="sxs-lookup"><span data-stu-id="2170d-111">value</span></span>|<span data-ttu-id="2170d-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2170d-112">String</span></span>|<span data-ttu-id="2170d-113">生の列挙値のテキスト</span><span class="sxs-lookup"><span data-stu-id="2170d-113">The raw enum value text</span></span>|
|<span data-ttu-id="2170d-114">displayName</span><span class="sxs-lookup"><span data-stu-id="2170d-114">displayName</span></span>|<span data-ttu-id="2170d-115">String</span><span class="sxs-lookup"><span data-stu-id="2170d-115">String</span></span>|<span data-ttu-id="2170d-116">この列挙値の表示名</span><span class="sxs-lookup"><span data-stu-id="2170d-116">Display name for this enum value</span></span>|

## <a name="relationships"></a><span data-ttu-id="2170d-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2170d-117">Relationships</span></span>
<span data-ttu-id="2170d-118">なし</span><span class="sxs-lookup"><span data-stu-id="2170d-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2170d-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2170d-119">JSON Representation</span></span>
<span data-ttu-id="2170d-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2170d-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementEnumValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementEnumValue",
  "value": "String",
  "displayName": "String"
}
```



