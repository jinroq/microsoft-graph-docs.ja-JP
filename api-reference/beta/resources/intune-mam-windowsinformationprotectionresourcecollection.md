---
title: windowsInformationProtectionResourceCollection リソースの種類
description: Windows 情報保護のリソース コレクション
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1bc8cb6afbf49c34d0a081eb6b6ae876df7cf1f6
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993705"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="71942-103">windowsInformationProtectionResourceCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="71942-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="71942-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71942-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71942-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="71942-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71942-106">Windows 情報保護のリソース コレクション</span><span class="sxs-lookup"><span data-stu-id="71942-106">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="71942-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="71942-107">Properties</span></span>
|<span data-ttu-id="71942-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="71942-108">Property</span></span>|<span data-ttu-id="71942-109">型</span><span class="sxs-lookup"><span data-stu-id="71942-109">Type</span></span>|<span data-ttu-id="71942-110">説明</span><span class="sxs-lookup"><span data-stu-id="71942-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71942-111">displayName</span><span class="sxs-lookup"><span data-stu-id="71942-111">displayName</span></span>|<span data-ttu-id="71942-112">String</span><span class="sxs-lookup"><span data-stu-id="71942-112">String</span></span>|<span data-ttu-id="71942-113">表示名</span><span class="sxs-lookup"><span data-stu-id="71942-113">Display name</span></span>|
|<span data-ttu-id="71942-114">リソース</span><span class="sxs-lookup"><span data-stu-id="71942-114">resources</span></span>|<span data-ttu-id="71942-115">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="71942-115">String collection</span></span>|<span data-ttu-id="71942-116">リソースのコレクション</span><span class="sxs-lookup"><span data-stu-id="71942-116">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="71942-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="71942-117">Relationships</span></span>
<span data-ttu-id="71942-118">なし</span><span class="sxs-lookup"><span data-stu-id="71942-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="71942-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="71942-119">JSON Representation</span></span>
<span data-ttu-id="71942-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="71942-120">Here is a JSON representation of the resource.</span></span>
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





