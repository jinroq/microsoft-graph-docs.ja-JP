---
title: iosHomeScreenItem リソースの種類
description: IOS ホーム画面上のアイテムを表します
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 190726b8ee7411a5ce53f8e2802ddf38e0e6b9ff
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408419"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="73b5b-103">iosHomeScreenItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="73b5b-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="73b5b-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="73b5b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="73b5b-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73b5b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="73b5b-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="73b5b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73b5b-107">IOS ホーム画面上のアイテムを表します</span><span class="sxs-lookup"><span data-stu-id="73b5b-107">Represents an item on the iOS Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="73b5b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="73b5b-108">Properties</span></span>
|<span data-ttu-id="73b5b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="73b5b-109">Property</span></span>|<span data-ttu-id="73b5b-110">型</span><span class="sxs-lookup"><span data-stu-id="73b5b-110">Type</span></span>|<span data-ttu-id="73b5b-111">説明</span><span class="sxs-lookup"><span data-stu-id="73b5b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73b5b-112">displayName</span><span class="sxs-lookup"><span data-stu-id="73b5b-112">displayName</span></span>|<span data-ttu-id="73b5b-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="73b5b-113">String</span></span>|<span data-ttu-id="73b5b-114">アプリの名前</span><span class="sxs-lookup"><span data-stu-id="73b5b-114">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="73b5b-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="73b5b-115">Relationships</span></span>
<span data-ttu-id="73b5b-116">なし</span><span class="sxs-lookup"><span data-stu-id="73b5b-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="73b5b-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="73b5b-117">JSON Representation</span></span>
<span data-ttu-id="73b5b-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="73b5b-118">Here is a JSON representation of the resource.</span></span>
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




