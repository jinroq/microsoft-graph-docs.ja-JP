---
title: keyValuePair リソースの種類
description: カスタム設定の保存用のキーと値のペア
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f31e83c5e53ea4c2873fd2b425cc0e0c02678ea7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415783"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="778eb-103">keyValuePair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="778eb-103">keyValuePair resource type</span></span>

> <span data-ttu-id="778eb-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="778eb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="778eb-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="778eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="778eb-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="778eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="778eb-107">カスタム設定の保存用のキーと値のペア</span><span class="sxs-lookup"><span data-stu-id="778eb-107">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="778eb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="778eb-108">Properties</span></span>
|<span data-ttu-id="778eb-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="778eb-109">Property</span></span>|<span data-ttu-id="778eb-110">型</span><span class="sxs-lookup"><span data-stu-id="778eb-110">Type</span></span>|<span data-ttu-id="778eb-111">説明</span><span class="sxs-lookup"><span data-stu-id="778eb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="778eb-112">name</span><span class="sxs-lookup"><span data-stu-id="778eb-112">name</span></span>|<span data-ttu-id="778eb-113">文字列</span><span class="sxs-lookup"><span data-stu-id="778eb-113">String</span></span>|<span data-ttu-id="778eb-114">キーと値のペアの名前</span><span class="sxs-lookup"><span data-stu-id="778eb-114">Name for this key-value pair</span></span>|
|<span data-ttu-id="778eb-115">value</span><span class="sxs-lookup"><span data-stu-id="778eb-115">value</span></span>|<span data-ttu-id="778eb-116">文字列</span><span class="sxs-lookup"><span data-stu-id="778eb-116">String</span></span>|<span data-ttu-id="778eb-117">キーと値のペアの値</span><span class="sxs-lookup"><span data-stu-id="778eb-117">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="778eb-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="778eb-118">Relationships</span></span>
<span data-ttu-id="778eb-119">なし</span><span class="sxs-lookup"><span data-stu-id="778eb-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="778eb-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="778eb-120">JSON Representation</span></span>
<span data-ttu-id="778eb-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="778eb-121">Here is a JSON representation of the resource.</span></span>
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




