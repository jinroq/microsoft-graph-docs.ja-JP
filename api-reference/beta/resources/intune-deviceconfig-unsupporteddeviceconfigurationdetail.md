---
title: unsupportedDeviceConfigurationDetail リソースの種類
description: エンティティがサポートされている理由の説明です。
ms.openlocfilehash: d64d6aedf5da0f3cd79e2582d84fa4f19ea7ccfa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068054"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="ecbd0-103">unsupportedDeviceConfigurationDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ecbd0-103">unsupportedDeviceConfigurationDetail resource type</span></span>

> <span data-ttu-id="ecbd0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ecbd0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ecbd0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ecbd0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ecbd0-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ecbd0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ecbd0-107">エンティティがサポートされている理由の説明です。</span><span class="sxs-lookup"><span data-stu-id="ecbd0-107">A description of why an entity is unsupported.</span></span>
## <a name="properties"></a><span data-ttu-id="ecbd0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ecbd0-108">Properties</span></span>
|<span data-ttu-id="ecbd0-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ecbd0-109">Property</span></span>|<span data-ttu-id="ecbd0-110">型</span><span class="sxs-lookup"><span data-stu-id="ecbd0-110">Type</span></span>|<span data-ttu-id="ecbd0-111">説明</span><span class="sxs-lookup"><span data-stu-id="ecbd0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecbd0-112">message</span><span class="sxs-lookup"><span data-stu-id="ecbd0-112">message</span></span>|<span data-ttu-id="ecbd0-113">String</span><span class="sxs-lookup"><span data-stu-id="ecbd0-113">String</span></span>|<span data-ttu-id="ecbd0-114">エンティティがサポートされている理由を説明するメッセージ。</span><span class="sxs-lookup"><span data-stu-id="ecbd0-114">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="ecbd0-115">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="ecbd0-115">propertyName</span></span>|<span data-ttu-id="ecbd0-116">String</span><span class="sxs-lookup"><span data-stu-id="ecbd0-116">String</span></span>|<span data-ttu-id="ecbd0-117">メッセージが元のエンティティでは、そのプロパティの名前に特定のプロパティに関連しています。</span><span class="sxs-lookup"><span data-stu-id="ecbd0-117">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ecbd0-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ecbd0-118">Relationships</span></span>
<span data-ttu-id="ecbd0-119">なし</span><span class="sxs-lookup"><span data-stu-id="ecbd0-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ecbd0-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ecbd0-120">JSON Representation</span></span>
<span data-ttu-id="ecbd0-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ecbd0-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfigurationDetail",
  "message": "String",
  "propertyName": "String"
}
```





