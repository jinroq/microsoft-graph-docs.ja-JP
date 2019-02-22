---
title: windowsKioskAzureADGroup リソースの種類
description: キオスク構成の AzureAD グループを識別するために使用されるクラス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f05bf9d01e8442a54c9fa70b863e3789309bd9d4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175137"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="7da87-103">windowsKioskAzureADGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7da87-103">windowsKioskAzureADGroup resource type</span></span>

> <span data-ttu-id="7da87-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7da87-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7da87-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7da87-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7da87-106">キオスク構成の AzureAD グループを識別するために使用されるクラス</span><span class="sxs-lookup"><span data-stu-id="7da87-106">The class used to identify an AzureAD group for the kiosk configuration</span></span>


<span data-ttu-id="7da87-107">[windowskioskuser](../resources/intune-deviceconfig-windowskioskuser.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="7da87-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7da87-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7da87-108">Properties</span></span>
|<span data-ttu-id="7da87-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7da87-109">Property</span></span>|<span data-ttu-id="7da87-110">型</span><span class="sxs-lookup"><span data-stu-id="7da87-110">Type</span></span>|<span data-ttu-id="7da87-111">説明</span><span class="sxs-lookup"><span data-stu-id="7da87-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7da87-112">displayName</span><span class="sxs-lookup"><span data-stu-id="7da87-112">displayName</span></span>|<span data-ttu-id="7da87-113">String</span><span class="sxs-lookup"><span data-stu-id="7da87-113">String</span></span>|<span data-ttu-id="7da87-114">このキオスク構成にロックされる AzureAD グループの表示名。</span><span class="sxs-lookup"><span data-stu-id="7da87-114">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="7da87-115">groupId</span><span class="sxs-lookup"><span data-stu-id="7da87-115">groupId</span></span>|<span data-ttu-id="7da87-116">String</span><span class="sxs-lookup"><span data-stu-id="7da87-116">String</span></span>|<span data-ttu-id="7da87-117">このキオスク構成にロックされる AzureAD グループの ID</span><span class="sxs-lookup"><span data-stu-id="7da87-117">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="7da87-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7da87-118">Relationships</span></span>
<span data-ttu-id="7da87-119">なし</span><span class="sxs-lookup"><span data-stu-id="7da87-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7da87-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7da87-120">JSON Representation</span></span>
<span data-ttu-id="7da87-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7da87-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADGroup",
  "displayName": "String",
  "groupId": "String"
}
```




