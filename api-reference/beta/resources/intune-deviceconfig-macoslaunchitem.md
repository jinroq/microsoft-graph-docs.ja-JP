---
title: macoslaunchitem リソースの種類
description: macOS 起動アイテムの一覧にあるアプリを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1317f2d42c21d0d11d45290696f183c679b049e1
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31809273"
---
# <a name="macoslaunchitem-resource-type"></a><span data-ttu-id="310ba-103">macoslaunchitem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="310ba-103">macOSLaunchItem resource type</span></span>

> <span data-ttu-id="310ba-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="310ba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="310ba-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="310ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="310ba-106">macOS 起動アイテムの一覧にあるアプリを表します。</span><span class="sxs-lookup"><span data-stu-id="310ba-106">Represents an app in the list of macOS launch items</span></span>

## <a name="properties"></a><span data-ttu-id="310ba-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="310ba-107">Properties</span></span>
|<span data-ttu-id="310ba-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="310ba-108">Property</span></span>|<span data-ttu-id="310ba-109">型</span><span class="sxs-lookup"><span data-stu-id="310ba-109">Type</span></span>|<span data-ttu-id="310ba-110">説明</span><span class="sxs-lookup"><span data-stu-id="310ba-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="310ba-111">path</span><span class="sxs-lookup"><span data-stu-id="310ba-111">path</span></span>|<span data-ttu-id="310ba-112">String</span><span class="sxs-lookup"><span data-stu-id="310ba-112">String</span></span>|<span data-ttu-id="310ba-113">起動項目へのパス。</span><span class="sxs-lookup"><span data-stu-id="310ba-113">Path to the launch item.</span></span>|
|<span data-ttu-id="310ba-114">と</span><span class="sxs-lookup"><span data-stu-id="310ba-114">hide</span></span>|<span data-ttu-id="310ba-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="310ba-115">Boolean</span></span>|<span data-ttu-id="310ba-116">[ユーザーとグループ] リストのアイテムを非表示にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="310ba-116">Whether or not to hide the item from the Users and Groups List.</span></span>|

## <a name="relationships"></a><span data-ttu-id="310ba-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="310ba-117">Relationships</span></span>
<span data-ttu-id="310ba-118">なし</span><span class="sxs-lookup"><span data-stu-id="310ba-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="310ba-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="310ba-119">JSON Representation</span></span>
<span data-ttu-id="310ba-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="310ba-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLaunchItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLaunchItem",
  "path": "String",
  "hide": true
}
```




