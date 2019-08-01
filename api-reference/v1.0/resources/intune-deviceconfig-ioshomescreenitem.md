---
title: iosHomeScreenItem リソースの種類
description: IOS ホーム画面上のアイテムを表します
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d5f7c92b1316b40efd9c87ac39c926669a251d58
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031517"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="4baee-103">iosHomeScreenItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4baee-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="4baee-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4baee-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4baee-105">IOS ホーム画面上のアイテムを表します</span><span class="sxs-lookup"><span data-stu-id="4baee-105">Represents an item on the iOS Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="4baee-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4baee-106">Properties</span></span>
|<span data-ttu-id="4baee-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4baee-107">Property</span></span>|<span data-ttu-id="4baee-108">型</span><span class="sxs-lookup"><span data-stu-id="4baee-108">Type</span></span>|<span data-ttu-id="4baee-109">説明</span><span class="sxs-lookup"><span data-stu-id="4baee-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4baee-110">displayName</span><span class="sxs-lookup"><span data-stu-id="4baee-110">displayName</span></span>|<span data-ttu-id="4baee-111">String</span><span class="sxs-lookup"><span data-stu-id="4baee-111">String</span></span>|<span data-ttu-id="4baee-112">アプリの名前</span><span class="sxs-lookup"><span data-stu-id="4baee-112">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="4baee-113">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4baee-113">Relationships</span></span>
<span data-ttu-id="4baee-114">なし</span><span class="sxs-lookup"><span data-stu-id="4baee-114">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4baee-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4baee-115">JSON Representation</span></span>
<span data-ttu-id="4baee-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4baee-116">Here is a JSON representation of the resource.</span></span>
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



