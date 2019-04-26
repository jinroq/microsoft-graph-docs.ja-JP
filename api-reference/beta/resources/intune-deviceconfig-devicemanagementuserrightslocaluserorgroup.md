---
title: deviceManagementUserRightsLocalUserOrGroup リソースの種類
description: ユーザー権限の設定に使用されるローカルユーザーまたはグループの情報を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cfdb49ef0b98e3d76d092b1ebf9574d6df8c47d9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567201"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="68433-103">deviceManagementUserRightsLocalUserOrGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="68433-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="68433-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68433-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68433-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="68433-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68433-106">ユーザー権限の設定に使用されるローカルユーザーまたはグループの情報を表します。</span><span class="sxs-lookup"><span data-stu-id="68433-106">Represents information for a local user or group used for user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="68433-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68433-107">Properties</span></span>
|<span data-ttu-id="68433-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68433-108">Property</span></span>|<span data-ttu-id="68433-109">型</span><span class="sxs-lookup"><span data-stu-id="68433-109">Type</span></span>|<span data-ttu-id="68433-110">説明</span><span class="sxs-lookup"><span data-stu-id="68433-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68433-111">name</span><span class="sxs-lookup"><span data-stu-id="68433-111">name</span></span>|<span data-ttu-id="68433-112">String</span><span class="sxs-lookup"><span data-stu-id="68433-112">String</span></span>|<span data-ttu-id="68433-113">このローカルユーザーまたはグループの名前。</span><span class="sxs-lookup"><span data-stu-id="68433-113">The name of this local user or group.</span></span>|
|<span data-ttu-id="68433-114">説明</span><span class="sxs-lookup"><span data-stu-id="68433-114">description</span></span>|<span data-ttu-id="68433-115">String</span><span class="sxs-lookup"><span data-stu-id="68433-115">String</span></span>|<span data-ttu-id="68433-116">このローカルユーザーまたはグループの管理者の説明。</span><span class="sxs-lookup"><span data-stu-id="68433-116">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="68433-117">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="68433-117">securityIdentifier</span></span>|<span data-ttu-id="68433-118">String</span><span class="sxs-lookup"><span data-stu-id="68433-118">String</span></span>|<span data-ttu-id="68433-119">このローカルユーザーまたはグループのセキュリティ識別子 (たとえば \* S-1-5-32-544)。</span><span class="sxs-lookup"><span data-stu-id="68433-119">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="68433-120">関係</span><span class="sxs-lookup"><span data-stu-id="68433-120">Relationships</span></span>
<span data-ttu-id="68433-121">なし</span><span class="sxs-lookup"><span data-stu-id="68433-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="68433-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="68433-122">JSON Representation</span></span>
<span data-ttu-id="68433-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="68433-123">Here is a JSON representation of the resource.</span></span>
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





