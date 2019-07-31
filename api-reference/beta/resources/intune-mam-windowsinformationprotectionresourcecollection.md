---
title: windowsInformationProtectionResourceCollection リソースの種類
description: Windows 情報保護のリソース コレクション
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7f8f21fcdf33676520301dbaeccefc12696375cf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967841"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="f3fb7-103">windowsInformationProtectionResourceCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f3fb7-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="f3fb7-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3fb7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3fb7-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3fb7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3fb7-106">Windows 情報保護のリソース コレクション</span><span class="sxs-lookup"><span data-stu-id="f3fb7-106">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="f3fb7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3fb7-107">Properties</span></span>
|<span data-ttu-id="f3fb7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3fb7-108">Property</span></span>|<span data-ttu-id="f3fb7-109">型</span><span class="sxs-lookup"><span data-stu-id="f3fb7-109">Type</span></span>|<span data-ttu-id="f3fb7-110">説明</span><span class="sxs-lookup"><span data-stu-id="f3fb7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3fb7-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f3fb7-111">displayName</span></span>|<span data-ttu-id="f3fb7-112">String</span><span class="sxs-lookup"><span data-stu-id="f3fb7-112">String</span></span>|<span data-ttu-id="f3fb7-113">表示名</span><span class="sxs-lookup"><span data-stu-id="f3fb7-113">Display name</span></span>|
|<span data-ttu-id="f3fb7-114">リソース</span><span class="sxs-lookup"><span data-stu-id="f3fb7-114">resources</span></span>|<span data-ttu-id="f3fb7-115">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="f3fb7-115">String collection</span></span>|<span data-ttu-id="f3fb7-116">リソースのコレクション</span><span class="sxs-lookup"><span data-stu-id="f3fb7-116">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3fb7-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f3fb7-117">Relationships</span></span>
<span data-ttu-id="f3fb7-118">なし</span><span class="sxs-lookup"><span data-stu-id="f3fb7-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3fb7-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f3fb7-119">JSON Representation</span></span>
<span data-ttu-id="f3fb7-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f3fb7-120">Here is a JSON representation of the resource.</span></span>
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





