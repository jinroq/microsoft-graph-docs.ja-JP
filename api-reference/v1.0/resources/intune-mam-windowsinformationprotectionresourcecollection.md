---
title: windowsInformationProtectionResourceCollection リソースの種類
description: Windows 情報保護のリソース コレクション
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 754f5ce902ca4cb5bb63be41f0e8094cc0738c26
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037640"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="6ff4e-103">windowsInformationProtectionResourceCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6ff4e-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="6ff4e-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6ff4e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ff4e-105">Windows 情報保護のリソース コレクション</span><span class="sxs-lookup"><span data-stu-id="6ff4e-105">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="6ff4e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ff4e-106">Properties</span></span>
|<span data-ttu-id="6ff4e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ff4e-107">Property</span></span>|<span data-ttu-id="6ff4e-108">型</span><span class="sxs-lookup"><span data-stu-id="6ff4e-108">Type</span></span>|<span data-ttu-id="6ff4e-109">説明</span><span class="sxs-lookup"><span data-stu-id="6ff4e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ff4e-110">displayName</span><span class="sxs-lookup"><span data-stu-id="6ff4e-110">displayName</span></span>|<span data-ttu-id="6ff4e-111">String</span><span class="sxs-lookup"><span data-stu-id="6ff4e-111">String</span></span>|<span data-ttu-id="6ff4e-112">表示名</span><span class="sxs-lookup"><span data-stu-id="6ff4e-112">Display name</span></span>|
|<span data-ttu-id="6ff4e-113">リソース</span><span class="sxs-lookup"><span data-stu-id="6ff4e-113">resources</span></span>|<span data-ttu-id="6ff4e-114">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="6ff4e-114">String collection</span></span>|<span data-ttu-id="6ff4e-115">リソースのコレクション</span><span class="sxs-lookup"><span data-stu-id="6ff4e-115">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ff4e-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6ff4e-116">Relationships</span></span>
<span data-ttu-id="6ff4e-117">なし</span><span class="sxs-lookup"><span data-stu-id="6ff4e-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ff4e-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6ff4e-118">JSON Representation</span></span>
<span data-ttu-id="6ff4e-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6ff4e-119">Here is a JSON representation of the resource.</span></span>
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



