---
title: iosNetworkUsageRule リソースの種類
description: ネットワーク使用規則により、企業は管理対象アプリで携帯電話会社の回線などのネットワークをどのように使用するかを指定できます。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 057ddb8027835702cdb487387efafb73cb986c2e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964845"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="bf7cf-103">iosNetworkUsageRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bf7cf-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="bf7cf-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bf7cf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bf7cf-105">ネットワーク使用規則により、企業は管理対象アプリで携帯電話会社の回線などのネットワークをどのように使用するかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="bf7cf-105">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>
## <a name="properties"></a><span data-ttu-id="bf7cf-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf7cf-106">Properties</span></span>
|<span data-ttu-id="bf7cf-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf7cf-107">Property</span></span>|<span data-ttu-id="bf7cf-108">種類</span><span class="sxs-lookup"><span data-stu-id="bf7cf-108">Type</span></span>|<span data-ttu-id="bf7cf-109">説明</span><span class="sxs-lookup"><span data-stu-id="bf7cf-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf7cf-110">managedApps</span><span class="sxs-lookup"><span data-stu-id="bf7cf-110">managedApps</span></span>|<span data-ttu-id="bf7cf-111">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bf7cf-111">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="bf7cf-112">このルールが適用される管理対象アプリに関する情報です。</span><span class="sxs-lookup"><span data-stu-id="bf7cf-112">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="bf7cf-113">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="bf7cf-113">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="bf7cf-114">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="bf7cf-114">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="bf7cf-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf7cf-115">Boolean</span></span>|<span data-ttu-id="bf7cf-116">true に設定すると、ローミングの際、対応する管理対象アプリで携帯電話データを使用できなくなります。</span><span class="sxs-lookup"><span data-stu-id="bf7cf-116">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="bf7cf-117">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="bf7cf-117">cellularDataBlocked</span></span>|<span data-ttu-id="bf7cf-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf7cf-118">Boolean</span></span>|<span data-ttu-id="bf7cf-119">true に設定すると、いかなる場合でも、対応する管理対象アプリで携帯電話データを使用できなくなります。</span><span class="sxs-lookup"><span data-stu-id="bf7cf-119">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf7cf-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bf7cf-120">Relationships</span></span>
<span data-ttu-id="bf7cf-121">なし</span><span class="sxs-lookup"><span data-stu-id="bf7cf-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bf7cf-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bf7cf-122">JSON Representation</span></span>
<span data-ttu-id="bf7cf-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bf7cf-123">Here is a JSON representation of the resource.</span></span>
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



