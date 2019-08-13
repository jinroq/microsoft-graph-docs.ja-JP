---
title: windows10AssociatedApps リソースの種類
description: Windows 10 関連アプリケーションの定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 438448d90dcbe5fa1922dfd3b51c28d3d5f80ecf
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337896"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="8d9ff-103">windows10AssociatedApps リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8d9ff-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="8d9ff-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d9ff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d9ff-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8d9ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d9ff-106">Windows 10 関連アプリケーションの定義。</span><span class="sxs-lookup"><span data-stu-id="8d9ff-106">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="8d9ff-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d9ff-107">Properties</span></span>
|<span data-ttu-id="8d9ff-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d9ff-108">Property</span></span>|<span data-ttu-id="8d9ff-109">型</span><span class="sxs-lookup"><span data-stu-id="8d9ff-109">Type</span></span>|<span data-ttu-id="8d9ff-110">説明</span><span class="sxs-lookup"><span data-stu-id="8d9ff-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d9ff-111">appType</span><span class="sxs-lookup"><span data-stu-id="8d9ff-111">appType</span></span>|[<span data-ttu-id="8d9ff-112">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="8d9ff-112">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="8d9ff-113">アプリケーションの種類。</span><span class="sxs-lookup"><span data-stu-id="8d9ff-113">Application type.</span></span> <span data-ttu-id="8d9ff-114">可能な値は、`desktop`、`universal` です。</span><span class="sxs-lookup"><span data-stu-id="8d9ff-114">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="8d9ff-115">識別子</span><span class="sxs-lookup"><span data-stu-id="8d9ff-115">identifier</span></span>|<span data-ttu-id="8d9ff-116">String</span><span class="sxs-lookup"><span data-stu-id="8d9ff-116">String</span></span>|<span data-ttu-id="8d9ff-117">識別子.</span><span class="sxs-lookup"><span data-stu-id="8d9ff-117">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d9ff-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8d9ff-118">Relationships</span></span>
<span data-ttu-id="8d9ff-119">なし</span><span class="sxs-lookup"><span data-stu-id="8d9ff-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d9ff-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8d9ff-120">JSON Representation</span></span>
<span data-ttu-id="8d9ff-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8d9ff-121">Here is a JSON representation of the resource.</span></span>
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



