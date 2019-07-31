---
title: officeConfigurationGroupAssignmentTarget リソースの種類
description: Office クライアント構成 AAD グループの割り当て先。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fb97541a86e820e02e56a20568d3869a047dc2c3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011961"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="866f6-103">officeConfigurationGroupAssignmentTarget リソースの種類</span><span class="sxs-lookup"><span data-stu-id="866f6-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="866f6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="866f6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="866f6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="866f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="866f6-106">Office クライアント構成 AAD グループの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="866f6-106">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="866f6-107">[OfficeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="866f6-107">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="866f6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="866f6-108">Properties</span></span>
|<span data-ttu-id="866f6-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="866f6-109">Property</span></span>|<span data-ttu-id="866f6-110">型</span><span class="sxs-lookup"><span data-stu-id="866f6-110">Type</span></span>|<span data-ttu-id="866f6-111">説明</span><span class="sxs-lookup"><span data-stu-id="866f6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="866f6-112">groupId</span><span class="sxs-lookup"><span data-stu-id="866f6-112">groupId</span></span>|<span data-ttu-id="866f6-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="866f6-113">String</span></span>|<span data-ttu-id="866f6-114">デバイス構成を対象としている AAD グループの Id。</span><span class="sxs-lookup"><span data-stu-id="866f6-114">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="866f6-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="866f6-115">Relationships</span></span>
<span data-ttu-id="866f6-116">なし</span><span class="sxs-lookup"><span data-stu-id="866f6-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="866f6-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="866f6-117">JSON Representation</span></span>
<span data-ttu-id="866f6-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="866f6-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfigurationGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfigurationGroupAssignmentTarget",
  "groupId": "String"
}
```



