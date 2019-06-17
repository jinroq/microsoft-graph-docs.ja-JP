---
title: edgeHomeButtonOpensCustomURL リソースの種類
description: '[ホーム] ボタンを表示します。[ホーム] ボタンをクリックすると、特定の URL が読み込まれます。'
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f16f883622ace795628d7c34214cc4b5d12017e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989795"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="358e9-103">edgeHomeButtonOpensCustomURL リソースの種類</span><span class="sxs-lookup"><span data-stu-id="358e9-103">edgeHomeButtonOpensCustomURL resource type</span></span>

> <span data-ttu-id="358e9-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="358e9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="358e9-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="358e9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="358e9-106">[ホーム] ボタンを表示します。[ホーム] ボタンをクリックすると、特定の URL が読み込まれます。</span><span class="sxs-lookup"><span data-stu-id="358e9-106">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="358e9-107">[EdgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="358e9-107">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="358e9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="358e9-108">Properties</span></span>
|<span data-ttu-id="358e9-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="358e9-109">Property</span></span>|<span data-ttu-id="358e9-110">型</span><span class="sxs-lookup"><span data-stu-id="358e9-110">Type</span></span>|<span data-ttu-id="358e9-111">説明</span><span class="sxs-lookup"><span data-stu-id="358e9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="358e9-112">ホームボタン Customurl</span><span class="sxs-lookup"><span data-stu-id="358e9-112">homeButtonCustomURL</span></span>|<span data-ttu-id="358e9-113">String</span><span class="sxs-lookup"><span data-stu-id="358e9-113">String</span></span>|<span data-ttu-id="358e9-114">読み込む特定の URL。</span><span class="sxs-lookup"><span data-stu-id="358e9-114">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="358e9-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="358e9-115">Relationships</span></span>
<span data-ttu-id="358e9-116">なし</span><span class="sxs-lookup"><span data-stu-id="358e9-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="358e9-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="358e9-117">JSON Representation</span></span>
<span data-ttu-id="358e9-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="358e9-118">Here is a JSON representation of the resource.</span></span>
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





