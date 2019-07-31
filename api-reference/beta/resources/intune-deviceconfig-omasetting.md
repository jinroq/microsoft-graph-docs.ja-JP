---
title: omaSetting リソースの種類
description: OMA 設定の定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 58de40a93fe85c1eb58b558cf44214358070901d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969976"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="d2857-103">omaSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d2857-103">omaSetting resource type</span></span>

> <span data-ttu-id="d2857-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2857-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2857-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d2857-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2857-106">OMA 設定の定義。</span><span class="sxs-lookup"><span data-stu-id="d2857-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="d2857-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d2857-107">Properties</span></span>
|<span data-ttu-id="d2857-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d2857-108">Property</span></span>|<span data-ttu-id="d2857-109">型</span><span class="sxs-lookup"><span data-stu-id="d2857-109">Type</span></span>|<span data-ttu-id="d2857-110">説明</span><span class="sxs-lookup"><span data-stu-id="d2857-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2857-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d2857-111">displayName</span></span>|<span data-ttu-id="d2857-112">String</span><span class="sxs-lookup"><span data-stu-id="d2857-112">String</span></span>|<span data-ttu-id="d2857-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="d2857-113">Display Name.</span></span>|
|<span data-ttu-id="d2857-114">description</span><span class="sxs-lookup"><span data-stu-id="d2857-114">description</span></span>|<span data-ttu-id="d2857-115">String</span><span class="sxs-lookup"><span data-stu-id="d2857-115">String</span></span>|<span data-ttu-id="d2857-116">説明。</span><span class="sxs-lookup"><span data-stu-id="d2857-116">Description.</span></span>|
|<span data-ttu-id="d2857-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="d2857-117">omaUri</span></span>|<span data-ttu-id="d2857-118">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="d2857-118">String</span></span>|<span data-ttu-id="d2857-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="d2857-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2857-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d2857-120">Relationships</span></span>
<span data-ttu-id="d2857-121">なし</span><span class="sxs-lookup"><span data-stu-id="d2857-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2857-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d2857-122">JSON Representation</span></span>
<span data-ttu-id="d2857-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d2857-123">Here is a JSON representation of the resource.</span></span>
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





