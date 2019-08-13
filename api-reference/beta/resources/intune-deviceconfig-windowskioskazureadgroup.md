---
title: windowsKioskAzureADGroup リソースの種類
description: キオスク構成の AzureAD グループを識別するために使用されるクラス
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 00cd2f43fb09df03dfe2f5ee1810871dc2b77fb2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370943"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="13454-103">windowsKioskAzureADGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="13454-103">windowsKioskAzureADGroup resource type</span></span>

> <span data-ttu-id="13454-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13454-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13454-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="13454-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13454-106">キオスク構成の AzureAD グループを識別するために使用されるクラス</span><span class="sxs-lookup"><span data-stu-id="13454-106">The class used to identify an AzureAD group for the kiosk configuration</span></span>


<span data-ttu-id="13454-107">[Windowskioskuser](../resources/intune-deviceconfig-windowskioskuser.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="13454-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="13454-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13454-108">Properties</span></span>
|<span data-ttu-id="13454-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13454-109">Property</span></span>|<span data-ttu-id="13454-110">型</span><span class="sxs-lookup"><span data-stu-id="13454-110">Type</span></span>|<span data-ttu-id="13454-111">説明</span><span class="sxs-lookup"><span data-stu-id="13454-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13454-112">displayName</span><span class="sxs-lookup"><span data-stu-id="13454-112">displayName</span></span>|<span data-ttu-id="13454-113">String</span><span class="sxs-lookup"><span data-stu-id="13454-113">String</span></span>|<span data-ttu-id="13454-114">このキオスク構成にロックされる AzureAD グループの表示名。</span><span class="sxs-lookup"><span data-stu-id="13454-114">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="13454-115">groupId</span><span class="sxs-lookup"><span data-stu-id="13454-115">groupId</span></span>|<span data-ttu-id="13454-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="13454-116">String</span></span>|<span data-ttu-id="13454-117">このキオスク構成にロックされる AzureAD グループの ID</span><span class="sxs-lookup"><span data-stu-id="13454-117">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="13454-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="13454-118">Relationships</span></span>
<span data-ttu-id="13454-119">なし</span><span class="sxs-lookup"><span data-stu-id="13454-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13454-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="13454-120">JSON Representation</span></span>
<span data-ttu-id="13454-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="13454-121">Here is a JSON representation of the resource.</span></span>
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



