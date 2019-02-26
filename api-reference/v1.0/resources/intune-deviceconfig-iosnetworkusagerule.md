---
title: iosNetworkUsageRule リソースの種類
description: ネットワーク使用規則により、企業は管理対象アプリで携帯電話会社の回線などのネットワークをどのように使用するかを指定できます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 516e880e4b6230ca165426b849f57609dcc6e6ad
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250104"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="636ec-103">iosNetworkUsageRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="636ec-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="636ec-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="636ec-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="636ec-105">ネットワーク使用規則により、企業は管理対象アプリで携帯電話会社の回線などのネットワークをどのように使用するかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="636ec-105">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="636ec-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="636ec-106">Properties</span></span>
|<span data-ttu-id="636ec-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="636ec-107">Property</span></span>|<span data-ttu-id="636ec-108">型</span><span class="sxs-lookup"><span data-stu-id="636ec-108">Type</span></span>|<span data-ttu-id="636ec-109">説明</span><span class="sxs-lookup"><span data-stu-id="636ec-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="636ec-110">managedApps</span><span class="sxs-lookup"><span data-stu-id="636ec-110">managedApps</span></span>|<span data-ttu-id="636ec-111">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="636ec-111">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="636ec-112">このルールが適用される管理対象アプリに関する情報です。</span><span class="sxs-lookup"><span data-stu-id="636ec-112">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="636ec-113">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="636ec-113">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="636ec-114">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="636ec-114">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="636ec-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="636ec-115">Boolean</span></span>|<span data-ttu-id="636ec-116">true に設定すると、ローミングの際、対応する管理対象アプリで携帯電話データを使用できなくなります。</span><span class="sxs-lookup"><span data-stu-id="636ec-116">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="636ec-117">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="636ec-117">cellularDataBlocked</span></span>|<span data-ttu-id="636ec-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="636ec-118">Boolean</span></span>|<span data-ttu-id="636ec-119">true に設定すると、いかなる場合でも、対応する管理対象アプリで携帯電話データを使用できなくなります。</span><span class="sxs-lookup"><span data-stu-id="636ec-119">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="636ec-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="636ec-120">Relationships</span></span>
<span data-ttu-id="636ec-121">なし</span><span class="sxs-lookup"><span data-stu-id="636ec-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="636ec-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="636ec-122">JSON Representation</span></span>
<span data-ttu-id="636ec-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="636ec-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNetworkUsageRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNetworkUsageRule",
  "managedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "cellularDataBlockWhenRoaming": true,
  "cellularDataBlocked": true
}
```



