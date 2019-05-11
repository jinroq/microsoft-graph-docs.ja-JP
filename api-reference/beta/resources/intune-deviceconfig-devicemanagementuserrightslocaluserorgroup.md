---
title: deviceManagementUserRightsLocalUserOrGroup リソースの種類
description: ユーザー権限の設定に使用されるローカルユーザーまたはグループの情報を表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: acccbb68ecc0b62d27ac20e3eba9e637aac3e11c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946939"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="e8ad9-103">deviceManagementUserRightsLocalUserOrGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e8ad9-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="e8ad9-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8ad9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8ad9-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e8ad9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8ad9-106">ユーザー権限の設定に使用されるローカルユーザーまたはグループの情報を表します。</span><span class="sxs-lookup"><span data-stu-id="e8ad9-106">Represents information for a local user or group used for user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="e8ad9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8ad9-107">Properties</span></span>
|<span data-ttu-id="e8ad9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8ad9-108">Property</span></span>|<span data-ttu-id="e8ad9-109">型</span><span class="sxs-lookup"><span data-stu-id="e8ad9-109">Type</span></span>|<span data-ttu-id="e8ad9-110">説明</span><span class="sxs-lookup"><span data-stu-id="e8ad9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8ad9-111">name</span><span class="sxs-lookup"><span data-stu-id="e8ad9-111">name</span></span>|<span data-ttu-id="e8ad9-112">String</span><span class="sxs-lookup"><span data-stu-id="e8ad9-112">String</span></span>|<span data-ttu-id="e8ad9-113">このローカルユーザーまたはグループの名前。</span><span class="sxs-lookup"><span data-stu-id="e8ad9-113">The name of this local user or group.</span></span>|
|<span data-ttu-id="e8ad9-114">description</span><span class="sxs-lookup"><span data-stu-id="e8ad9-114">description</span></span>|<span data-ttu-id="e8ad9-115">String</span><span class="sxs-lookup"><span data-stu-id="e8ad9-115">String</span></span>|<span data-ttu-id="e8ad9-116">このローカルユーザーまたはグループの管理者の説明。</span><span class="sxs-lookup"><span data-stu-id="e8ad9-116">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="e8ad9-117">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="e8ad9-117">securityIdentifier</span></span>|<span data-ttu-id="e8ad9-118">String</span><span class="sxs-lookup"><span data-stu-id="e8ad9-118">String</span></span>|<span data-ttu-id="e8ad9-119">このローカルユーザーまたはグループのセキュリティ識別子 (たとえば \* S-1-5-32-544)。</span><span class="sxs-lookup"><span data-stu-id="e8ad9-119">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8ad9-120">関係</span><span class="sxs-lookup"><span data-stu-id="e8ad9-120">Relationships</span></span>
<span data-ttu-id="e8ad9-121">なし</span><span class="sxs-lookup"><span data-stu-id="e8ad9-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8ad9-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e8ad9-122">JSON Representation</span></span>
<span data-ttu-id="e8ad9-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e8ad9-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
  "name": "String",
  "description": "String",
  "securityIdentifier": "String"
}
```




