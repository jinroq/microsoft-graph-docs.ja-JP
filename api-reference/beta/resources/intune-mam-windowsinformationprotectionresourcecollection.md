---
title: windowsInformationProtectionResourceCollection リソースの種類
description: Windows 情報保護のリソース コレクション
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e5a303ad0b05813a4e44dc2208ff1b8692242d88
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561846"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="6ff3f-103">windowsInformationProtectionResourceCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6ff3f-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="6ff3f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ff3f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ff3f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6ff3f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ff3f-106">Windows 情報保護のリソース コレクション</span><span class="sxs-lookup"><span data-stu-id="6ff3f-106">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="6ff3f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ff3f-107">Properties</span></span>
|<span data-ttu-id="6ff3f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ff3f-108">Property</span></span>|<span data-ttu-id="6ff3f-109">型</span><span class="sxs-lookup"><span data-stu-id="6ff3f-109">Type</span></span>|<span data-ttu-id="6ff3f-110">説明</span><span class="sxs-lookup"><span data-stu-id="6ff3f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ff3f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="6ff3f-111">displayName</span></span>|<span data-ttu-id="6ff3f-112">String</span><span class="sxs-lookup"><span data-stu-id="6ff3f-112">String</span></span>|<span data-ttu-id="6ff3f-113">表示名</span><span class="sxs-lookup"><span data-stu-id="6ff3f-113">Display name</span></span>|
|<span data-ttu-id="6ff3f-114">リソース</span><span class="sxs-lookup"><span data-stu-id="6ff3f-114">resources</span></span>|<span data-ttu-id="6ff3f-115">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="6ff3f-115">String collection</span></span>|<span data-ttu-id="6ff3f-116">リソースのコレクション</span><span class="sxs-lookup"><span data-stu-id="6ff3f-116">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ff3f-117">関係</span><span class="sxs-lookup"><span data-stu-id="6ff3f-117">Relationships</span></span>
<span data-ttu-id="6ff3f-118">なし</span><span class="sxs-lookup"><span data-stu-id="6ff3f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ff3f-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6ff3f-119">JSON Representation</span></span>
<span data-ttu-id="6ff3f-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6ff3f-120">Here is a JSON representation of the resource.</span></span>
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





