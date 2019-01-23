---
title: exclusionGroupAssignmentTarget リソースの種類
description: 割り当てから除外するグループを表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a42cab192a9cd643c6c11de596ca0790fa8b4a5c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421887"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="b4d96-103">exclusionGroupAssignmentTarget リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b4d96-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="b4d96-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b4d96-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b4d96-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4d96-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b4d96-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b4d96-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4d96-107">割り当てから除外するグループを表します。</span><span class="sxs-lookup"><span data-stu-id="b4d96-107">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="b4d96-108">[groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="b4d96-108">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b4d96-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b4d96-109">Properties</span></span>
|<span data-ttu-id="b4d96-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b4d96-110">Property</span></span>|<span data-ttu-id="b4d96-111">型</span><span class="sxs-lookup"><span data-stu-id="b4d96-111">Type</span></span>|<span data-ttu-id="b4d96-112">説明</span><span class="sxs-lookup"><span data-stu-id="b4d96-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4d96-113">groupId</span><span class="sxs-lookup"><span data-stu-id="b4d96-113">groupId</span></span>|<span data-ttu-id="b4d96-114">文字列</span><span class="sxs-lookup"><span data-stu-id="b4d96-114">String</span></span>|<span data-ttu-id="b4d96-115">割り当てのターゲットとなるグループ ID です。</span><span class="sxs-lookup"><span data-stu-id="b4d96-115">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="b4d96-116">[groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="b4d96-116">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4d96-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b4d96-117">Relationships</span></span>
<span data-ttu-id="b4d96-118">なし</span><span class="sxs-lookup"><span data-stu-id="b4d96-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4d96-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b4d96-119">JSON Representation</span></span>
<span data-ttu-id="b4d96-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b4d96-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.exclusionGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exclusionGroupAssignmentTarget",
  "groupId": "String"
}
```




