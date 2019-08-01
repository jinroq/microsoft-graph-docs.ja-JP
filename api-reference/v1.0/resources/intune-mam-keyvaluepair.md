---
title: keyValuePair リソースの種類
description: カスタム設定の保存用のキーと値のペア
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fd0f9c6e17d1550e4b2584200239ff303ba91232
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36038116"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="9dacd-103">keyValuePair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9dacd-103">keyValuePair resource type</span></span>

> <span data-ttu-id="9dacd-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9dacd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9dacd-105">カスタム設定の保存用のキーと値のペア</span><span class="sxs-lookup"><span data-stu-id="9dacd-105">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="9dacd-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9dacd-106">Properties</span></span>
|<span data-ttu-id="9dacd-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9dacd-107">Property</span></span>|<span data-ttu-id="9dacd-108">型</span><span class="sxs-lookup"><span data-stu-id="9dacd-108">Type</span></span>|<span data-ttu-id="9dacd-109">説明</span><span class="sxs-lookup"><span data-stu-id="9dacd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9dacd-110">name</span><span class="sxs-lookup"><span data-stu-id="9dacd-110">name</span></span>|<span data-ttu-id="9dacd-111">String</span><span class="sxs-lookup"><span data-stu-id="9dacd-111">String</span></span>|<span data-ttu-id="9dacd-112">キーと値のペアの名前</span><span class="sxs-lookup"><span data-stu-id="9dacd-112">Name for this key-value pair</span></span>|
|<span data-ttu-id="9dacd-113">value</span><span class="sxs-lookup"><span data-stu-id="9dacd-113">value</span></span>|<span data-ttu-id="9dacd-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="9dacd-114">String</span></span>|<span data-ttu-id="9dacd-115">キーと値のペアの値</span><span class="sxs-lookup"><span data-stu-id="9dacd-115">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="9dacd-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9dacd-116">Relationships</span></span>
<span data-ttu-id="9dacd-117">なし</span><span class="sxs-lookup"><span data-stu-id="9dacd-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9dacd-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9dacd-118">JSON Representation</span></span>
<span data-ttu-id="9dacd-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9dacd-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValuePair",
  "name": "String",
  "value": "String"
}
```



