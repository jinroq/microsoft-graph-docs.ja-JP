---
title: windowsInformationProtectionResourceCollection リソースの種類
description: Windows 情報保護のリソース コレクション
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74d7549f57ecc59f70aa1af4350544ec21b156ec
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254822"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="b5764-103">windowsInformationProtectionResourceCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b5764-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="b5764-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b5764-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5764-105">Windows 情報保護のリソース コレクション</span><span class="sxs-lookup"><span data-stu-id="b5764-105">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="b5764-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5764-106">Properties</span></span>
|<span data-ttu-id="b5764-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5764-107">Property</span></span>|<span data-ttu-id="b5764-108">型</span><span class="sxs-lookup"><span data-stu-id="b5764-108">Type</span></span>|<span data-ttu-id="b5764-109">説明</span><span class="sxs-lookup"><span data-stu-id="b5764-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5764-110">displayName</span><span class="sxs-lookup"><span data-stu-id="b5764-110">displayName</span></span>|<span data-ttu-id="b5764-111">文字列</span><span class="sxs-lookup"><span data-stu-id="b5764-111">String</span></span>|<span data-ttu-id="b5764-112">表示名</span><span class="sxs-lookup"><span data-stu-id="b5764-112">Display name</span></span>|
|<span data-ttu-id="b5764-113">リソース</span><span class="sxs-lookup"><span data-stu-id="b5764-113">resources</span></span>|<span data-ttu-id="b5764-114">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="b5764-114">String collection</span></span>|<span data-ttu-id="b5764-115">リソースのコレクション</span><span class="sxs-lookup"><span data-stu-id="b5764-115">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5764-116">関係</span><span class="sxs-lookup"><span data-stu-id="b5764-116">Relationships</span></span>
<span data-ttu-id="b5764-117">なし</span><span class="sxs-lookup"><span data-stu-id="b5764-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5764-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b5764-118">JSON Representation</span></span>
<span data-ttu-id="b5764-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b5764-119">Here is a JSON representation of the resource.</span></span>
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



