---
title: deviceManagementUserRightsLocalUserOrGroup リソースの種類
description: ユーザー権限の設定に使用されるローカルユーザーまたはグループの情報を表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e41a5dbf5d4756e7c635bfdf87aca46f54d8139f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970410"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="66c7e-103">deviceManagementUserRightsLocalUserOrGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="66c7e-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="66c7e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66c7e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66c7e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="66c7e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66c7e-106">ユーザー権限の設定に使用されるローカルユーザーまたはグループの情報を表します。</span><span class="sxs-lookup"><span data-stu-id="66c7e-106">Represents information for a local user or group used for user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="66c7e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66c7e-107">Properties</span></span>
|<span data-ttu-id="66c7e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66c7e-108">Property</span></span>|<span data-ttu-id="66c7e-109">型</span><span class="sxs-lookup"><span data-stu-id="66c7e-109">Type</span></span>|<span data-ttu-id="66c7e-110">説明</span><span class="sxs-lookup"><span data-stu-id="66c7e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66c7e-111">name</span><span class="sxs-lookup"><span data-stu-id="66c7e-111">name</span></span>|<span data-ttu-id="66c7e-112">String</span><span class="sxs-lookup"><span data-stu-id="66c7e-112">String</span></span>|<span data-ttu-id="66c7e-113">このローカルユーザーまたはグループの名前。</span><span class="sxs-lookup"><span data-stu-id="66c7e-113">The name of this local user or group.</span></span>|
|<span data-ttu-id="66c7e-114">description</span><span class="sxs-lookup"><span data-stu-id="66c7e-114">description</span></span>|<span data-ttu-id="66c7e-115">String</span><span class="sxs-lookup"><span data-stu-id="66c7e-115">String</span></span>|<span data-ttu-id="66c7e-116">このローカルユーザーまたはグループの管理者の説明。</span><span class="sxs-lookup"><span data-stu-id="66c7e-116">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="66c7e-117">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="66c7e-117">securityIdentifier</span></span>|<span data-ttu-id="66c7e-118">String</span><span class="sxs-lookup"><span data-stu-id="66c7e-118">String</span></span>|<span data-ttu-id="66c7e-119">このローカルユーザーまたはグループのセキュリティ識別子 (たとえば \* S-1-5-32-544)。</span><span class="sxs-lookup"><span data-stu-id="66c7e-119">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="66c7e-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="66c7e-120">Relationships</span></span>
<span data-ttu-id="66c7e-121">なし</span><span class="sxs-lookup"><span data-stu-id="66c7e-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="66c7e-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="66c7e-122">JSON Representation</span></span>
<span data-ttu-id="66c7e-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="66c7e-123">Here is a JSON representation of the resource.</span></span>
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





