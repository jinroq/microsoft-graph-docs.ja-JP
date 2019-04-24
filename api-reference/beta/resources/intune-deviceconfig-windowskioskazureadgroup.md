---
title: windowsKioskAzureADGroup リソースの種類
description: キオスク構成の AzureAD グループを識別するために使用されるクラス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a3224f55f4a5158fb8c0850a4dbea7e6bcf8d18d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522434"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="6cd28-103">windowsKioskAzureADGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6cd28-103">windowsKioskAzureADGroup resource type</span></span>

> <span data-ttu-id="6cd28-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6cd28-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6cd28-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6cd28-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cd28-106">キオスク構成の AzureAD グループを識別するために使用されるクラス</span><span class="sxs-lookup"><span data-stu-id="6cd28-106">The class used to identify an AzureAD group for the kiosk configuration</span></span>


<span data-ttu-id="6cd28-107">[windowskioskuser](../resources/intune-deviceconfig-windowskioskuser.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="6cd28-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6cd28-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6cd28-108">Properties</span></span>
|<span data-ttu-id="6cd28-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6cd28-109">Property</span></span>|<span data-ttu-id="6cd28-110">型</span><span class="sxs-lookup"><span data-stu-id="6cd28-110">Type</span></span>|<span data-ttu-id="6cd28-111">説明</span><span class="sxs-lookup"><span data-stu-id="6cd28-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cd28-112">displayName</span><span class="sxs-lookup"><span data-stu-id="6cd28-112">displayName</span></span>|<span data-ttu-id="6cd28-113">String</span><span class="sxs-lookup"><span data-stu-id="6cd28-113">String</span></span>|<span data-ttu-id="6cd28-114">このキオスク構成にロックされる AzureAD グループの表示名。</span><span class="sxs-lookup"><span data-stu-id="6cd28-114">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="6cd28-115">groupId</span><span class="sxs-lookup"><span data-stu-id="6cd28-115">groupId</span></span>|<span data-ttu-id="6cd28-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="6cd28-116">String</span></span>|<span data-ttu-id="6cd28-117">このキオスク構成にロックされる AzureAD グループの ID</span><span class="sxs-lookup"><span data-stu-id="6cd28-117">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="6cd28-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6cd28-118">Relationships</span></span>
<span data-ttu-id="6cd28-119">なし</span><span class="sxs-lookup"><span data-stu-id="6cd28-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6cd28-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6cd28-120">JSON Representation</span></span>
<span data-ttu-id="6cd28-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6cd28-121">Here is a JSON representation of the resource.</span></span>
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





