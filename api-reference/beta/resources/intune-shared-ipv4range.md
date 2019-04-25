---
title: iPv4Range リソースの種類
description: IPv4 の範囲定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c896eb6f9a35992d7370cf29124d8072c171eb30
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550596"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="86547-103">iPv4Range リソースの種類</span><span class="sxs-lookup"><span data-stu-id="86547-103">iPv4Range resource type</span></span>

> <span data-ttu-id="86547-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86547-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86547-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="86547-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86547-106">IPv4 の範囲定義。</span><span class="sxs-lookup"><span data-stu-id="86547-106">IPv4 Range definition.</span></span>


<span data-ttu-id="86547-107">[ipRange](../resources/intune-shared-iprange.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="86547-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="86547-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86547-108">Properties</span></span>
|<span data-ttu-id="86547-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86547-109">Property</span></span>|<span data-ttu-id="86547-110">型</span><span class="sxs-lookup"><span data-stu-id="86547-110">Type</span></span>|<span data-ttu-id="86547-111">説明</span><span class="sxs-lookup"><span data-stu-id="86547-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86547-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="86547-112">lowerAddress</span></span>|<span data-ttu-id="86547-113">String</span><span class="sxs-lookup"><span data-stu-id="86547-113">String</span></span>|<span data-ttu-id="86547-114">小さいアドレス。</span><span class="sxs-lookup"><span data-stu-id="86547-114">Lower address.</span></span>|
|<span data-ttu-id="86547-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="86547-115">upperAddress</span></span>|<span data-ttu-id="86547-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="86547-116">String</span></span>|<span data-ttu-id="86547-117">上住所</span><span class="sxs-lookup"><span data-stu-id="86547-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86547-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="86547-118">Relationships</span></span>
<span data-ttu-id="86547-119">なし</span><span class="sxs-lookup"><span data-stu-id="86547-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="86547-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="86547-120">JSON Representation</span></span>
<span data-ttu-id="86547-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="86547-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv4Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv4Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```





