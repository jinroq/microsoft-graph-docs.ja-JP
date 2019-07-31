---
title: " secureScoreControlStateUpdate リソースの種類"
description: このリソースには、ユーザーによって更新されたコントロールの状態の履歴が含まれます (コントロールの状態には、Default、ThirdParty、、レビュー済み) があります。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 92616569a87a6ccf91c17ea7c845b8185bd33e8b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965230"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="6e1dd-103">secureScoreControlStateUpdate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6e1dd-103">secureScoreControlStateUpdate resource type</span></span>
<span data-ttu-id="6e1dd-104">ユーザーによって更新されたコントロールの状態の履歴が含まれます (コントロールの状態には、既定では、無視される、ThirdParty、レビューされます)。</span><span class="sxs-lookup"><span data-stu-id="6e1dd-104">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

|<span data-ttu-id="6e1dd-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6e1dd-105">Property</span></span> |<span data-ttu-id="6e1dd-106">型</span><span class="sxs-lookup"><span data-stu-id="6e1dd-106">Type</span></span> |<span data-ttu-id="6e1dd-107">説明</span><span class="sxs-lookup"><span data-stu-id="6e1dd-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="6e1dd-108">assignedTo</span><span class="sxs-lookup"><span data-stu-id="6e1dd-108">assignedTo</span></span> | <span data-ttu-id="6e1dd-109">string</span><span class="sxs-lookup"><span data-stu-id="6e1dd-109">string</span></span> | <span data-ttu-id="6e1dd-110">アクションを実行するユーザーにコントロールを割り当てる</span><span class="sxs-lookup"><span data-stu-id="6e1dd-110">Assign the control to the user who will take the action</span></span> |
|<span data-ttu-id="6e1dd-111">comment</span><span class="sxs-lookup"><span data-stu-id="6e1dd-111">comment</span></span> | <span data-ttu-id="6e1dd-112">string</span><span class="sxs-lookup"><span data-stu-id="6e1dd-112">string</span></span> | <span data-ttu-id="6e1dd-113">コントロールに関するオプションのコメントを提供します。</span><span class="sxs-lookup"><span data-stu-id="6e1dd-113">Provides optional comment about the control</span></span> |
|<span data-ttu-id="6e1dd-114">state</span><span class="sxs-lookup"><span data-stu-id="6e1dd-114">state</span></span> | <span data-ttu-id="6e1dd-115">string</span><span class="sxs-lookup"><span data-stu-id="6e1dd-115">string</span></span> | <span data-ttu-id="6e1dd-116">PATCH コマンドを使用してコントロールの状態を変更できます (例: 無視、thirdParty など)</span><span class="sxs-lookup"><span data-stu-id="6e1dd-116">State of the control can be modified using PATCH command(Ex: ignored, thirdParty etc)</span></span> |
|<span data-ttu-id="6e1dd-117">updatedBy</span><span class="sxs-lookup"><span data-stu-id="6e1dd-117">updatedBy</span></span> | <span data-ttu-id="6e1dd-118">string</span><span class="sxs-lookup"><span data-stu-id="6e1dd-118">string</span></span> |<span data-ttu-id="6e1dd-119">テナント状態を更新したユーザーの ID</span><span class="sxs-lookup"><span data-stu-id="6e1dd-119">ID of the user who updated tenant state</span></span> |
|<span data-ttu-id="6e1dd-120">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="6e1dd-120">updatedDateTime</span></span> | <span data-ttu-id="6e1dd-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e1dd-121">DateTimeOffset</span></span> |<span data-ttu-id="6e1dd-122">コントロールの状態が更新された時刻</span><span class="sxs-lookup"><span data-stu-id="6e1dd-122">Time at which control state was updated</span></span> |
 ## <a name="json-representation"></a><span data-ttu-id="6e1dd-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6e1dd-123">JSON representation</span></span>
 <span data-ttu-id="6e1dd-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6e1dd-124">The following is a JSON representation of the resource.</span></span>
 <!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
}-->
 ```json
{
  "assignedTo": "String",
  "comment": "string",
  "state": "string",
  "updatedBy": "string",
  "updatedDateTime": "DateTimeOffset"
}
 ```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
