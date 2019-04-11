---
title: deviceAndAppManagementAssignedRoleDetails リソースの種類
description: ユーザーに割り当てられた役割定義と役割の割り当てのセット。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 93f99cdc91d046b9ebf292bbd34f1bba39b494ac
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771405"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a><span data-ttu-id="dcf17-103">deviceAndAppManagementAssignedRoleDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dcf17-103">deviceAndAppManagementAssignedRoleDetails resource type</span></span>

> <span data-ttu-id="dcf17-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dcf17-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dcf17-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dcf17-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcf17-106">ユーザーに割り当てられた役割定義と役割の割り当てのセット。</span><span class="sxs-lookup"><span data-stu-id="dcf17-106">The set of Role Definitions and Role Assignments assigned to a user.</span></span>

## <a name="properties"></a><span data-ttu-id="dcf17-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dcf17-107">Properties</span></span>
|<span data-ttu-id="dcf17-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dcf17-108">Property</span></span>|<span data-ttu-id="dcf17-109">型</span><span class="sxs-lookup"><span data-stu-id="dcf17-109">Type</span></span>|<span data-ttu-id="dcf17-110">説明</span><span class="sxs-lookup"><span data-stu-id="dcf17-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcf17-111">roledefinitionids</span><span class="sxs-lookup"><span data-stu-id="dcf17-111">roleDefinitionIds</span></span>|<span data-ttu-id="dcf17-112">String コレクション</span><span class="sxs-lookup"><span data-stu-id="dcf17-112">String collection</span></span>|<span data-ttu-id="dcf17-113">ユーザーに割り当てられている表面化ロール定義のロール定義 id。</span><span class="sxs-lookup"><span data-stu-id="dcf17-113">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="dcf17-114">roleAssignmentIds</span><span class="sxs-lookup"><span data-stu-id="dcf17-114">roleAssignmentIds</span></span>|<span data-ttu-id="dcf17-115">String コレクション</span><span class="sxs-lookup"><span data-stu-id="dcf17-115">String collection</span></span>|<span data-ttu-id="dcf17-116">ユーザーに割り当てられている表面化の役割の割り当ての役割割り当て id。</span><span class="sxs-lookup"><span data-stu-id="dcf17-116">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dcf17-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dcf17-117">Relationships</span></span>
<span data-ttu-id="dcf17-118">なし</span><span class="sxs-lookup"><span data-stu-id="dcf17-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dcf17-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dcf17-119">JSON Representation</span></span>
<span data-ttu-id="dcf17-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dcf17-120">Here is a JSON representation of the resource.</span></span>
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





