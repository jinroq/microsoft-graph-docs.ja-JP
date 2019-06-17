---
title: windowsKioskAzureADGroup リソースの種類
description: キオスク構成の AzureAD グループを識別するために使用されるクラス
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a80ef23c94424b79d1392cd5632f8dce85f675d1
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978522"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="f7aba-103">windowsKioskAzureADGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f7aba-103">windowsKioskAzureADGroup resource type</span></span>

> <span data-ttu-id="f7aba-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f7aba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7aba-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f7aba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7aba-106">キオスク構成の AzureAD グループを識別するために使用されるクラス</span><span class="sxs-lookup"><span data-stu-id="f7aba-106">The class used to identify an AzureAD group for the kiosk configuration</span></span>


<span data-ttu-id="f7aba-107">[Windowskioskuser](../resources/intune-deviceconfig-windowskioskuser.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="f7aba-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f7aba-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f7aba-108">Properties</span></span>
|<span data-ttu-id="f7aba-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f7aba-109">Property</span></span>|<span data-ttu-id="f7aba-110">型</span><span class="sxs-lookup"><span data-stu-id="f7aba-110">Type</span></span>|<span data-ttu-id="f7aba-111">説明</span><span class="sxs-lookup"><span data-stu-id="f7aba-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7aba-112">displayName</span><span class="sxs-lookup"><span data-stu-id="f7aba-112">displayName</span></span>|<span data-ttu-id="f7aba-113">String</span><span class="sxs-lookup"><span data-stu-id="f7aba-113">String</span></span>|<span data-ttu-id="f7aba-114">このキオスク構成にロックされる AzureAD グループの表示名。</span><span class="sxs-lookup"><span data-stu-id="f7aba-114">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="f7aba-115">groupId</span><span class="sxs-lookup"><span data-stu-id="f7aba-115">groupId</span></span>|<span data-ttu-id="f7aba-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f7aba-116">String</span></span>|<span data-ttu-id="f7aba-117">このキオスク構成にロックされる AzureAD グループの ID</span><span class="sxs-lookup"><span data-stu-id="f7aba-117">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7aba-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f7aba-118">Relationships</span></span>
<span data-ttu-id="f7aba-119">なし</span><span class="sxs-lookup"><span data-stu-id="f7aba-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7aba-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f7aba-120">JSON Representation</span></span>
<span data-ttu-id="f7aba-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f7aba-121">Here is a JSON representation of the resource.</span></span>
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





