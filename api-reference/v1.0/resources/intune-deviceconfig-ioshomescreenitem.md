---
title: iosHomeScreenItem リソースの種類
description: IOS ホーム画面上のアイテムを表します
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8aecb99c036d3e8a5d89271afd6042ccb18b4fda
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253394"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="39ba6-103">iosHomeScreenItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="39ba6-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="39ba6-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="39ba6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39ba6-105">IOS ホーム画面上のアイテムを表します</span><span class="sxs-lookup"><span data-stu-id="39ba6-105">Represents an item on the iOS Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="39ba6-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39ba6-106">Properties</span></span>
|<span data-ttu-id="39ba6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39ba6-107">Property</span></span>|<span data-ttu-id="39ba6-108">型</span><span class="sxs-lookup"><span data-stu-id="39ba6-108">Type</span></span>|<span data-ttu-id="39ba6-109">説明</span><span class="sxs-lookup"><span data-stu-id="39ba6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39ba6-110">displayName</span><span class="sxs-lookup"><span data-stu-id="39ba6-110">displayName</span></span>|<span data-ttu-id="39ba6-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="39ba6-111">String</span></span>|<span data-ttu-id="39ba6-112">アプリの名前</span><span class="sxs-lookup"><span data-stu-id="39ba6-112">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="39ba6-113">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="39ba6-113">Relationships</span></span>
<span data-ttu-id="39ba6-114">なし</span><span class="sxs-lookup"><span data-stu-id="39ba6-114">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="39ba6-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="39ba6-115">JSON Representation</span></span>
<span data-ttu-id="39ba6-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="39ba6-116">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenItem",
  "displayName": "String"
}
```



