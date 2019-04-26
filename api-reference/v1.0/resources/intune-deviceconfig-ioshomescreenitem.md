---
title: iosHomeScreenItem リソースの種類
description: IOS ホーム画面上のアイテムを表します
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8aecb99c036d3e8a5d89271afd6042ccb18b4fda
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554654"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="a2644-103">iosHomeScreenItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a2644-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="a2644-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a2644-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2644-105">IOS ホーム画面上のアイテムを表します</span><span class="sxs-lookup"><span data-stu-id="a2644-105">Represents an item on the iOS Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="a2644-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2644-106">Properties</span></span>
|<span data-ttu-id="a2644-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2644-107">Property</span></span>|<span data-ttu-id="a2644-108">型</span><span class="sxs-lookup"><span data-stu-id="a2644-108">Type</span></span>|<span data-ttu-id="a2644-109">説明</span><span class="sxs-lookup"><span data-stu-id="a2644-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2644-110">displayName</span><span class="sxs-lookup"><span data-stu-id="a2644-110">displayName</span></span>|<span data-ttu-id="a2644-111">String</span><span class="sxs-lookup"><span data-stu-id="a2644-111">String</span></span>|<span data-ttu-id="a2644-112">アプリの名前</span><span class="sxs-lookup"><span data-stu-id="a2644-112">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2644-113">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a2644-113">Relationships</span></span>
<span data-ttu-id="a2644-114">なし</span><span class="sxs-lookup"><span data-stu-id="a2644-114">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2644-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a2644-115">JSON Representation</span></span>
<span data-ttu-id="a2644-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a2644-116">Here is a JSON representation of the resource.</span></span>
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



