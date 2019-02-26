---
title: resourceAction リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d229a6d4d8b514cbf092efb224ff09dfb0c78ad4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157625"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="c643a-103">resourceAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c643a-103">resourceAction resource type</span></span>

> <span data-ttu-id="c643a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c643a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c643a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c643a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c643a-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c643a-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c643a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c643a-107">Properties</span></span>
|<span data-ttu-id="c643a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c643a-108">Property</span></span>|<span data-ttu-id="c643a-109">型</span><span class="sxs-lookup"><span data-stu-id="c643a-109">Type</span></span>|<span data-ttu-id="c643a-110">説明</span><span class="sxs-lookup"><span data-stu-id="c643a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c643a-111">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="c643a-111">allowedResourceActions</span></span>|<span data-ttu-id="c643a-112">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c643a-112">String collection</span></span>|<span data-ttu-id="c643a-113">許可されるアクション</span><span class="sxs-lookup"><span data-stu-id="c643a-113">Allowed Actions</span></span>|
|<span data-ttu-id="c643a-114">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="c643a-114">notAllowedResourceActions</span></span>|<span data-ttu-id="c643a-115">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="c643a-115">String collection</span></span>|<span data-ttu-id="c643a-116">許可されていないアクション</span><span class="sxs-lookup"><span data-stu-id="c643a-116">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="c643a-117">関係</span><span class="sxs-lookup"><span data-stu-id="c643a-117">Relationships</span></span>
<span data-ttu-id="c643a-118">なし</span><span class="sxs-lookup"><span data-stu-id="c643a-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c643a-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c643a-119">JSON Representation</span></span>
<span data-ttu-id="c643a-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c643a-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```




