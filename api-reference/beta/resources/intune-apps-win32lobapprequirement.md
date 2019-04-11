---
title: win32LobAppRequirement リソースの種類
description: Win32 アプリを検出するための基本クラス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a3177493c5289b54cb43369a9dc62970097486f9
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31809288"
---
# <a name="win32lobapprequirement-resource-type"></a><span data-ttu-id="8c75b-103">win32LobAppRequirement リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8c75b-103">win32LobAppRequirement resource type</span></span>

> <span data-ttu-id="8c75b-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c75b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c75b-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8c75b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c75b-106">Win32 アプリを検出するための基本クラス</span><span class="sxs-lookup"><span data-stu-id="8c75b-106">Base class to detect a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="8c75b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8c75b-107">Properties</span></span>
|<span data-ttu-id="8c75b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8c75b-108">Property</span></span>|<span data-ttu-id="8c75b-109">型</span><span class="sxs-lookup"><span data-stu-id="8c75b-109">Type</span></span>|<span data-ttu-id="8c75b-110">説明</span><span class="sxs-lookup"><span data-stu-id="8c75b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c75b-111">operator</span><span class="sxs-lookup"><span data-stu-id="8c75b-111">operator</span></span>|[<span data-ttu-id="8c75b-112">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="8c75b-112">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="8c75b-113">検出のための演算子。</span><span class="sxs-lookup"><span data-stu-id="8c75b-113">The operator for detection.</span></span> <span data-ttu-id="8c75b-114">可能な値は、`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual` です。</span><span class="sxs-lookup"><span data-stu-id="8c75b-114">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="8c75b-115">detectionValue</span><span class="sxs-lookup"><span data-stu-id="8c75b-115">detectionValue</span></span>|<span data-ttu-id="8c75b-116">文字列</span><span class="sxs-lookup"><span data-stu-id="8c75b-116">String</span></span>|<span data-ttu-id="8c75b-117">検出値</span><span class="sxs-lookup"><span data-stu-id="8c75b-117">The detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c75b-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8c75b-118">Relationships</span></span>
<span data-ttu-id="8c75b-119">なし</span><span class="sxs-lookup"><span data-stu-id="8c75b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c75b-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8c75b-120">JSON Representation</span></span>
<span data-ttu-id="8c75b-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8c75b-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRequirement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRequirement",
  "operator": "String",
  "detectionValue": "String"
}
```





