---
title: managedAppPolicyDeploymentSummaryPerApp リソースの種類
description: アプリごとのポリシーの展開の概要を表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1174e46f40a7f80944cf686a403edb0db60cb1fd
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994728"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="f24aa-103">managedAppPolicyDeploymentSummaryPerApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f24aa-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="f24aa-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f24aa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f24aa-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f24aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f24aa-106">アプリごとのポリシーの展開の概要を表します。</span><span class="sxs-lookup"><span data-stu-id="f24aa-106">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="f24aa-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f24aa-107">Properties</span></span>
|<span data-ttu-id="f24aa-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f24aa-108">Property</span></span>|<span data-ttu-id="f24aa-109">型</span><span class="sxs-lookup"><span data-stu-id="f24aa-109">Type</span></span>|<span data-ttu-id="f24aa-110">説明</span><span class="sxs-lookup"><span data-stu-id="f24aa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f24aa-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="f24aa-111">mobileAppIdentifier</span></span>|[<span data-ttu-id="f24aa-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="f24aa-112">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="f24aa-113">アプリの展開</span><span class="sxs-lookup"><span data-stu-id="f24aa-113">Deployment of an app.</span></span>|
|<span data-ttu-id="f24aa-114">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="f24aa-114">configurationAppliedUserCount</span></span>|<span data-ttu-id="f24aa-115">Int32</span><span class="sxs-lookup"><span data-stu-id="f24aa-115">Int32</span></span>|<span data-ttu-id="f24aa-116">ポリシーが適用されているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="f24aa-116">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f24aa-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f24aa-117">Relationships</span></span>
<span data-ttu-id="f24aa-118">なし</span><span class="sxs-lookup"><span data-stu-id="f24aa-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f24aa-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f24aa-119">JSON Representation</span></span>
<span data-ttu-id="f24aa-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f24aa-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "configurationAppliedUserCount": 1024
}
```





