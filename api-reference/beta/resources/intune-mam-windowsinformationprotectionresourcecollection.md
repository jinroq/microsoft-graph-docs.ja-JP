---
title: windowsInformationProtectionResourceCollection リソースの種類
description: Windows 情報保護のリソース コレクション
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c4a8ad51177507613c3fd84b524503d0e79c208f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424680"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="c1a94-103">windowsInformationProtectionResourceCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c1a94-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="c1a94-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c1a94-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c1a94-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c1a94-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1a94-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c1a94-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1a94-107">Windows 情報保護のリソース コレクション</span><span class="sxs-lookup"><span data-stu-id="c1a94-107">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="c1a94-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1a94-108">Properties</span></span>
|<span data-ttu-id="c1a94-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1a94-109">Property</span></span>|<span data-ttu-id="c1a94-110">型</span><span class="sxs-lookup"><span data-stu-id="c1a94-110">Type</span></span>|<span data-ttu-id="c1a94-111">説明</span><span class="sxs-lookup"><span data-stu-id="c1a94-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1a94-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c1a94-112">displayName</span></span>|<span data-ttu-id="c1a94-113">文字列</span><span class="sxs-lookup"><span data-stu-id="c1a94-113">String</span></span>|<span data-ttu-id="c1a94-114">表示名</span><span class="sxs-lookup"><span data-stu-id="c1a94-114">Display name</span></span>|
|<span data-ttu-id="c1a94-115">リソース</span><span class="sxs-lookup"><span data-stu-id="c1a94-115">resources</span></span>|<span data-ttu-id="c1a94-116">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="c1a94-116">String collection</span></span>|<span data-ttu-id="c1a94-117">リソースのコレクション</span><span class="sxs-lookup"><span data-stu-id="c1a94-117">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1a94-118">関係</span><span class="sxs-lookup"><span data-stu-id="c1a94-118">Relationships</span></span>
<span data-ttu-id="c1a94-119">なし</span><span class="sxs-lookup"><span data-stu-id="c1a94-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1a94-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c1a94-120">JSON Representation</span></span>
<span data-ttu-id="c1a94-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c1a94-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionResourceCollection",
  "displayName": "String",
  "resources": [
    "String"
  ]
}
```




