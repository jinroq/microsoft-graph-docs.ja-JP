---
title: edgeHomeButtonOpensCustomURL リソースの種類
description: '[ホーム] ボタンを表示します。[ホーム] ボタンをクリックすると、特定の URL が読み込まれます。'
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2dad4baba5fd55b99efd6b2b7ebadf1973d6c9c8
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31783716"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="24729-103">edgeHomeButtonOpensCustomURL リソースの種類</span><span class="sxs-lookup"><span data-stu-id="24729-103">edgeHomeButtonOpensCustomURL resource type</span></span>

> <span data-ttu-id="24729-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24729-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24729-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="24729-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24729-106">[ホーム] ボタンを表示します。[ホーム] ボタンをクリックすると、特定の URL が読み込まれます。</span><span class="sxs-lookup"><span data-stu-id="24729-106">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="24729-107">[edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="24729-107">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="24729-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24729-108">Properties</span></span>
|<span data-ttu-id="24729-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24729-109">Property</span></span>|<span data-ttu-id="24729-110">型</span><span class="sxs-lookup"><span data-stu-id="24729-110">Type</span></span>|<span data-ttu-id="24729-111">説明</span><span class="sxs-lookup"><span data-stu-id="24729-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24729-112">ホームボタン customurl</span><span class="sxs-lookup"><span data-stu-id="24729-112">homeButtonCustomURL</span></span>|<span data-ttu-id="24729-113">文字列</span><span class="sxs-lookup"><span data-stu-id="24729-113">String</span></span>|<span data-ttu-id="24729-114">読み込む特定の URL。</span><span class="sxs-lookup"><span data-stu-id="24729-114">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="24729-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="24729-115">Relationships</span></span>
<span data-ttu-id="24729-116">なし</span><span class="sxs-lookup"><span data-stu-id="24729-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="24729-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="24729-117">JSON Representation</span></span>
<span data-ttu-id="24729-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="24729-118">Here is a JSON representation of the resource.</span></span>
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





