---
title: deviceManagementSettingRegexConstraint リソースの種類
description: 指定された RegEx パターンに対して設定の一致を強制する制約
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d0f9a04583bfb9b28546e9057f0530f72558a0be
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364636"
---
# <a name="devicemanagementsettingregexconstraint-resource-type"></a><span data-ttu-id="1efea-103">deviceManagementSettingRegexConstraint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1efea-103">deviceManagementSettingRegexConstraint resource type</span></span>

> <span data-ttu-id="1efea-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1efea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1efea-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1efea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1efea-106">指定された RegEx パターンに対して設定の一致を強制する制約</span><span class="sxs-lookup"><span data-stu-id="1efea-106">Constraint enforcing the setting matches against a given RegEx pattern</span></span>


<span data-ttu-id="1efea-107">[Devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="1efea-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1efea-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1efea-108">Properties</span></span>
|<span data-ttu-id="1efea-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1efea-109">Property</span></span>|<span data-ttu-id="1efea-110">型</span><span class="sxs-lookup"><span data-stu-id="1efea-110">Type</span></span>|<span data-ttu-id="1efea-111">説明</span><span class="sxs-lookup"><span data-stu-id="1efea-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1efea-112">pcre</span><span class="sxs-lookup"><span data-stu-id="1efea-112">regex</span></span>|<span data-ttu-id="1efea-113">String</span><span class="sxs-lookup"><span data-stu-id="1efea-113">String</span></span>|<span data-ttu-id="1efea-114">照合する正規表現パターン</span><span class="sxs-lookup"><span data-stu-id="1efea-114">The RegEx pattern to match against</span></span>|

## <a name="relationships"></a><span data-ttu-id="1efea-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1efea-115">Relationships</span></span>
<span data-ttu-id="1efea-116">なし</span><span class="sxs-lookup"><span data-stu-id="1efea-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1efea-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1efea-117">JSON Representation</span></span>
<span data-ttu-id="1efea-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1efea-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingRegexConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingRegexConstraint",
  "regex": "String"
}
```



