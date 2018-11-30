---
title: iosNetworkUsageRule リソースの種類
description: ネットワーク使用規則により、企業は管理対象アプリで携帯電話会社の回線などのネットワークをどのように使用するかを指定できます。
ms.openlocfilehash: 93cfd1f5eefe6f32fd0b112b24e3cdfba6969434
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070649"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="fd870-103">iosNetworkUsageRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fd870-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="fd870-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fd870-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd870-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd870-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fd870-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fd870-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd870-107">ネットワーク使用規則により、企業は管理対象アプリで携帯電話会社の回線などのネットワークをどのように使用するかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="fd870-107">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>
## <a name="properties"></a><span data-ttu-id="fd870-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd870-108">Properties</span></span>
|<span data-ttu-id="fd870-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd870-109">Property</span></span>|<span data-ttu-id="fd870-110">型</span><span class="sxs-lookup"><span data-stu-id="fd870-110">Type</span></span>|<span data-ttu-id="fd870-111">説明</span><span class="sxs-lookup"><span data-stu-id="fd870-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd870-112">managedApps</span><span class="sxs-lookup"><span data-stu-id="fd870-112">managedApps</span></span>|<span data-ttu-id="fd870-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fd870-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="fd870-114">このルールが適用される管理対象アプリに関する情報です。</span><span class="sxs-lookup"><span data-stu-id="fd870-114">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="fd870-115">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="fd870-115">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="fd870-116">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="fd870-116">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="fd870-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd870-117">Boolean</span></span>|<span data-ttu-id="fd870-118">true に設定すると、ローミングの際、対応する管理対象アプリで携帯電話データを使用できなくなります。</span><span class="sxs-lookup"><span data-stu-id="fd870-118">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="fd870-119">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="fd870-119">cellularDataBlocked</span></span>|<span data-ttu-id="fd870-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd870-120">Boolean</span></span>|<span data-ttu-id="fd870-121">true に設定すると、いかなる場合でも、対応する管理対象アプリで携帯電話データを使用できなくなります。</span><span class="sxs-lookup"><span data-stu-id="fd870-121">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd870-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fd870-122">Relationships</span></span>
<span data-ttu-id="fd870-123">なし</span><span class="sxs-lookup"><span data-stu-id="fd870-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fd870-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fd870-124">JSON Representation</span></span>
<span data-ttu-id="fd870-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fd870-125">Here is a JSON representation of the resource.</span></span>
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





