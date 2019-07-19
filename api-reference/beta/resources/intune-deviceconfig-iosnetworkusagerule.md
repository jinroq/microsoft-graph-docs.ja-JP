---
title: iosNetworkUsageRule リソースの種類
description: ネットワーク使用規則により、企業は管理対象アプリで携帯電話会社の回線などのネットワークをどのように使用するかを指定できます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2dc693eb993e6740098ab90dcae53214d8af4d0c
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995694"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="ccd5a-103">iosNetworkUsageRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ccd5a-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="ccd5a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ccd5a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ccd5a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ccd5a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccd5a-106">ネットワーク使用規則により、企業は管理対象アプリで携帯電話会社の回線などのネットワークをどのように使用するかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="ccd5a-106">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="ccd5a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ccd5a-107">Properties</span></span>
|<span data-ttu-id="ccd5a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ccd5a-108">Property</span></span>|<span data-ttu-id="ccd5a-109">型</span><span class="sxs-lookup"><span data-stu-id="ccd5a-109">Type</span></span>|<span data-ttu-id="ccd5a-110">説明</span><span class="sxs-lookup"><span data-stu-id="ccd5a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccd5a-111">managedApps</span><span class="sxs-lookup"><span data-stu-id="ccd5a-111">managedApps</span></span>|<span data-ttu-id="ccd5a-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ccd5a-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="ccd5a-113">このルールが適用される管理対象アプリに関する情報です。</span><span class="sxs-lookup"><span data-stu-id="ccd5a-113">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="ccd5a-114">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="ccd5a-114">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ccd5a-115">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="ccd5a-115">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="ccd5a-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="ccd5a-116">Boolean</span></span>|<span data-ttu-id="ccd5a-117">true に設定すると、ローミングの際、対応する管理対象アプリで携帯電話データを使用できなくなります。</span><span class="sxs-lookup"><span data-stu-id="ccd5a-117">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="ccd5a-118">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="ccd5a-118">cellularDataBlocked</span></span>|<span data-ttu-id="ccd5a-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="ccd5a-119">Boolean</span></span>|<span data-ttu-id="ccd5a-120">true に設定すると、いかなる場合でも、対応する管理対象アプリで携帯電話データを使用できなくなります。</span><span class="sxs-lookup"><span data-stu-id="ccd5a-120">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ccd5a-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ccd5a-121">Relationships</span></span>
<span data-ttu-id="ccd5a-122">なし</span><span class="sxs-lookup"><span data-stu-id="ccd5a-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ccd5a-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ccd5a-123">JSON Representation</span></span>
<span data-ttu-id="ccd5a-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ccd5a-124">Here is a JSON representation of the resource.</span></span>
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





