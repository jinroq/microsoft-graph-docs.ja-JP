---
title: keyValuePair リソースの種類
description: カスタム設定の保存用のキーと値のペア
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ed4af707320da09c9b72537168f8fd77a424c790
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465434"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="e7600-103">keyValuePair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e7600-103">keyValuePair resource type</span></span>

> <span data-ttu-id="e7600-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e7600-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7600-105">カスタム設定の保存用のキーと値のペア</span><span class="sxs-lookup"><span data-stu-id="e7600-105">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="e7600-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e7600-106">Properties</span></span>
|<span data-ttu-id="e7600-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e7600-107">Property</span></span>|<span data-ttu-id="e7600-108">型</span><span class="sxs-lookup"><span data-stu-id="e7600-108">Type</span></span>|<span data-ttu-id="e7600-109">説明</span><span class="sxs-lookup"><span data-stu-id="e7600-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7600-110">name</span><span class="sxs-lookup"><span data-stu-id="e7600-110">name</span></span>|<span data-ttu-id="e7600-111">String</span><span class="sxs-lookup"><span data-stu-id="e7600-111">String</span></span>|<span data-ttu-id="e7600-112">キーと値のペアの名前</span><span class="sxs-lookup"><span data-stu-id="e7600-112">Name for this key-value pair</span></span>|
|<span data-ttu-id="e7600-113">value</span><span class="sxs-lookup"><span data-stu-id="e7600-113">value</span></span>|<span data-ttu-id="e7600-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e7600-114">String</span></span>|<span data-ttu-id="e7600-115">キーと値のペアの値</span><span class="sxs-lookup"><span data-stu-id="e7600-115">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7600-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e7600-116">Relationships</span></span>
<span data-ttu-id="e7600-117">なし</span><span class="sxs-lookup"><span data-stu-id="e7600-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7600-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e7600-118">JSON Representation</span></span>
<span data-ttu-id="e7600-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e7600-119">Here is a JSON representation of the resource.</span></span>
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



