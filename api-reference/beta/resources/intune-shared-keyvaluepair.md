---
title: keyValuePair リソースの種類
description: カスタム設定の保存用のキーと値のペア
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 69924cf755192d8ddefa074b9ec1cfed53a0d5f7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347949"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="ee626-103">keyValuePair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ee626-103">keyValuePair resource type</span></span>

> <span data-ttu-id="ee626-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee626-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee626-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ee626-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee626-106">カスタム設定の保存用のキーと値のペア</span><span class="sxs-lookup"><span data-stu-id="ee626-106">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="ee626-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee626-107">Properties</span></span>
|<span data-ttu-id="ee626-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee626-108">Property</span></span>|<span data-ttu-id="ee626-109">型</span><span class="sxs-lookup"><span data-stu-id="ee626-109">Type</span></span>|<span data-ttu-id="ee626-110">説明</span><span class="sxs-lookup"><span data-stu-id="ee626-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee626-111">name</span><span class="sxs-lookup"><span data-stu-id="ee626-111">name</span></span>|<span data-ttu-id="ee626-112">String</span><span class="sxs-lookup"><span data-stu-id="ee626-112">String</span></span>|<span data-ttu-id="ee626-113">キーと値のペアの名前</span><span class="sxs-lookup"><span data-stu-id="ee626-113">Name for this key-value pair</span></span>|
|<span data-ttu-id="ee626-114">value</span><span class="sxs-lookup"><span data-stu-id="ee626-114">value</span></span>|<span data-ttu-id="ee626-115">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ee626-115">String</span></span>|<span data-ttu-id="ee626-116">キーと値のペアの値</span><span class="sxs-lookup"><span data-stu-id="ee626-116">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee626-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ee626-117">Relationships</span></span>
<span data-ttu-id="ee626-118">なし</span><span class="sxs-lookup"><span data-stu-id="ee626-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee626-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ee626-119">JSON Representation</span></span>
<span data-ttu-id="ee626-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ee626-120">Here is a JSON representation of the resource.</span></span>
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



