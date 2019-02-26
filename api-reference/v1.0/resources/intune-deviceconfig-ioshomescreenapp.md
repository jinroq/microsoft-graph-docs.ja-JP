---
title: iosHomeScreenApp リソースの種類
description: ホーム画面上のアプリのアイコンを表します
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 67c11096414db0dccad2ccf56ec184a4e3f30397
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260936"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="dc247-103">iosHomeScreenApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dc247-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="dc247-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dc247-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc247-105">ホーム画面上のアプリのアイコンを表します</span><span class="sxs-lookup"><span data-stu-id="dc247-105">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="dc247-106">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="dc247-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dc247-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc247-107">Properties</span></span>
|<span data-ttu-id="dc247-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc247-108">Property</span></span>|<span data-ttu-id="dc247-109">型</span><span class="sxs-lookup"><span data-stu-id="dc247-109">Type</span></span>|<span data-ttu-id="dc247-110">説明</span><span class="sxs-lookup"><span data-stu-id="dc247-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc247-111">displayName</span><span class="sxs-lookup"><span data-stu-id="dc247-111">displayName</span></span>|<span data-ttu-id="dc247-112">String</span><span class="sxs-lookup"><span data-stu-id="dc247-112">String</span></span>|<span data-ttu-id="dc247-113">アプリの名前。[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) から継承</span><span class="sxs-lookup"><span data-stu-id="dc247-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="dc247-114">bundleID</span><span class="sxs-lookup"><span data-stu-id="dc247-114">bundleID</span></span>|<span data-ttu-id="dc247-115">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="dc247-115">String</span></span>|<span data-ttu-id="dc247-116">アプリの BundleID</span><span class="sxs-lookup"><span data-stu-id="dc247-116">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc247-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dc247-117">Relationships</span></span>
<span data-ttu-id="dc247-118">なし</span><span class="sxs-lookup"><span data-stu-id="dc247-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc247-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dc247-119">JSON Representation</span></span>
<span data-ttu-id="dc247-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dc247-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String"
}
```



