---
title: deviceAndAppManagementAssignedRoleDetails リソースの種類
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d6ace16ba496feb24948c3e40c32dd8fcb2fcf48
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29428900"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a><span data-ttu-id="f77c3-103">deviceAndAppManagementAssignedRoleDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f77c3-103">deviceAndAppManagementAssignedRoleDetails resource type</span></span>

> <span data-ttu-id="f77c3-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f77c3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f77c3-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f77c3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f77c3-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f77c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f77c3-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f77c3-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f77c3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f77c3-108">Properties</span></span>
|<span data-ttu-id="f77c3-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f77c3-109">Property</span></span>|<span data-ttu-id="f77c3-110">型</span><span class="sxs-lookup"><span data-stu-id="f77c3-110">Type</span></span>|<span data-ttu-id="f77c3-111">説明</span><span class="sxs-lookup"><span data-stu-id="f77c3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f77c3-112">roleDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="f77c3-112">roleDefinitionIds</span></span>|<span data-ttu-id="f77c3-113">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f77c3-113">String collection</span></span>|<span data-ttu-id="f77c3-114">特定ユーザーに割り当てられているロールの定義のロール定義の Id。</span><span class="sxs-lookup"><span data-stu-id="f77c3-114">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="f77c3-115">roleAssignmentIds</span><span class="sxs-lookup"><span data-stu-id="f77c3-115">roleAssignmentIds</span></span>|<span data-ttu-id="f77c3-116">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f77c3-116">String collection</span></span>|<span data-ttu-id="f77c3-117">ロールの割り当てがユーザーに割り当て、特定のロールの割り当ての Id です。</span><span class="sxs-lookup"><span data-stu-id="f77c3-117">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f77c3-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f77c3-118">Relationships</span></span>
<span data-ttu-id="f77c3-119">なし</span><span class="sxs-lookup"><span data-stu-id="f77c3-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f77c3-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f77c3-120">JSON Representation</span></span>
<span data-ttu-id="f77c3-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f77c3-121">Here is a JSON representation of the resource.</span></span>
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




