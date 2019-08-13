---
title: configurationManagerClientInformation リソースの種類
description: SCCM から同期された Configuration manager クライアント情報
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ae7d36b353b989d4256294872fba4c4f225d2668
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371542"
---
# <a name="configurationmanagerclientinformation-resource-type"></a><span data-ttu-id="4b156-103">configurationManagerClientInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4b156-103">configurationManagerClientInformation resource type</span></span>

> <span data-ttu-id="4b156-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b156-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b156-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4b156-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b156-106">SCCM から同期された Configuration manager クライアント情報</span><span class="sxs-lookup"><span data-stu-id="4b156-106">Configuration manager client information synced from SCCM</span></span>

## <a name="properties"></a><span data-ttu-id="4b156-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b156-107">Properties</span></span>
|<span data-ttu-id="4b156-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b156-108">Property</span></span>|<span data-ttu-id="4b156-109">型</span><span class="sxs-lookup"><span data-stu-id="4b156-109">Type</span></span>|<span data-ttu-id="4b156-110">説明</span><span class="sxs-lookup"><span data-stu-id="4b156-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b156-111">clientIdentifier</span><span class="sxs-lookup"><span data-stu-id="4b156-111">clientIdentifier</span></span>|<span data-ttu-id="4b156-112">String</span><span class="sxs-lookup"><span data-stu-id="4b156-112">String</span></span>|<span data-ttu-id="4b156-113">SCCM からの Configuration Manager クライアント Id</span><span class="sxs-lookup"><span data-stu-id="4b156-113">Configuration Manager Client Id from SCCM</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b156-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4b156-114">Relationships</span></span>
<span data-ttu-id="4b156-115">なし</span><span class="sxs-lookup"><span data-stu-id="4b156-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b156-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4b156-116">JSON Representation</span></span>
<span data-ttu-id="4b156-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4b156-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientInformation",
  "clientIdentifier": "String"
}
```



