---
title: windows10AssociatedApps リソースの種類
description: Windows 10 関連アプリケーションの定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 22adbc6be90718f95a574443c8bd2f96a55f2ee4
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31784643"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="971ba-103">windows10AssociatedApps リソースの種類</span><span class="sxs-lookup"><span data-stu-id="971ba-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="971ba-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="971ba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="971ba-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="971ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="971ba-106">Windows 10 関連アプリケーションの定義。</span><span class="sxs-lookup"><span data-stu-id="971ba-106">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="971ba-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="971ba-107">Properties</span></span>
|<span data-ttu-id="971ba-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="971ba-108">Property</span></span>|<span data-ttu-id="971ba-109">型</span><span class="sxs-lookup"><span data-stu-id="971ba-109">Type</span></span>|<span data-ttu-id="971ba-110">説明</span><span class="sxs-lookup"><span data-stu-id="971ba-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="971ba-111">appType</span><span class="sxs-lookup"><span data-stu-id="971ba-111">appType</span></span>|[<span data-ttu-id="971ba-112">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="971ba-112">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="971ba-113">アプリケーションの種類。</span><span class="sxs-lookup"><span data-stu-id="971ba-113">Application type.</span></span> <span data-ttu-id="971ba-114">可能な値は、`desktop`、`universal` です。</span><span class="sxs-lookup"><span data-stu-id="971ba-114">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="971ba-115">識別子</span><span class="sxs-lookup"><span data-stu-id="971ba-115">identifier</span></span>|<span data-ttu-id="971ba-116">文字列</span><span class="sxs-lookup"><span data-stu-id="971ba-116">String</span></span>|<span data-ttu-id="971ba-117">識別子.</span><span class="sxs-lookup"><span data-stu-id="971ba-117">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="971ba-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="971ba-118">Relationships</span></span>
<span data-ttu-id="971ba-119">なし</span><span class="sxs-lookup"><span data-stu-id="971ba-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="971ba-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="971ba-120">JSON Representation</span></span>
<span data-ttu-id="971ba-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="971ba-121">Here is a JSON representation of the resource.</span></span>
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





