---
title: unsupportedDeviceConfigurationDetail リソースの種類
description: エンティティがサポートされている理由の説明です。
author: tfitzmac
ms.openlocfilehash: 4cccf49366a803e5f964605a4dc4ba7f56707823
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344052"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="80566-103">unsupportedDeviceConfigurationDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="80566-103">unsupportedDeviceConfigurationDetail resource type</span></span>

> <span data-ttu-id="80566-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="80566-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80566-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80566-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="80566-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="80566-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80566-107">エンティティがサポートされている理由の説明です。</span><span class="sxs-lookup"><span data-stu-id="80566-107">A description of why an entity is unsupported.</span></span>
## <a name="properties"></a><span data-ttu-id="80566-108">Properties</span><span class="sxs-lookup"><span data-stu-id="80566-108">Properties</span></span>
|<span data-ttu-id="80566-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="80566-109">Property</span></span>|<span data-ttu-id="80566-110">種類</span><span class="sxs-lookup"><span data-stu-id="80566-110">Type</span></span>|<span data-ttu-id="80566-111">説明</span><span class="sxs-lookup"><span data-stu-id="80566-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80566-112">message</span><span class="sxs-lookup"><span data-stu-id="80566-112">message</span></span>|<span data-ttu-id="80566-113">String</span><span class="sxs-lookup"><span data-stu-id="80566-113">String</span></span>|<span data-ttu-id="80566-114">エンティティがサポートされている理由を説明するメッセージ。</span><span class="sxs-lookup"><span data-stu-id="80566-114">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="80566-115">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="80566-115">propertyName</span></span>|<span data-ttu-id="80566-116">String</span><span class="sxs-lookup"><span data-stu-id="80566-116">String</span></span>|<span data-ttu-id="80566-117">メッセージが元のエンティティでは、そのプロパティの名前に特定のプロパティに関連しています。</span><span class="sxs-lookup"><span data-stu-id="80566-117">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80566-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="80566-118">Relationships</span></span>
<span data-ttu-id="80566-119">なし</span><span class="sxs-lookup"><span data-stu-id="80566-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="80566-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="80566-120">JSON Representation</span></span>
<span data-ttu-id="80566-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="80566-121">Here is a JSON representation of the resource.</span></span>
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





