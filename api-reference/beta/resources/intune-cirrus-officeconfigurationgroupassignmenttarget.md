---
title: officeConfigurationGroupAssignmentTarget リソースの種類
description: Office クライアント構成 AAD グループの割り当て先。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7a3451d4bddec96c1e21cd605b05cb34d96372ff
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526392"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="21452-103">officeConfigurationGroupAssignmentTarget リソースの種類</span><span class="sxs-lookup"><span data-stu-id="21452-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="21452-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="21452-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21452-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="21452-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21452-106">Office クライアント構成 AAD グループの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="21452-106">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="21452-107">[officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="21452-107">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="21452-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21452-108">Properties</span></span>
|<span data-ttu-id="21452-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21452-109">Property</span></span>|<span data-ttu-id="21452-110">型</span><span class="sxs-lookup"><span data-stu-id="21452-110">Type</span></span>|<span data-ttu-id="21452-111">説明</span><span class="sxs-lookup"><span data-stu-id="21452-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21452-112">groupId</span><span class="sxs-lookup"><span data-stu-id="21452-112">groupId</span></span>|<span data-ttu-id="21452-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="21452-113">String</span></span>|<span data-ttu-id="21452-114">デバイス構成を対象としている AAD グループの Id。</span><span class="sxs-lookup"><span data-stu-id="21452-114">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21452-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="21452-115">Relationships</span></span>
<span data-ttu-id="21452-116">なし</span><span class="sxs-lookup"><span data-stu-id="21452-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="21452-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="21452-117">JSON Representation</span></span>
<span data-ttu-id="21452-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="21452-118">Here is a JSON representation of the resource.</span></span>
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



