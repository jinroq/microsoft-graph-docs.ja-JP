---
title: iosHomeScreenItem リソースの種類
description: IOS ホーム画面上のアイテムを表します
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 832b38b7b27c810c78db07bedcd8083d8b203070
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139950"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="42463-103">iosHomeScreenItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="42463-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="42463-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="42463-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42463-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="42463-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42463-106">IOS ホーム画面上のアイテムを表します</span><span class="sxs-lookup"><span data-stu-id="42463-106">Represents an item on the iOS Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="42463-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42463-107">Properties</span></span>
|<span data-ttu-id="42463-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42463-108">Property</span></span>|<span data-ttu-id="42463-109">型</span><span class="sxs-lookup"><span data-stu-id="42463-109">Type</span></span>|<span data-ttu-id="42463-110">説明</span><span class="sxs-lookup"><span data-stu-id="42463-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42463-111">displayName</span><span class="sxs-lookup"><span data-stu-id="42463-111">displayName</span></span>|<span data-ttu-id="42463-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="42463-112">String</span></span>|<span data-ttu-id="42463-113">アプリの名前</span><span class="sxs-lookup"><span data-stu-id="42463-113">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="42463-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="42463-114">Relationships</span></span>
<span data-ttu-id="42463-115">なし</span><span class="sxs-lookup"><span data-stu-id="42463-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="42463-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="42463-116">JSON Representation</span></span>
<span data-ttu-id="42463-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="42463-117">Here is a JSON representation of the resource.</span></span>
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




