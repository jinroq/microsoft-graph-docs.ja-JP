---
title: edgeHomeButtonOpensCustomURL リソースの種類
description: '[ホーム] ボタンを表示します。[ホーム] ボタンをクリックすると、特定の URL が読み込まれます。'
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3b82acaf8ef5f6e008d759f257c7382ff64492b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946820"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="c2963-103">edgeHomeButtonOpensCustomURL リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c2963-103">edgeHomeButtonOpensCustomURL resource type</span></span>

> <span data-ttu-id="c2963-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c2963-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2963-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c2963-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2963-106">[ホーム] ボタンを表示します。[ホーム] ボタンをクリックすると、特定の URL が読み込まれます。</span><span class="sxs-lookup"><span data-stu-id="c2963-106">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="c2963-107">[EdgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c2963-107">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c2963-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c2963-108">Properties</span></span>
|<span data-ttu-id="c2963-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c2963-109">Property</span></span>|<span data-ttu-id="c2963-110">型</span><span class="sxs-lookup"><span data-stu-id="c2963-110">Type</span></span>|<span data-ttu-id="c2963-111">説明</span><span class="sxs-lookup"><span data-stu-id="c2963-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2963-112">ホームボタン Customurl</span><span class="sxs-lookup"><span data-stu-id="c2963-112">homeButtonCustomURL</span></span>|<span data-ttu-id="c2963-113">String</span><span class="sxs-lookup"><span data-stu-id="c2963-113">String</span></span>|<span data-ttu-id="c2963-114">読み込む特定の URL。</span><span class="sxs-lookup"><span data-stu-id="c2963-114">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2963-115">関係</span><span class="sxs-lookup"><span data-stu-id="c2963-115">Relationships</span></span>
<span data-ttu-id="c2963-116">なし</span><span class="sxs-lookup"><span data-stu-id="c2963-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2963-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c2963-117">JSON Representation</span></span>
<span data-ttu-id="c2963-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c2963-118">Here is a JSON representation of the resource.</span></span>
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




