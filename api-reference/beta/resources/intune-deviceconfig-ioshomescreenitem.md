---
title: iosHomeScreenItem リソースの種類
description: IOS ホーム画面上のアイテムを表します
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b4685c62177dcb7d8cdf0f827d5af085d571d9b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31779735"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="47af2-103">iosHomeScreenItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="47af2-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="47af2-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47af2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47af2-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="47af2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47af2-106">IOS ホーム画面上のアイテムを表します</span><span class="sxs-lookup"><span data-stu-id="47af2-106">Represents an item on the iOS Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="47af2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="47af2-107">Properties</span></span>
|<span data-ttu-id="47af2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="47af2-108">Property</span></span>|<span data-ttu-id="47af2-109">型</span><span class="sxs-lookup"><span data-stu-id="47af2-109">Type</span></span>|<span data-ttu-id="47af2-110">説明</span><span class="sxs-lookup"><span data-stu-id="47af2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47af2-111">displayName</span><span class="sxs-lookup"><span data-stu-id="47af2-111">displayName</span></span>|<span data-ttu-id="47af2-112">String</span><span class="sxs-lookup"><span data-stu-id="47af2-112">String</span></span>|<span data-ttu-id="47af2-113">アプリの名前</span><span class="sxs-lookup"><span data-stu-id="47af2-113">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="47af2-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="47af2-114">Relationships</span></span>
<span data-ttu-id="47af2-115">なし</span><span class="sxs-lookup"><span data-stu-id="47af2-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="47af2-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="47af2-116">JSON Representation</span></span>
<span data-ttu-id="47af2-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="47af2-117">Here is a JSON representation of the resource.</span></span>
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





