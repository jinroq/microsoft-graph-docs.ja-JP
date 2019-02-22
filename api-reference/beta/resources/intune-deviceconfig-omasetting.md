---
title: omaSetting リソースの種類
description: OMA 設定の定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fab80ad06fb5654578f29b92e3b0f3aa9c09abdb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143849"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="55a70-103">omaSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="55a70-103">omaSetting resource type</span></span>

> <span data-ttu-id="55a70-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="55a70-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55a70-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="55a70-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55a70-106">OMA 設定の定義。</span><span class="sxs-lookup"><span data-stu-id="55a70-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="55a70-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="55a70-107">Properties</span></span>
|<span data-ttu-id="55a70-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="55a70-108">Property</span></span>|<span data-ttu-id="55a70-109">型</span><span class="sxs-lookup"><span data-stu-id="55a70-109">Type</span></span>|<span data-ttu-id="55a70-110">説明</span><span class="sxs-lookup"><span data-stu-id="55a70-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55a70-111">displayName</span><span class="sxs-lookup"><span data-stu-id="55a70-111">displayName</span></span>|<span data-ttu-id="55a70-112">String</span><span class="sxs-lookup"><span data-stu-id="55a70-112">String</span></span>|<span data-ttu-id="55a70-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="55a70-113">Display Name.</span></span>|
|<span data-ttu-id="55a70-114">説明</span><span class="sxs-lookup"><span data-stu-id="55a70-114">description</span></span>|<span data-ttu-id="55a70-115">String</span><span class="sxs-lookup"><span data-stu-id="55a70-115">String</span></span>|<span data-ttu-id="55a70-116">説明。</span><span class="sxs-lookup"><span data-stu-id="55a70-116">Description.</span></span>|
|<span data-ttu-id="55a70-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="55a70-117">omaUri</span></span>|<span data-ttu-id="55a70-118">文字列</span><span class="sxs-lookup"><span data-stu-id="55a70-118">String</span></span>|<span data-ttu-id="55a70-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="55a70-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55a70-120">関係</span><span class="sxs-lookup"><span data-stu-id="55a70-120">Relationships</span></span>
<span data-ttu-id="55a70-121">なし</span><span class="sxs-lookup"><span data-stu-id="55a70-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="55a70-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="55a70-122">JSON Representation</span></span>
<span data-ttu-id="55a70-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="55a70-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```




