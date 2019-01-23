---
title: officeConfigurationGroupAssignmentTarget リソースの種類
description: AAD Office クライアントの構成は、ターゲットの割り当てをグループ化します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 411af117999498050288405874bd6b5baff5b6b5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422748"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="c327c-103">officeConfigurationGroupAssignmentTarget リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c327c-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="c327c-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c327c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c327c-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c327c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c327c-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c327c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c327c-107">AAD Office クライアントの構成は、ターゲットの割り当てをグループ化します。</span><span class="sxs-lookup"><span data-stu-id="c327c-107">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="c327c-108">[OfficeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c327c-108">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c327c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c327c-109">Properties</span></span>
|<span data-ttu-id="c327c-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c327c-110">Property</span></span>|<span data-ttu-id="c327c-111">型</span><span class="sxs-lookup"><span data-stu-id="c327c-111">Type</span></span>|<span data-ttu-id="c327c-112">説明</span><span class="sxs-lookup"><span data-stu-id="c327c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c327c-113">groupId</span><span class="sxs-lookup"><span data-stu-id="c327c-113">groupId</span></span>|<span data-ttu-id="c327c-114">String</span><span class="sxs-lookup"><span data-stu-id="c327c-114">String</span></span>|<span data-ttu-id="c327c-115">AAD グループの Id は、対象としてデバイスを構成します。</span><span class="sxs-lookup"><span data-stu-id="c327c-115">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c327c-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c327c-116">Relationships</span></span>
<span data-ttu-id="c327c-117">なし</span><span class="sxs-lookup"><span data-stu-id="c327c-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c327c-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c327c-118">JSON Representation</span></span>
<span data-ttu-id="c327c-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c327c-119">Here is a JSON representation of the resource.</span></span>
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



