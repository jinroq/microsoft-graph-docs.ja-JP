---
title: secureScoreControlStateUpdate リソースの種類
description: このリソースには、ユーザーが更新したコントロールの状態の履歴が含まれています (コントロールの状態には、Default、ThirdParty、、レビュー済み) などがあります。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9e051f2c4319a2b2ae1e3dbd9ba633785a345c4a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034476"
---
#  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="c268d-103">secureScoreControlStateUpdate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c268d-103">secureScoreControlStateUpdate resource type</span></span>

<span data-ttu-id="c268d-104">ユーザーによって更新されたコントロールの状態の履歴が含まれます (コントロールの状態には、既定では、無視される、ThirdParty、レビューされます)。</span><span class="sxs-lookup"><span data-stu-id="c268d-104">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

## <a name="properties"></a><span data-ttu-id="c268d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c268d-105">Properties</span></span>

|<span data-ttu-id="c268d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c268d-106">Property</span></span> |<span data-ttu-id="c268d-107">型</span><span class="sxs-lookup"><span data-stu-id="c268d-107">Type</span></span> |<span data-ttu-id="c268d-108">説明</span><span class="sxs-lookup"><span data-stu-id="c268d-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="c268d-109">assignedTo</span><span class="sxs-lookup"><span data-stu-id="c268d-109">assignedTo</span></span>|<span data-ttu-id="c268d-110">String</span><span class="sxs-lookup"><span data-stu-id="c268d-110">String</span></span>|<span data-ttu-id="c268d-111">アクションを実行するユーザーにコントロールを割り当てます。</span><span class="sxs-lookup"><span data-stu-id="c268d-111">Assigns the control to the user who will take the action.</span></span> |
|<span data-ttu-id="c268d-112">comment</span><span class="sxs-lookup"><span data-stu-id="c268d-112">comment</span></span>|<span data-ttu-id="c268d-113">String</span><span class="sxs-lookup"><span data-stu-id="c268d-113">String</span></span>|<span data-ttu-id="c268d-114">コントロールに関するコメント (省略可能) を提供します。</span><span class="sxs-lookup"><span data-stu-id="c268d-114">Provides optional comment about the control.</span></span> |
|<span data-ttu-id="c268d-115">state</span><span class="sxs-lookup"><span data-stu-id="c268d-115">state</span></span>|<span data-ttu-id="c268d-116">String</span><span class="sxs-lookup"><span data-stu-id="c268d-116">String</span></span>|<span data-ttu-id="c268d-117">コントロールの状態。 PATCH コマンドで変更することができます (たとえば、無視、thirdParty)。</span><span class="sxs-lookup"><span data-stu-id="c268d-117">State of the control, which can be modified via a PATCH command (for example, ignored, thirdParty).</span></span> |
|<span data-ttu-id="c268d-118">updatedBy</span><span class="sxs-lookup"><span data-stu-id="c268d-118">updatedBy</span></span>|<span data-ttu-id="c268d-119">String</span><span class="sxs-lookup"><span data-stu-id="c268d-119">String</span></span>|<span data-ttu-id="c268d-120">テナントの状態を更新したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="c268d-120">ID of the user who updated tenant state.</span></span> |
|<span data-ttu-id="c268d-121">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="c268d-121">updatedDateTime</span></span>|<span data-ttu-id="c268d-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c268d-122">DateTimeOffset</span></span>|<span data-ttu-id="c268d-123">コントロールの状態が更新された時刻。</span><span class="sxs-lookup"><span data-stu-id="c268d-123">Time at which the control state was updated.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c268d-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c268d-124">JSON representation</span></span>
 <span data-ttu-id="c268d-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c268d-125">The following is a JSON representation of the resource.</span></span>
 <!-- {
  "blockType": "resource",
  "optionalProperties": [
    
   ],
  "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
}-->
 ```json
{
  "assignedTo": "String",
  "comment": "String",
  "state": "String",
  "updatedBy": "String",
  "updatedDateTime": "String (timestamp)"
}
 ```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
