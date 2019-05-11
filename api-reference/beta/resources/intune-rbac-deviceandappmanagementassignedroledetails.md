---
title: deviceAndAppManagementAssignedRoleDetails リソースの種類
description: ユーザーに割り当てられた役割定義と役割の割り当てのセット。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 03b98e2d98774ae166bba6b9ab74d8e42953c78e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940030"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a><span data-ttu-id="0278c-103">deviceAndAppManagementAssignedRoleDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0278c-103">deviceAndAppManagementAssignedRoleDetails resource type</span></span>

> <span data-ttu-id="0278c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0278c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0278c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0278c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0278c-106">ユーザーに割り当てられた役割定義と役割の割り当てのセット。</span><span class="sxs-lookup"><span data-stu-id="0278c-106">The set of Role Definitions and Role Assignments assigned to a user.</span></span>

## <a name="properties"></a><span data-ttu-id="0278c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0278c-107">Properties</span></span>
|<span data-ttu-id="0278c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0278c-108">Property</span></span>|<span data-ttu-id="0278c-109">型</span><span class="sxs-lookup"><span data-stu-id="0278c-109">Type</span></span>|<span data-ttu-id="0278c-110">説明</span><span class="sxs-lookup"><span data-stu-id="0278c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0278c-111">roleDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="0278c-111">roleDefinitionIds</span></span>|<span data-ttu-id="0278c-112">String collection</span><span class="sxs-lookup"><span data-stu-id="0278c-112">String collection</span></span>|<span data-ttu-id="0278c-113">ユーザーに割り当てられている表面化ロール定義のロール定義 Id。</span><span class="sxs-lookup"><span data-stu-id="0278c-113">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="0278c-114">roleAssignmentIds</span><span class="sxs-lookup"><span data-stu-id="0278c-114">roleAssignmentIds</span></span>|<span data-ttu-id="0278c-115">String collection</span><span class="sxs-lookup"><span data-stu-id="0278c-115">String collection</span></span>|<span data-ttu-id="0278c-116">ユーザーに割り当てられている表面化の役割の割り当ての役割割り当て Id。</span><span class="sxs-lookup"><span data-stu-id="0278c-116">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0278c-117">関係</span><span class="sxs-lookup"><span data-stu-id="0278c-117">Relationships</span></span>
<span data-ttu-id="0278c-118">なし</span><span class="sxs-lookup"><span data-stu-id="0278c-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0278c-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0278c-119">JSON Representation</span></span>
<span data-ttu-id="0278c-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0278c-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceAndAppManagementAssignedRoleDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignedRoleDetails",
  "roleDefinitionIds": [
    "String"
  ],
  "roleAssignmentIds": [
    "String"
  ]
}
```




