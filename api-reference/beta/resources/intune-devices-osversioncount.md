---
title: osversioncount リソースの種類
description: 各 OS バージョンのマルウェアがあるデバイスの数
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7df4f920335c579e2e17cdeb275cc0545887f1d4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578730"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="13aa8-103">osversioncount リソースの種類</span><span class="sxs-lookup"><span data-stu-id="13aa8-103">osVersionCount resource type</span></span>

> <span data-ttu-id="13aa8-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13aa8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13aa8-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="13aa8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13aa8-106">各 OS バージョンのマルウェアがあるデバイスの数</span><span class="sxs-lookup"><span data-stu-id="13aa8-106">Count of devices with malware for each OS version</span></span>

## <a name="properties"></a><span data-ttu-id="13aa8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13aa8-107">Properties</span></span>
|<span data-ttu-id="13aa8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13aa8-108">Property</span></span>|<span data-ttu-id="13aa8-109">型</span><span class="sxs-lookup"><span data-stu-id="13aa8-109">Type</span></span>|<span data-ttu-id="13aa8-110">説明</span><span class="sxs-lookup"><span data-stu-id="13aa8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13aa8-111">osVersion</span><span class="sxs-lookup"><span data-stu-id="13aa8-111">osVersion</span></span>|<span data-ttu-id="13aa8-112">String</span><span class="sxs-lookup"><span data-stu-id="13aa8-112">String</span></span>|<span data-ttu-id="13aa8-113">OS のバージョン</span><span class="sxs-lookup"><span data-stu-id="13aa8-113">OS version</span></span>|
|<span data-ttu-id="13aa8-114">deviceCount</span><span class="sxs-lookup"><span data-stu-id="13aa8-114">deviceCount</span></span>|<span data-ttu-id="13aa8-115">Int32</span><span class="sxs-lookup"><span data-stu-id="13aa8-115">Int32</span></span>|<span data-ttu-id="13aa8-116">OS バージョン用のマルウェアがあるデバイスの数</span><span class="sxs-lookup"><span data-stu-id="13aa8-116">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="13aa8-117">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="13aa8-117">lastUpdateDateTime</span></span>|<span data-ttu-id="13aa8-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13aa8-118">DateTimeOffset</span></span>|<span data-ttu-id="13aa8-119">デバイス数の最終更新のタイムスタンプ (UTC)</span><span class="sxs-lookup"><span data-stu-id="13aa8-119">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="13aa8-120">関係</span><span class="sxs-lookup"><span data-stu-id="13aa8-120">Relationships</span></span>
<span data-ttu-id="13aa8-121">なし</span><span class="sxs-lookup"><span data-stu-id="13aa8-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13aa8-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="13aa8-122">JSON Representation</span></span>
<span data-ttu-id="13aa8-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="13aa8-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.osVersionCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.osVersionCount",
  "osVersion": "String",
  "deviceCount": 1024,
  "lastUpdateDateTime": "String (timestamp)"
}
```





