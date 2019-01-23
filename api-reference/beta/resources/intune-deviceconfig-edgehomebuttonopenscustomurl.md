---
title: edgeHomeButtonOpensCustomURL リソースの種類
description: ホーム ボタンを表示します。[ホーム] ボタンをクリックすると、特定の URL が読み込まれます。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 06f73375772f53b546e7e9b758a7513366949326
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431675"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="abda3-103">edgeHomeButtonOpensCustomURL リソースの種類</span><span class="sxs-lookup"><span data-stu-id="abda3-103">edgeHomeButtonOpensCustomURL resource type</span></span>

> <span data-ttu-id="abda3-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="abda3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="abda3-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="abda3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="abda3-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="abda3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abda3-107">ホーム ボタンを表示します。[ホーム] ボタンをクリックすると、特定の URL が読み込まれます。</span><span class="sxs-lookup"><span data-stu-id="abda3-107">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="abda3-108">[EdgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="abda3-108">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="abda3-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="abda3-109">Properties</span></span>
|<span data-ttu-id="abda3-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="abda3-110">Property</span></span>|<span data-ttu-id="abda3-111">型</span><span class="sxs-lookup"><span data-stu-id="abda3-111">Type</span></span>|<span data-ttu-id="abda3-112">説明</span><span class="sxs-lookup"><span data-stu-id="abda3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abda3-113">homeButtonCustomURL</span><span class="sxs-lookup"><span data-stu-id="abda3-113">homeButtonCustomURL</span></span>|<span data-ttu-id="abda3-114">String</span><span class="sxs-lookup"><span data-stu-id="abda3-114">String</span></span>|<span data-ttu-id="abda3-115">ロードするのには特定の URL です。</span><span class="sxs-lookup"><span data-stu-id="abda3-115">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="abda3-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="abda3-116">Relationships</span></span>
<span data-ttu-id="abda3-117">なし</span><span class="sxs-lookup"><span data-stu-id="abda3-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="abda3-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="abda3-118">JSON Representation</span></span>
<span data-ttu-id="abda3-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="abda3-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeHomeButtonOpensCustomURL"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeHomeButtonOpensCustomURL",
  "homeButtonCustomURL": "String"
}
```




