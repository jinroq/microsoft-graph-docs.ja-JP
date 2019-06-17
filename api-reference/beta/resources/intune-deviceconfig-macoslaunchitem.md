---
title: macOSLaunchItem リソースの種類
description: MacOS 起動アイテムの一覧にあるアプリを表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2752abd8d76c08e1da162d58aa8863d2f8b63940
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34992123"
---
# <a name="macoslaunchitem-resource-type"></a><span data-ttu-id="48f05-103">macOSLaunchItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="48f05-103">macOSLaunchItem resource type</span></span>

> <span data-ttu-id="48f05-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="48f05-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48f05-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="48f05-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48f05-106">MacOS 起動アイテムの一覧にあるアプリを表します。</span><span class="sxs-lookup"><span data-stu-id="48f05-106">Represents an app in the list of macOS launch items</span></span>

## <a name="properties"></a><span data-ttu-id="48f05-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48f05-107">Properties</span></span>
|<span data-ttu-id="48f05-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48f05-108">Property</span></span>|<span data-ttu-id="48f05-109">型</span><span class="sxs-lookup"><span data-stu-id="48f05-109">Type</span></span>|<span data-ttu-id="48f05-110">説明</span><span class="sxs-lookup"><span data-stu-id="48f05-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48f05-111">path</span><span class="sxs-lookup"><span data-stu-id="48f05-111">path</span></span>|<span data-ttu-id="48f05-112">String</span><span class="sxs-lookup"><span data-stu-id="48f05-112">String</span></span>|<span data-ttu-id="48f05-113">起動項目へのパス。</span><span class="sxs-lookup"><span data-stu-id="48f05-113">Path to the launch item.</span></span>|
|<span data-ttu-id="48f05-114">と</span><span class="sxs-lookup"><span data-stu-id="48f05-114">hide</span></span>|<span data-ttu-id="48f05-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="48f05-115">Boolean</span></span>|<span data-ttu-id="48f05-116">[ユーザーとグループ] リストのアイテムを非表示にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="48f05-116">Whether or not to hide the item from the Users and Groups List.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48f05-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="48f05-117">Relationships</span></span>
<span data-ttu-id="48f05-118">なし</span><span class="sxs-lookup"><span data-stu-id="48f05-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="48f05-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="48f05-119">JSON Representation</span></span>
<span data-ttu-id="48f05-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="48f05-120">Here is a JSON representation of the resource.</span></span>
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





