---
title: unsupportedDeviceConfigurationDetail リソースの種類
description: エンティティがサポートされている理由の説明です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6b82dcf28652cbe54a4932a641579101cb392639
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949774"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="c385c-103">unsupportedDeviceConfigurationDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c385c-103">unsupportedDeviceConfigurationDetail resource type</span></span>

> <span data-ttu-id="c385c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c385c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c385c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c385c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c385c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c385c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c385c-107">エンティティがサポートされている理由の説明です。</span><span class="sxs-lookup"><span data-stu-id="c385c-107">A description of why an entity is unsupported.</span></span>
## <a name="properties"></a><span data-ttu-id="c385c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c385c-108">Properties</span></span>
|<span data-ttu-id="c385c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c385c-109">Property</span></span>|<span data-ttu-id="c385c-110">種類</span><span class="sxs-lookup"><span data-stu-id="c385c-110">Type</span></span>|<span data-ttu-id="c385c-111">説明</span><span class="sxs-lookup"><span data-stu-id="c385c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c385c-112">message</span><span class="sxs-lookup"><span data-stu-id="c385c-112">message</span></span>|<span data-ttu-id="c385c-113">String</span><span class="sxs-lookup"><span data-stu-id="c385c-113">String</span></span>|<span data-ttu-id="c385c-114">エンティティがサポートされている理由を説明するメッセージ。</span><span class="sxs-lookup"><span data-stu-id="c385c-114">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="c385c-115">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="c385c-115">propertyName</span></span>|<span data-ttu-id="c385c-116">String</span><span class="sxs-lookup"><span data-stu-id="c385c-116">String</span></span>|<span data-ttu-id="c385c-117">メッセージが元のエンティティでは、そのプロパティの名前に特定のプロパティに関連しています。</span><span class="sxs-lookup"><span data-stu-id="c385c-117">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c385c-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c385c-118">Relationships</span></span>
<span data-ttu-id="c385c-119">なし</span><span class="sxs-lookup"><span data-stu-id="c385c-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c385c-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c385c-120">JSON Representation</span></span>
<span data-ttu-id="c385c-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c385c-121">Here is a JSON representation of the resource.</span></span>
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





