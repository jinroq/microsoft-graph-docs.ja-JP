---
title: edgeHomeButtonOpensCustomURL リソースの種類
description: '[ホーム] ボタンを表示します。[ホーム] ボタンをクリックすると、特定の URL が読み込まれます。'
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e83fd3dbb0961011584ef9d65e01c361ccf6a228
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143240"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="a9614-103">edgeHomeButtonOpensCustomURL リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a9614-103">edgeHomeButtonOpensCustomURL resource type</span></span>

> <span data-ttu-id="a9614-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9614-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9614-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a9614-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9614-106">[ホーム] ボタンを表示します。[ホーム] ボタンをクリックすると、特定の URL が読み込まれます。</span><span class="sxs-lookup"><span data-stu-id="a9614-106">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="a9614-107">[edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="a9614-107">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a9614-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9614-108">Properties</span></span>
|<span data-ttu-id="a9614-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9614-109">Property</span></span>|<span data-ttu-id="a9614-110">型</span><span class="sxs-lookup"><span data-stu-id="a9614-110">Type</span></span>|<span data-ttu-id="a9614-111">説明</span><span class="sxs-lookup"><span data-stu-id="a9614-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9614-112">ホームボタン customurl</span><span class="sxs-lookup"><span data-stu-id="a9614-112">homeButtonCustomURL</span></span>|<span data-ttu-id="a9614-113">String</span><span class="sxs-lookup"><span data-stu-id="a9614-113">String</span></span>|<span data-ttu-id="a9614-114">読み込む特定の URL。</span><span class="sxs-lookup"><span data-stu-id="a9614-114">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9614-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a9614-115">Relationships</span></span>
<span data-ttu-id="a9614-116">なし</span><span class="sxs-lookup"><span data-stu-id="a9614-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9614-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a9614-117">JSON Representation</span></span>
<span data-ttu-id="a9614-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a9614-118">Here is a JSON representation of the resource.</span></span>
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




