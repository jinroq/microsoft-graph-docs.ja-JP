---
title: windows10AssociatedApps リソースの種類
description: Windows 10 関連アプリケーションの定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3b53f2b2ec70a2d7420a754a795905da5b1dcb4a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34992753"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="39b34-103">windows10AssociatedApps リソースの種類</span><span class="sxs-lookup"><span data-stu-id="39b34-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="39b34-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="39b34-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39b34-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="39b34-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39b34-106">Windows 10 関連アプリケーションの定義。</span><span class="sxs-lookup"><span data-stu-id="39b34-106">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="39b34-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39b34-107">Properties</span></span>
|<span data-ttu-id="39b34-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39b34-108">Property</span></span>|<span data-ttu-id="39b34-109">型</span><span class="sxs-lookup"><span data-stu-id="39b34-109">Type</span></span>|<span data-ttu-id="39b34-110">説明</span><span class="sxs-lookup"><span data-stu-id="39b34-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39b34-111">appType</span><span class="sxs-lookup"><span data-stu-id="39b34-111">appType</span></span>|[<span data-ttu-id="39b34-112">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="39b34-112">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="39b34-113">アプリケーションの種類。</span><span class="sxs-lookup"><span data-stu-id="39b34-113">Application type.</span></span> <span data-ttu-id="39b34-114">可能な値は、`desktop`、`universal` です。</span><span class="sxs-lookup"><span data-stu-id="39b34-114">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="39b34-115">識別子</span><span class="sxs-lookup"><span data-stu-id="39b34-115">identifier</span></span>|<span data-ttu-id="39b34-116">String</span><span class="sxs-lookup"><span data-stu-id="39b34-116">String</span></span>|<span data-ttu-id="39b34-117">識別子.</span><span class="sxs-lookup"><span data-stu-id="39b34-117">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39b34-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="39b34-118">Relationships</span></span>
<span data-ttu-id="39b34-119">なし</span><span class="sxs-lookup"><span data-stu-id="39b34-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="39b34-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="39b34-120">JSON Representation</span></span>
<span data-ttu-id="39b34-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="39b34-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AssociatedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AssociatedApps",
  "appType": "String",
  "identifier": "String"
}
```





