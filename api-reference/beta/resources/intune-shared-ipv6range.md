---
title: iPv6Range リソースの種類
description: IPv6 範囲の定義。
author: rolyon
localization_priority: Normal
doc_type: resourcePageType
ms.prod: Intune
ms.openlocfilehash: 1f2b46cea71d097955ca9e78cc74f6f0cddd1002
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967378"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="ffbbb-103">iPv6Range リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ffbbb-103">iPv6Range resource type</span></span>

> <span data-ttu-id="ffbbb-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ffbbb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ffbbb-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ffbbb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffbbb-106">IPv6 範囲の定義。</span><span class="sxs-lookup"><span data-stu-id="ffbbb-106">IPv6 Range definition.</span></span>


<span data-ttu-id="ffbbb-107">[ipRange](../resources/intune-shared-iprange.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="ffbbb-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ffbbb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ffbbb-108">Properties</span></span>
|<span data-ttu-id="ffbbb-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ffbbb-109">Property</span></span>|<span data-ttu-id="ffbbb-110">型</span><span class="sxs-lookup"><span data-stu-id="ffbbb-110">Type</span></span>|<span data-ttu-id="ffbbb-111">説明</span><span class="sxs-lookup"><span data-stu-id="ffbbb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffbbb-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="ffbbb-112">lowerAddress</span></span>|<span data-ttu-id="ffbbb-113">String</span><span class="sxs-lookup"><span data-stu-id="ffbbb-113">String</span></span>|<span data-ttu-id="ffbbb-114">小さいアドレス。</span><span class="sxs-lookup"><span data-stu-id="ffbbb-114">Lower address.</span></span>|
|<span data-ttu-id="ffbbb-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="ffbbb-115">upperAddress</span></span>|<span data-ttu-id="ffbbb-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ffbbb-116">String</span></span>|<span data-ttu-id="ffbbb-117">上住所</span><span class="sxs-lookup"><span data-stu-id="ffbbb-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ffbbb-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ffbbb-118">Relationships</span></span>
<span data-ttu-id="ffbbb-119">なし</span><span class="sxs-lookup"><span data-stu-id="ffbbb-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ffbbb-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ffbbb-120">JSON Representation</span></span>
<span data-ttu-id="ffbbb-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ffbbb-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv6Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv6Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```





