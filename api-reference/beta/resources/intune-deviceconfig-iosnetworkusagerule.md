---
title: iosNetworkUsageRule リソースの種類
description: ネットワーク使用規則により、企業は管理対象アプリで携帯電話会社の回線などのネットワークをどのように使用するかを指定できます。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0a287fcf8be771037a39efd821f5468acf518371
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398325"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="3eaa3-103">iosNetworkUsageRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3eaa3-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="3eaa3-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3eaa3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3eaa3-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3eaa3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3eaa3-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3eaa3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3eaa3-107">ネットワーク使用規則により、企業は管理対象アプリで携帯電話会社の回線などのネットワークをどのように使用するかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="3eaa3-107">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="3eaa3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3eaa3-108">Properties</span></span>
|<span data-ttu-id="3eaa3-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3eaa3-109">Property</span></span>|<span data-ttu-id="3eaa3-110">型</span><span class="sxs-lookup"><span data-stu-id="3eaa3-110">Type</span></span>|<span data-ttu-id="3eaa3-111">説明</span><span class="sxs-lookup"><span data-stu-id="3eaa3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3eaa3-112">managedApps</span><span class="sxs-lookup"><span data-stu-id="3eaa3-112">managedApps</span></span>|<span data-ttu-id="3eaa3-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3eaa3-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="3eaa3-114">このルールが適用される管理対象アプリに関する情報です。</span><span class="sxs-lookup"><span data-stu-id="3eaa3-114">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="3eaa3-115">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="3eaa3-115">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3eaa3-116">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="3eaa3-116">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="3eaa3-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="3eaa3-117">Boolean</span></span>|<span data-ttu-id="3eaa3-118">true に設定すると、ローミングの際、対応する管理対象アプリで携帯電話データを使用できなくなります。</span><span class="sxs-lookup"><span data-stu-id="3eaa3-118">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="3eaa3-119">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="3eaa3-119">cellularDataBlocked</span></span>|<span data-ttu-id="3eaa3-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="3eaa3-120">Boolean</span></span>|<span data-ttu-id="3eaa3-121">true に設定すると、いかなる場合でも、対応する管理対象アプリで携帯電話データを使用できなくなります。</span><span class="sxs-lookup"><span data-stu-id="3eaa3-121">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3eaa3-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3eaa3-122">Relationships</span></span>
<span data-ttu-id="3eaa3-123">なし</span><span class="sxs-lookup"><span data-stu-id="3eaa3-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3eaa3-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3eaa3-124">JSON Representation</span></span>
<span data-ttu-id="3eaa3-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3eaa3-125">Here is a JSON representation of the resource.</span></span>
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




