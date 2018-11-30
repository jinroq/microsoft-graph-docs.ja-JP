---
title: iosNetworkUsageRule リソースの種類
description: ネットワーク使用規則により、企業は管理対象アプリで携帯電話会社の回線などのネットワークをどのように使用するかを指定できます。
ms.openlocfilehash: 211cbc52f596bbe62647a14c84bd5fd5178fdfc6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023966"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="efc45-103">iosNetworkUsageRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="efc45-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="efc45-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="efc45-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="efc45-105">ネットワーク使用規則により、企業は管理対象アプリで携帯電話会社の回線などのネットワークをどのように使用するかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="efc45-105">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>
## <a name="properties"></a><span data-ttu-id="efc45-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="efc45-106">Properties</span></span>
|<span data-ttu-id="efc45-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="efc45-107">Property</span></span>|<span data-ttu-id="efc45-108">型</span><span class="sxs-lookup"><span data-stu-id="efc45-108">Type</span></span>|<span data-ttu-id="efc45-109">説明</span><span class="sxs-lookup"><span data-stu-id="efc45-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efc45-110">managedApps</span><span class="sxs-lookup"><span data-stu-id="efc45-110">managedApps</span></span>|<span data-ttu-id="efc45-111">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="efc45-111">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="efc45-112">このルールが適用される管理対象アプリに関する情報です。</span><span class="sxs-lookup"><span data-stu-id="efc45-112">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="efc45-113">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="efc45-113">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="efc45-114">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="efc45-114">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="efc45-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="efc45-115">Boolean</span></span>|<span data-ttu-id="efc45-116">true に設定すると、ローミングの際、対応する管理対象アプリで携帯電話データを使用できなくなります。</span><span class="sxs-lookup"><span data-stu-id="efc45-116">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="efc45-117">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="efc45-117">cellularDataBlocked</span></span>|<span data-ttu-id="efc45-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="efc45-118">Boolean</span></span>|<span data-ttu-id="efc45-119">true に設定すると、いかなる場合でも、対応する管理対象アプリで携帯電話データを使用できなくなります。</span><span class="sxs-lookup"><span data-stu-id="efc45-119">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="efc45-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="efc45-120">Relationships</span></span>
<span data-ttu-id="efc45-121">なし</span><span class="sxs-lookup"><span data-stu-id="efc45-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="efc45-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="efc45-122">JSON Representation</span></span>
<span data-ttu-id="efc45-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="efc45-123">Here is a JSON representation of the resource.</span></span>
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



